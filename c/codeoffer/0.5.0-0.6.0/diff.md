# Comparing `tmp/codeoffer-0.5.0.tar.gz` & `tmp/codeoffer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/codeoffer-0.5.0.tar", last modified: Wed May 10 10:47:15 2023, max compression
+gzip compressed data, was "dist/codeoffer-0.6.0.tar", last modified: Wed May 10 11:19:23 2023, max compression
```

## Comparing `codeoffer-0.5.0.tar` & `codeoffer-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 maximilianosinski   (501) staff       (20)        0 2023-05-10 10:47:15.000000 codeoffer-0.5.0/
--rw-r--r--   0 maximilianosinski   (501) staff       (20)       17 2023-05-10 10:44:55.000000 codeoffer-0.5.0/MANIFEST.in
--rw-r--r--   0 maximilianosinski   (501) staff       (20)     3498 2023-05-10 10:47:15.000000 codeoffer-0.5.0/PKG-INFO
--rw-r--r--   0 maximilianosinski   (501) staff       (20)     2394 2023-05-10 10:38:10.000000 codeoffer-0.5.0/README.md
-drwxr-xr-x   0 maximilianosinski   (501) staff       (20)        0 2023-05-10 10:47:15.000000 codeoffer-0.5.0/codeoffer.egg-info/
--rw-r--r--   0 maximilianosinski   (501) staff       (20)     3498 2023-05-10 10:47:15.000000 codeoffer-0.5.0/codeoffer.egg-info/PKG-INFO
--rw-r--r--   0 maximilianosinski   (501) staff       (20)      162 2023-05-10 10:47:15.000000 codeoffer-0.5.0/codeoffer.egg-info/SOURCES.txt
--rw-r--r--   0 maximilianosinski   (501) staff       (20)        1 2023-05-10 10:47:15.000000 codeoffer-0.5.0/codeoffer.egg-info/dependency_links.txt
--rw-r--r--   0 maximilianosinski   (501) staff       (20)        1 2023-05-10 10:47:15.000000 codeoffer-0.5.0/codeoffer.egg-info/top_level.txt
--rw-r--r--   0 maximilianosinski   (501) staff       (20)       38 2023-05-10 10:47:15.000000 codeoffer-0.5.0/setup.cfg
--rw-r--r--   0 maximilianosinski   (501) staff       (20)      642 2023-05-10 10:47:08.000000 codeoffer-0.5.0/setup.py
+drwxr-xr-x   0 maximilianosinski   (501) staff       (20)        0 2023-05-10 11:19:23.000000 codeoffer-0.6.0/
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)       17 2023-05-10 10:44:55.000000 codeoffer-0.6.0/MANIFEST.in
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)     3693 2023-05-10 11:19:23.000000 codeoffer-0.6.0/PKG-INFO
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)     2429 2023-05-10 11:17:31.000000 codeoffer-0.6.0/README.md
+drwxr-xr-x   0 maximilianosinski   (501) staff       (20)        0 2023-05-10 11:19:23.000000 codeoffer-0.6.0/codeoffer.egg-info/
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)     3693 2023-05-10 11:19:23.000000 codeoffer-0.6.0/codeoffer.egg-info/PKG-INFO
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)      162 2023-05-10 11:19:23.000000 codeoffer-0.6.0/codeoffer.egg-info/SOURCES.txt
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)        1 2023-05-10 11:19:23.000000 codeoffer-0.6.0/codeoffer.egg-info/dependency_links.txt
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)        1 2023-05-10 11:19:23.000000 codeoffer-0.6.0/codeoffer.egg-info/top_level.txt
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)       38 2023-05-10 11:19:23.000000 codeoffer-0.6.0/setup.cfg
+-rw-r--r--   0 maximilianosinski   (501) staff       (20)      642 2023-05-10 11:19:12.000000 codeoffer-0.6.0/setup.py
```

### Comparing `codeoffer-0.5.0/PKG-INFO` & `codeoffer-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,112 @@
 Metadata-Version: 2.1
 Name: codeoffer
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python library that simplifies access to the Public CodeOffer API
 Home-page: https://github.com/codeoffer/v1-python-library
 Author: CodeOffer
 Author-email: contact@codeoffer.net
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/codeoffer/v1-python-library
 Project-URL: Source, https://github.com/codeoffer/v1-python-library
 Description: # CodeOffer Python Package
         
-        This is a Python package that provides an API wrapper for the public CodeOffer API. The package simplifies authentication and management of in-app assets for developers who use the CodeOffer API in their applications.
+        CodeOffer is a Python package that provides an API wrapper for the public CodeOffer API. The package simplifies authentication and management of in-app assets for developers who use the CodeOffer API in their applications.
         
         ## Installation
         
         To install the package, run the following command:
         
-        `pip install codeoffer` 
+        ```py
+        pip install codeoffer
+        ``` 
         
         ## Usage
         
         Import the `codeoffer` class from the package:
         
         ### Authentication & Sessions
         
         Initialize a new session, but first you need to import the `oauth` class from `codeoffer`
         
-        `from codeoffer import oauth`
+        ```py
+        from codeoffer import oauth
+        ```
         
         After that you can create a new session token:
         
-        `token = session.create_session_token()`
+        ```py
+        token = session.create_session_token()
+        ```
         
         Now get the login link and ask the user to log in:
         `token.get_login_link()`
         
         Right after that call the `token.wait_for_confirmation()` method, this method will wait until the user completed the login-process.
         
         To return the current logged in user you need to import the `user` class from `codeoffer`
         
-        `from codeoffer import user`
+        ```py
+        from codeoffer import user
+        ```
         
         Then you can return the current user by using the `get_user` method and passing the token as a parameter:
         
-        `user = user.User.get_user(token)`
+        ```py
+        user = user.User.get_user(token)
+        ```
         
         And now you can get the username, email, profile picture and access to the current logged in app (if the user purchased / downloaded the app with his account)
         
-        `print(f"Hey {user.username}")`
+        ```py
+        print(f"Hey {user.username}")
+        ```
         
         ### Assets
         
         You can return all the apps your app contains.
         
         First import the `app` class from `codeoffer`
         
-        `from codeoffer import app`
+        ```py
+        from codeoffer import app
+        ```
         
         Then you need to initialize the app with a session token.
         
-        `app = app.App.by_session_token(token)`
+        ```py
+        app = app.App.by_session_token(token)
+        ```
         
         After that you can return all the assets your app contains and return properties like the name, identifier and if the user has access to that asset.
         
-        `assets = app.get_asset_directory()`
-        
-            for asset in assets:  
-        	    print(f"{asset.name}: {asset.access}")
+        ```py
+        assets = app.get_asset_directory()
+        ```
+        ```py
+        for asset in assets:  
+        	print(f"{asset.name}: {asset.access}")
+        ```
         
         #### Complete Example
-        
-            from codeoffer import oauth  
-            from codeoffer import app  
-            from codeoffer import user  
+        ```py
+        from codeoffer import oauth  
+        from codeoffer import app  
+        from codeoffer import user  
               
-            session = oauth.Session("10aa641e562bdd82d2f8449d")  
-            token = session.create_session_token()  
-            token.get_login_link()  
-            token.wait_for_confirmation()  
-            user = user.User.get_user(token)  
-            print(f"Hey {user.username}")  
-            app = app.App.by_session_token(token)  
-            assets = app.get_asset_directory()  
-            for asset in assets:  
-        	    print(f"{asset.name}: {asset.access}")
+        session = oauth.Session("10aa641e562bdd82d2f8449d")  
+        token = session.create_session_token()  
+        token.get_login_link()  
+        token.wait_for_confirmation()  
+        user = user.User.get_user(token)  
+        print(f"Hey {user.username}")  
+        app = app.App.by_session_token(token)  
+        assets = app.get_asset_directory()  
+        for asset in assets:  
+        	print(f"{asset.name}: {asset.access}")
+        ```
         
         ## License
         
         This package is licensed under the MIT License.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `codeoffer-0.5.0/README.md` & `codeoffer-0.6.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,80 +1,100 @@
 # CodeOffer Python Package
 
-This is a Python package that provides an API wrapper for the public CodeOffer API. The package simplifies authentication and management of in-app assets for developers who use the CodeOffer API in their applications.
+CodeOffer is a Python package that provides an API wrapper for the public CodeOffer API. The package simplifies authentication and management of in-app assets for developers who use the CodeOffer API in their applications.
 
 ## Installation
 
 To install the package, run the following command:
 
-`pip install codeoffer` 
+```py
+pip install codeoffer
+``` 
 
 ## Usage
 
 Import the `codeoffer` class from the package:
 
 ### Authentication & Sessions
 
 Initialize a new session, but first you need to import the `oauth` class from `codeoffer`
 
-`from codeoffer import oauth`
+```py
+from codeoffer import oauth
+```
 
 After that you can create a new session token:
 
-`token = session.create_session_token()`
+```py
+token = session.create_session_token()
+```
 
 Now get the login link and ask the user to log in:
 `token.get_login_link()`
 
 Right after that call the `token.wait_for_confirmation()` method, this method will wait until the user completed the login-process.
 
 To return the current logged in user you need to import the `user` class from `codeoffer`
 
-`from codeoffer import user`
+```py
+from codeoffer import user
+```
 
 Then you can return the current user by using the `get_user` method and passing the token as a parameter:
 
-`user = user.User.get_user(token)`
+```py
+user = user.User.get_user(token)
+```
 
 And now you can get the username, email, profile picture and access to the current logged in app (if the user purchased / downloaded the app with his account)
 
-`print(f"Hey {user.username}")`
+```py
+print(f"Hey {user.username}")
+```
 
 ### Assets
 
 You can return all the apps your app contains.
 
 First import the `app` class from `codeoffer`
 
-`from codeoffer import app`
+```py
+from codeoffer import app
+```
 
 Then you need to initialize the app with a session token.
 
-`app = app.App.by_session_token(token)`
+```py
+app = app.App.by_session_token(token)
+```
 
 After that you can return all the assets your app contains and return properties like the name, identifier and if the user has access to that asset.
 
-`assets = app.get_asset_directory()`
-
-    for asset in assets:  
-	    print(f"{asset.name}: {asset.access}")
+```py
+assets = app.get_asset_directory()
+```
+```py
+for asset in assets:  
+	print(f"{asset.name}: {asset.access}")
+```
 
 #### Complete Example
-
-    from codeoffer import oauth  
-    from codeoffer import app  
-    from codeoffer import user  
+```py
+from codeoffer import oauth  
+from codeoffer import app  
+from codeoffer import user  
       
-    session = oauth.Session("10aa641e562bdd82d2f8449d")  
-    token = session.create_session_token()  
-    token.get_login_link()  
-    token.wait_for_confirmation()  
-    user = user.User.get_user(token)  
-    print(f"Hey {user.username}")  
-    app = app.App.by_session_token(token)  
-    assets = app.get_asset_directory()  
-    for asset in assets:  
-	    print(f"{asset.name}: {asset.access}")
+session = oauth.Session("10aa641e562bdd82d2f8449d")  
+token = session.create_session_token()  
+token.get_login_link()  
+token.wait_for_confirmation()  
+user = user.User.get_user(token)  
+print(f"Hey {user.username}")  
+app = app.App.by_session_token(token)  
+assets = app.get_asset_directory()  
+for asset in assets:  
+	print(f"{asset.name}: {asset.access}")
+```
 
 ## License
 
 This package is licensed under the MIT License.
```

### Comparing `codeoffer-0.5.0/codeoffer.egg-info/PKG-INFO` & `codeoffer-0.6.0/codeoffer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,92 +1,112 @@
 Metadata-Version: 2.1
 Name: codeoffer
-Version: 0.5.0
+Version: 0.6.0
 Summary: Python library that simplifies access to the Public CodeOffer API
 Home-page: https://github.com/codeoffer/v1-python-library
 Author: CodeOffer
 Author-email: contact@codeoffer.net
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/codeoffer/v1-python-library
 Project-URL: Source, https://github.com/codeoffer/v1-python-library
 Description: # CodeOffer Python Package
         
-        This is a Python package that provides an API wrapper for the public CodeOffer API. The package simplifies authentication and management of in-app assets for developers who use the CodeOffer API in their applications.
+        CodeOffer is a Python package that provides an API wrapper for the public CodeOffer API. The package simplifies authentication and management of in-app assets for developers who use the CodeOffer API in their applications.
         
         ## Installation
         
         To install the package, run the following command:
         
-        `pip install codeoffer` 
+        ```py
+        pip install codeoffer
+        ``` 
         
         ## Usage
         
         Import the `codeoffer` class from the package:
         
         ### Authentication & Sessions
         
         Initialize a new session, but first you need to import the `oauth` class from `codeoffer`
         
-        `from codeoffer import oauth`
+        ```py
+        from codeoffer import oauth
+        ```
         
         After that you can create a new session token:
         
-        `token = session.create_session_token()`
+        ```py
+        token = session.create_session_token()
+        ```
         
         Now get the login link and ask the user to log in:
         `token.get_login_link()`
         
         Right after that call the `token.wait_for_confirmation()` method, this method will wait until the user completed the login-process.
         
         To return the current logged in user you need to import the `user` class from `codeoffer`
         
-        `from codeoffer import user`
+        ```py
+        from codeoffer import user
+        ```
         
         Then you can return the current user by using the `get_user` method and passing the token as a parameter:
         
-        `user = user.User.get_user(token)`
+        ```py
+        user = user.User.get_user(token)
+        ```
         
         And now you can get the username, email, profile picture and access to the current logged in app (if the user purchased / downloaded the app with his account)
         
-        `print(f"Hey {user.username}")`
+        ```py
+        print(f"Hey {user.username}")
+        ```
         
         ### Assets
         
         You can return all the apps your app contains.
         
         First import the `app` class from `codeoffer`
         
-        `from codeoffer import app`
+        ```py
+        from codeoffer import app
+        ```
         
         Then you need to initialize the app with a session token.
         
-        `app = app.App.by_session_token(token)`
+        ```py
+        app = app.App.by_session_token(token)
+        ```
         
         After that you can return all the assets your app contains and return properties like the name, identifier and if the user has access to that asset.
         
-        `assets = app.get_asset_directory()`
-        
-            for asset in assets:  
-        	    print(f"{asset.name}: {asset.access}")
+        ```py
+        assets = app.get_asset_directory()
+        ```
+        ```py
+        for asset in assets:  
+        	print(f"{asset.name}: {asset.access}")
+        ```
         
         #### Complete Example
-        
-            from codeoffer import oauth  
-            from codeoffer import app  
-            from codeoffer import user  
+        ```py
+        from codeoffer import oauth  
+        from codeoffer import app  
+        from codeoffer import user  
               
-            session = oauth.Session("10aa641e562bdd82d2f8449d")  
-            token = session.create_session_token()  
-            token.get_login_link()  
-            token.wait_for_confirmation()  
-            user = user.User.get_user(token)  
-            print(f"Hey {user.username}")  
-            app = app.App.by_session_token(token)  
-            assets = app.get_asset_directory()  
-            for asset in assets:  
-        	    print(f"{asset.name}: {asset.access}")
+        session = oauth.Session("10aa641e562bdd82d2f8449d")  
+        token = session.create_session_token()  
+        token.get_login_link()  
+        token.wait_for_confirmation()  
+        user = user.User.get_user(token)  
+        print(f"Hey {user.username}")  
+        app = app.App.by_session_token(token)  
+        assets = app.get_asset_directory()  
+        for asset in assets:  
+        	print(f"{asset.name}: {asset.access}")
+        ```
         
         ## License
         
         This package is licensed under the MIT License.
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `codeoffer-0.5.0/setup.py` & `codeoffer-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='codeoffer',
-    version='0.5.0',
+    version='0.6.0',
     description='Python library that simplifies access to the Public CodeOffer API',
     author='CodeOffer',
     author_email='contact@codeoffer.net',
     packages=find_packages(),
     url='https://github.com/codeoffer/v1-python-library',
     project_urls={
         'Documentation': 'https://github.com/codeoffer/v1-python-library',
```

