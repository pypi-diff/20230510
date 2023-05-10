# Comparing `tmp/fyers_token_manager_v2-0.0.3.tar.gz` & `tmp/fyers_token_manager_v2-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_token_manager_v2-0.0.3.tar", last modified: Wed May 10 05:00:34 2023, max compression
+gzip compressed data, was "fyers_token_manager_v2-0.0.4.tar", last modified: Wed May 10 05:10:53 2023, max compression
```

## Comparing `fyers_token_manager_v2-0.0.3.tar` & `fyers_token_manager_v2-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.3/LICENSE
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 04:19:57.000000 fyers_token_manager_v2-0.0.3/README.md
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4523 2023-05-10 04:19:45.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2/__init__.py
-drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/PKG-INFO
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/SOURCES.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/dependency_links.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        9 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/requires.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:00:34.000000 fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/top_level.txt
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:00:34.457183 fyers_token_manager_v2-0.0.3/setup.cfg
--rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      690 2023-05-10 04:58:29.000000 fyers_token_manager_v2-0.0.3/setup.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:10:53.951569 fyers_token_manager_v2-0.0.4/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       11 2022-10-12 11:09:01.000000 fyers_token_manager_v2-0.0.4/LICENSE
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:10:53.951569 fyers_token_manager_v2-0.0.4/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      786 2023-05-10 04:19:57.000000 fyers_token_manager_v2-0.0.4/README.md
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:10:53.947569 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     4868 2023-05-10 05:10:03.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2/__init__.py
+drwxrwxr-x   0 krunaldodiya  (1000) krunaldodiya  (1000)        0 2023-05-10 05:10:53.947569 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)     1120 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/PKG-INFO
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      290 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/SOURCES.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)        1 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/dependency_links.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       15 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/requires.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       23 2023-05-10 05:10:53.000000 fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/top_level.txt
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)       38 2023-05-10 05:10:53.951569 fyers_token_manager_v2-0.0.4/setup.cfg
+-rw-rw-r--   0 krunaldodiya  (1000) krunaldodiya  (1000)      682 2023-05-10 05:10:45.000000 fyers_token_manager_v2-0.0.4/setup.py
```

### Comparing `fyers_token_manager_v2-0.0.3/PKG-INFO` & `fyers_token_manager_v2-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_token_manager_v2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.0.3/README.md` & `fyers_token_manager_v2-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fyers_token_manager_v2-0.0.3/fyers_token_manager_v2/__init__.py` & `fyers_token_manager_v2-0.0.4/fyers_token_manager_v2/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,14 +66,25 @@
         return token
 
     def __write_file(self, token):
         with open(f"{fyers_access_token_path}", "w") as f:
             f.write(token)
 
     def __get_token(self):
+        session = self.__accessToken.SessionModel(
+            client_id=self.client_id,
+            secret_key=self.secret_key,
+            redirect_uri=self.redirect_uri,
+            response_type="code",
+        )
+
+        auth_code = session.generate_authcode()
+
+        print(f"if app is not activated, you can activate using", auth_code)
+
         headers = {
             "Accept": "application/json",
             "Accept-Language": "en-US,en;q=0.9",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36",
         }
 
         s = requests.Session()
```

### Comparing `fyers_token_manager_v2-0.0.3/fyers_token_manager_v2.egg-info/PKG-INFO` & `fyers_token_manager_v2-0.0.4/fyers_token_manager_v2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-token-manager-v2
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fyers Token Manager
 Home-page: https://github.com/krunaldodiya/fyers_token_manager
 Author: Krunal Dodiya
 Author-email: kunal.dodiya1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fyers_token_manager_v2-0.0.3/setup.py` & `fyers_token_manager_v2-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,21 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     include_package_data=True,
     name="fyers_token_manager_v2",
-    version="0.0.3",
+    version="0.0.4",
     description="Fyers Token Manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/krunaldodiya/fyers_token_manager",
     author="Krunal Dodiya",
     author_email="kunal.dodiya1@gmail.com",
     packages=setuptools.find_packages(),
-    install_requires=[
-        "requests",
-    ],
+    install_requires=["requests", "pyotp"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
 )
```

