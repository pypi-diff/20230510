# Comparing `tmp/afex-sso-0.0.43.tar.gz` & `tmp/afex-sso-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-sso-0.0.43.tar", last modified: Wed May 10 09:17:38 2023, max compression
+gzip compressed data, was "afex-sso-0.0.5.tar", last modified: Wed May 10 09:41:01 2023, max compression
```

## Comparing `afex-sso-0.0.43.tar` & `afex-sso-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.131185 afex-sso-0.0.43/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-03-04 00:13:16.000000 afex-sso-0.0.43/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     1615 2023-05-10 09:17:38.131260 afex-sso-0.0.43/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1170 2023-05-10 08:31:16.000000 afex-sso-0.0.43/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.128414 afex-sso-0.0.43/app/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.129661 afex-sso-0.0.43/app/AFEX_SSO/
--rw-r--r--   0 mac        (501) staff       (20)       33 2023-03-20 23:30:24.000000 afex-sso-0.0.43/app/AFEX_SSO/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.130359 afex-sso-0.0.43/app/AFEX_SSO/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-03-20 23:17:21.000000 afex-sso-0.0.43/app/AFEX_SSO/src/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1706 2023-05-10 08:17:42.000000 afex-sso-0.0.43/app/AFEX_SSO/src/sso.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:17:38.131055 afex-sso-0.0.43/app/afex_sso.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1615 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      308 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       61 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        9 2023-05-10 09:17:38.000000 afex-sso-0.0.43/app/afex_sso.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)      134 2023-03-15 21:51:52.000000 afex-sso-0.0.43/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)      474 2023-05-10 09:17:38.131556 afex-sso-0.0.43/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      802 2023-05-10 09:05:27.000000 afex-sso-0.0.43/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:41:01.139875 afex-sso-0.0.5/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-03-04 00:13:16.000000 afex-sso-0.0.5/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)     1614 2023-05-10 09:41:01.139947 afex-sso-0.0.5/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1170 2023-05-10 08:31:16.000000 afex-sso-0.0.5/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:41:01.137439 afex-sso-0.0.5/app/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:41:01.138456 afex-sso-0.0.5/app/AFEX_SSO/
+-rw-r--r--   0 mac        (501) staff       (20)       33 2023-03-20 23:30:24.000000 afex-sso-0.0.5/app/AFEX_SSO/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:41:01.139001 afex-sso-0.0.5/app/AFEX_SSO/src/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-03-20 23:17:21.000000 afex-sso-0.0.5/app/AFEX_SSO/src/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1705 2023-05-10 09:40:13.000000 afex-sso-0.0.5/app/AFEX_SSO/src/sso.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-10 09:41:01.139716 afex-sso-0.0.5/app/afex_sso.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1614 2023-05-10 09:41:01.000000 afex-sso-0.0.5/app/afex_sso.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      308 2023-05-10 09:41:01.000000 afex-sso-0.0.5/app/afex_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-10 09:41:01.000000 afex-sso-0.0.5/app/afex_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       61 2023-05-10 09:41:01.000000 afex-sso-0.0.5/app/afex_sso.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        9 2023-05-10 09:41:01.000000 afex-sso-0.0.5/app/afex_sso.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)      134 2023-03-15 21:51:52.000000 afex-sso-0.0.5/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)      474 2023-05-10 09:41:01.140220 afex-sso-0.0.5/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      801 2023-05-10 09:40:49.000000 afex-sso-0.0.5/setup.py
```

### Comparing `afex-sso-0.0.43/LICENSE` & `afex-sso-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.43/PKG-INFO` & `afex-sso-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.43
+Version: 0.0.5
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `afex-sso-0.0.43/README.md` & `afex-sso-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.43/app/AFEX_SSO/src/sso.py` & `afex-sso-0.0.5/app/AFEX_SSO/src/sso.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         try:
             headers = {
                 "api-key": sp_api_key,
                 "hash-key":  sp_hash_key,
                 "request-ts": session_key
             }
             response = requests.get(
-                f"{URL}/v1/api/verify_sp/{self.session}", headers=headers)
+                f"{URL}/v1/api/verify_sp/{session_key}", headers=headers)
             data = json.loads(response.text)
             return data
 
         except Exception as e:
             return f"Something went wrong, please confirm the credentials and try again: {e}"
 
     def sign_out(self, sp_api_key, sp_hash_key, session_key, email: str):
```

### Comparing `afex-sso-0.0.43/app/afex_sso.egg-info/PKG-INFO` & `afex-sso-0.0.5/app/afex_sso.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.43
+Version: 0.0.5
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
 Author-email: it@africaexchange.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `afex-sso-0.0.43/setup.py` & `afex-sso-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="afex-sso",
-    version="0.0.43",
+    version="0.0.5",
     description="For integrating sso",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="AFEX NIGERIA",
```

