# Comparing `tmp/threadsafe_shell-1.4.0.tar.gz` & `tmp/threadsafe_shell-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadsafe_shell-1.4.0.tar", last modified: Wed May 10 00:33:43 2023, max compression
+gzip compressed data, was "threadsafe_shell-1.5.0.tar", last modified: Wed May 10 00:46:37 2023, max compression
```

## Comparing `threadsafe_shell-1.4.0.tar` & `threadsafe_shell-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-10 00:33:43.418482 threadsafe_shell-1.4.0/
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)     1071 2022-11-05 20:17:37.000000 threadsafe_shell-1.4.0/LICENSE
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-10 00:33:43.418482 threadsafe_shell-1.4.0/PKG-INFO
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       88 2022-11-05 20:23:15.000000 threadsafe_shell-1.4.0/README.md
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      565 2023-05-10 00:33:10.000000 threadsafe_shell-1.4.0/pyproject.toml
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       38 2023-05-10 00:33:43.418482 threadsafe_shell-1.4.0/setup.cfg
-drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-10 00:33:43.418482 threadsafe_shell-1.4.0/threadsafe_shell.egg-info/
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-10 00:33:43.000000 threadsafe_shell-1.4.0/threadsafe_shell.egg-info/PKG-INFO
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)      212 2023-05-10 00:33:43.000000 threadsafe_shell-1.4.0/threadsafe_shell.egg-info/SOURCES.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)        1 2023-05-10 00:33:43.000000 threadsafe_shell-1.4.0/threadsafe_shell.egg-info/dependency_links.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)       17 2023-05-10 00:33:43.000000 threadsafe_shell-1.4.0/threadsafe_shell.egg-info/top_level.txt
--rw-r--r--   0 kalamari  (1000) kalamari  (1001)     6478 2023-05-10 00:33:30.000000 threadsafe_shell-1.4.0/threadsafe_shell.py
+drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-10 00:46:37.406461 threadsafe_shell-1.5.0/
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)     1071 2022-11-05 20:17:37.000000 threadsafe_shell-1.5.0/LICENSE
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-10 00:46:37.406461 threadsafe_shell-1.5.0/PKG-INFO
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       88 2022-11-05 20:23:15.000000 threadsafe_shell-1.5.0/README.md
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      565 2023-05-10 00:46:32.000000 threadsafe_shell-1.5.0/pyproject.toml
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       38 2023-05-10 00:46:37.406461 threadsafe_shell-1.5.0/setup.cfg
+drwxr-xr-x   0 kalamari  (1000) kalamari  (1001)        0 2023-05-10 00:46:37.406461 threadsafe_shell-1.5.0/threadsafe_shell.egg-info/
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      668 2023-05-10 00:46:37.000000 threadsafe_shell-1.5.0/threadsafe_shell.egg-info/PKG-INFO
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)      212 2023-05-10 00:46:37.000000 threadsafe_shell-1.5.0/threadsafe_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)        1 2023-05-10 00:46:37.000000 threadsafe_shell-1.5.0/threadsafe_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)       17 2023-05-10 00:46:37.000000 threadsafe_shell-1.5.0/threadsafe_shell.egg-info/top_level.txt
+-rw-r--r--   0 kalamari  (1000) kalamari  (1001)     6354 2023-05-10 00:46:15.000000 threadsafe_shell-1.5.0/threadsafe_shell.py
```

### Comparing `threadsafe_shell-1.4.0/LICENSE` & `threadsafe_shell-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threadsafe_shell-1.4.0/PKG-INFO` & `threadsafe_shell-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsafe_shell
-Version: 1.4.0
+Version: 1.5.0
 Summary: A pure-python, thread-safe, queue-based logging and user input module
 Author-email: Calico Kalamari <kalamariking@proton.me>
 Project-URL: Homepage, https://github.com/KalamariKing/threadsafe-shell
 Project-URL: Bug Tracker, https://github.com/KalamariKing/threadsafe-shell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `threadsafe_shell-1.4.0/pyproject.toml` & `threadsafe_shell-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "threadsafe_shell"
-version = "1.4.0"
+version = "1.5.0"
 authors = [
   { name="Calico Kalamari", email="kalamariking@proton.me" },
 ]
 description = "A pure-python, thread-safe, queue-based logging and user input module"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `threadsafe_shell-1.4.0/threadsafe_shell.egg-info/PKG-INFO` & `threadsafe_shell-1.5.0/threadsafe_shell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadsafe-shell
-Version: 1.4.0
+Version: 1.5.0
 Summary: A pure-python, thread-safe, queue-based logging and user input module
 Author-email: Calico Kalamari <kalamariking@proton.me>
 Project-URL: Homepage, https://github.com/KalamariKing/threadsafe-shell
 Project-URL: Bug Tracker, https://github.com/KalamariKing/threadsafe-shell/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `threadsafe_shell-1.4.0/threadsafe_shell.py` & `threadsafe_shell-1.5.0/threadsafe_shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,43 +113,43 @@
     def ask(self, string: str, default:str=None) -> str:
         """
         Asks the user a question and returns the answer.
         If `default` is `None`, will ask again until an answer is given. Otherwise, when no answer is given, returns `default`.
         """
         string += "\033[35mPROMPT "+string+"\033[0m "
         with self.__input_lock:
-            self.__add_to_queue("\033[35mPROMPT ", string, end='', console_only=True)
+            self.__add_to_queue("\033[35mPROMPT ", string, end='')
             val = input().strip()
             while default is None and len(val) == 0:
-                self.__add_to_queue("\033[35mPROMPT ", string, end='', console_only=True)
+                self.__add_to_queue("\033[35mPROMPT ", string, end='')
                 val = input().strip()
-        if not (self.__log_file is None): self.__add_to_queue("\033[35mPROMPT ", string, val, file_only=True, sep='')
+        if not (self.__log_file is None): self.__add_to_queue("\033[35mPROMPT ", string, val, sep='')
         return default if val=="" else val
 
 
     def prompt(self, string: str, default: bool = None) -> bool:
         """
         Prompts a yes-or-no question and returns the boolean answer.
         kwarg `default` controls `'Y|n'` (`True`) or `'y|N'` (`False`), or if to ask infinitely (`None`).
         """
         if default is None:
             val = ""
             string += " (y|n)  "
             with self.__input_lock:
                 while len(val)==0 or not (val[0] in "ynYN"):
-                    self.__add_to_queue("\033[35mPROMPT ", string, end='', console_only=True)
+                    self.__add_to_queue("\033[35mPROMPT ", string, end='')
                     val = input().strip()
-            if not (self.__log_file is None): self.__add_to_queue("\033[35mPROMPT ", string, val, file_only=True, sep='')
+            if not (self.__log_file is None): self.__add_to_queue("\033[35mPROMPT ", string, val, sep='')
             return val[0].lower() == "y"
         else:
             string += f" ({'Y|n' if default else 'y|N'})  "
             with self.__input_lock:
-                self.__add_to_queue("\033[35mPROMPT ", string, end='', console_only=True)
+                self.__add_to_queue("\033[35mPROMPT ", string, end='')
                 val = input().strip()
-            if not (self.__log_file is None): self.__add_to_queue("\033[35mPROMPT ", string, val, file_only=True, sep='')
+            if not (self.__log_file is None): self.__add_to_queue("\033[35mPROMPT ", string, val, sep='')
             if len(val)==0 or val[0] not in "ynYN":
                 val = "y" if default else "n"
             if default: return val[0].lower() != "n"
             else:       return val[0].lower() == "y"
 
 
 def get_shell() -> Shell:
```

