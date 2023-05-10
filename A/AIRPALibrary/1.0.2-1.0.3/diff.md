# Comparing `tmp/AIRPALibrary-1.0.2.tar.gz` & `tmp/AIRPALibrary-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AIRPALibrary\dist\.tmp-0gs4tgcd\AIRPALibrary-1.0.2.tar", last modified: Wed Mar 29 03:11:27 2023, max compression
+gzip compressed data, was "D:\Annas\SAP Modified\Build Wheel\AIRPALibrary\dist\.tmp-jwf5fnke\AIRPALibrary-1.0.3.tar", last modified: Wed May 10 04:15:50 2023, max compression
```

## Comparing `AIRPALibrary-1.0.2.tar` & `AIRPALibrary-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/
--rw-rw-rw-   0        0        0      299 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      637 2023-03-13 07:36:18.000000 AIRPALibrary-1.0.2/README.md
--rw-rw-rw-   0        0        0      529 2023-03-29 03:11:04.000000 AIRPALibrary-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/src/AIRPALibrary/
--rw-rw-rw-   0        0        0     8216 2023-03-29 03:09:28.000000 AIRPALibrary-1.0.2/src/AIRPALibrary/AIRPALibrary.py
--rw-rw-rw-   0        0        0       38 2023-03-13 07:41:23.000000 AIRPALibrary-1.0.2/src/AIRPALibrary/__init__.py
--rw-rw-rw-   0        0        0     1267 2023-03-15 02:37:59.000000 AIRPALibrary-1.0.2/src/AIRPALibrary/function_timeout.py
--rw-rw-rw-   0        0        0     1613 2023-03-18 15:19:28.000000 AIRPALibrary-1.0.2/src/AIRPALibrary/function_timeout_robot.py
-drwxrwxrwx   0        0        0        0 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/src/AIRPALibrary.egg-info/
--rw-rw-rw-   0        0        0      299 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/src/AIRPALibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/src/AIRPALibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/src/AIRPALibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-29 03:11:27.000000 AIRPALibrary-1.0.2/src/AIRPALibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/
+-rw-rw-rw-   0        0        0      299 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      637 2023-03-13 07:36:18.000000 AIRPALibrary-1.0.3/README.md
+-rw-rw-rw-   0        0        0      529 2023-05-10 03:43:07.000000 AIRPALibrary-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/src/AIRPALibrary/
+-rw-rw-rw-   0        0        0     8281 2023-05-10 03:42:44.000000 AIRPALibrary-1.0.3/src/AIRPALibrary/AIRPALibrary.py
+-rw-rw-rw-   0        0        0       38 2023-03-13 07:41:23.000000 AIRPALibrary-1.0.3/src/AIRPALibrary/__init__.py
+-rw-rw-rw-   0        0        0     1267 2023-03-15 02:37:59.000000 AIRPALibrary-1.0.3/src/AIRPALibrary/function_timeout.py
+-rw-rw-rw-   0        0        0     1613 2023-03-18 15:19:28.000000 AIRPALibrary-1.0.3/src/AIRPALibrary/function_timeout_robot.py
+drwxrwxrwx   0        0        0        0 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/src/AIRPALibrary.egg-info/
+-rw-rw-rw-   0        0        0      299 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/src/AIRPALibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/src/AIRPALibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/src/AIRPALibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-10 04:15:50.000000 AIRPALibrary-1.0.3/src/AIRPALibrary.egg-info/top_level.txt
```

### Comparing `AIRPALibrary-1.0.2/README.md` & `AIRPALibrary-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `AIRPALibrary-1.0.2/pyproject.toml` & `AIRPALibrary-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AIRPALibrary"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="IT Dev HOTD Python Developer"},
 ]
 description = "RPA Package for AI"
 requires-python = ">=3.7"
 dependencies = []
 classifiers = [
```

### Comparing `AIRPALibrary-1.0.2/src/AIRPALibrary/AIRPALibrary.py` & `AIRPALibrary-1.0.3/src/AIRPALibrary/AIRPALibrary.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         
         if bool(value.strip()[-5:].decode('utf-8'))==True:
             raise RuntimeError('The execution failed because of time exceeded')
         else :
             print('Execution sucessfully initiated')
             
     
-    def send_email(self, subject=None, content=None, to=None, cc=None, file_path=None):
+    def send_email(self, subject=None, content=None, to=None, cc=None, file_path=None, sender=None):
         ''' Fungsi untuk mengirimkan email dengan parameter input sebagai berikut ini :\n
             subject = (string) masukkan subject yang anda inginkan, contoh : RPA Email\n
             content = (string) masukkan content email atau isi dari email. content email bisa juga dengan menggunakan html layouting\n
             Untuk masukkan data receiver email baik to maupun cc bisa tunggal(string or list) atau banyak(list). Contoh adalah sebagai berikut : \n
             tunggal :
                 to = 'example@contoh.com'   atau    to = ['example@contoh.com']\n
                 cc = 'example@contoh.com'   atau    cc = ['example@contoh.com']
@@ -146,17 +146,18 @@
                 'to':';'.join(to),
                 'subject': subject,
                 'content': content}
         
         if cc!=None:
             if isinstance(cc, list)==False : cc = [cc]
             payload['cc'] = ';'.join(str(c) for c in cc)
+            
+        if sender!=None:
+            payload['from'] = sender
         
-        print(payload)
-
         headers = {
             'X-Client-Code':cli_code
         } 
         
         try:
             if file_path!=None:
                 files = {}
```

### Comparing `AIRPALibrary-1.0.2/src/AIRPALibrary/function_timeout.py` & `AIRPALibrary-1.0.3/src/AIRPALibrary/function_timeout.py`

 * *Files identical despite different names*

### Comparing `AIRPALibrary-1.0.2/src/AIRPALibrary/function_timeout_robot.py` & `AIRPALibrary-1.0.3/src/AIRPALibrary/function_timeout_robot.py`

 * *Files identical despite different names*

