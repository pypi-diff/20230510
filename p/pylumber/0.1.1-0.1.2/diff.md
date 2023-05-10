# Comparing `tmp/pylumber-0.1.1.tar.gz` & `tmp/pylumber-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylumber-0.1.1.tar", last modified: Thu Apr 20 23:48:49 2023, max compression
+gzip compressed data, was "pylumber-0.1.2.tar", last modified: Wed May 10 18:32:49 2023, max compression
```

## Comparing `pylumber-0.1.1.tar` & `pylumber-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-04-20 23:48:49.101161 pylumber-0.1.1/
--rw-r--r--   0 thryang    (501) staff       (20)     1065 2023-03-14 19:30:15.000000 pylumber-0.1.1/LICENSE
--rw-r--r--   0 thryang    (501) staff       (20)      535 2023-04-20 23:48:49.101055 pylumber-0.1.1/PKG-INFO
--rw-r--r--   0 thryang    (501) staff       (20)      103 2023-03-14 19:30:15.000000 pylumber-0.1.1/README.md
-drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-04-20 23:48:49.100308 pylumber-0.1.1/pylumber/
--rw-r--r--   0 thryang    (501) staff       (20)     2966 2023-04-20 23:17:25.000000 pylumber-0.1.1/pylumber/__init__.py
--rw-r--r--   0 thryang    (501) staff       (20)       37 2023-04-10 22:49:31.000000 pylumber-0.1.1/pylumber/format.py
-drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-04-20 23:48:49.100891 pylumber-0.1.1/pylumber.egg-info/
--rw-r--r--   0 thryang    (501) staff       (20)      535 2023-04-20 23:48:49.000000 pylumber-0.1.1/pylumber.egg-info/PKG-INFO
--rw-r--r--   0 thryang    (501) staff       (20)      194 2023-04-20 23:48:49.000000 pylumber-0.1.1/pylumber.egg-info/SOURCES.txt
--rw-r--r--   0 thryang    (501) staff       (20)        1 2023-04-20 23:48:49.000000 pylumber-0.1.1/pylumber.egg-info/dependency_links.txt
--rw-r--r--   0 thryang    (501) staff       (20)        9 2023-04-20 23:48:49.000000 pylumber-0.1.1/pylumber.egg-info/top_level.txt
--rw-r--r--   0 thryang    (501) staff       (20)       38 2023-04-20 23:48:49.101192 pylumber-0.1.1/setup.cfg
--rw-r--r--   0 thryang    (501) staff       (20)      775 2023-04-20 23:48:35.000000 pylumber-0.1.1/setup.py
+drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-05-10 18:32:49.806551 pylumber-0.1.2/
+-rw-r--r--   0 thryang    (501) staff       (20)     1065 2023-03-14 19:30:15.000000 pylumber-0.1.2/LICENSE
+-rw-r--r--   0 thryang    (501) staff       (20)      601 2023-05-10 18:32:49.806428 pylumber-0.1.2/PKG-INFO
+-rw-r--r--   0 thryang    (501) staff       (20)      103 2023-03-14 19:30:15.000000 pylumber-0.1.2/README.md
+drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-05-10 18:32:49.805807 pylumber-0.1.2/pylumber/
+-rw-r--r--   0 thryang    (501) staff       (20)     3038 2023-05-10 18:31:47.000000 pylumber-0.1.2/pylumber/__init__.py
+-rw-r--r--   0 thryang    (501) staff       (20)       37 2023-04-10 22:49:31.000000 pylumber-0.1.2/pylumber/format.py
+drwxr-xr-x   0 thryang    (501) staff       (20)        0 2023-05-10 18:32:49.806267 pylumber-0.1.2/pylumber.egg-info/
+-rw-r--r--   0 thryang    (501) staff       (20)      601 2023-05-10 18:32:49.000000 pylumber-0.1.2/pylumber.egg-info/PKG-INFO
+-rw-r--r--   0 thryang    (501) staff       (20)      194 2023-05-10 18:32:49.000000 pylumber-0.1.2/pylumber.egg-info/SOURCES.txt
+-rw-r--r--   0 thryang    (501) staff       (20)        1 2023-05-10 18:32:49.000000 pylumber-0.1.2/pylumber.egg-info/dependency_links.txt
+-rw-r--r--   0 thryang    (501) staff       (20)        9 2023-05-10 18:32:49.000000 pylumber-0.1.2/pylumber.egg-info/top_level.txt
+-rw-r--r--   0 thryang    (501) staff       (20)       38 2023-05-10 18:32:49.806592 pylumber-0.1.2/setup.cfg
+-rw-r--r--   0 thryang    (501) staff       (20)      841 2023-05-10 18:32:41.000000 pylumber-0.1.2/setup.py
```

### Comparing `pylumber-0.1.1/LICENSE` & `pylumber-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylumber-0.1.1/PKG-INFO` & `pylumber-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pylumber
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lumberjack for your Code, Logs, Prints, Errors and more.
 Author: Tim Yang (TimMUP)
 Author-email: thryang@outlook.com
 Keywords: python,logging,debugging,lumberjack
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
-pyLumber is a Python library for logging and debugging. It is designed to be simple and easy to use.
+pyLumber is a Python library for logging and debugging. It is designed to be simple and easy to use, while being user friendly to those who are in a business setting.
```

### Comparing `pylumber-0.1.1/pylumber/__init__.py` & `pylumber-0.1.2/pylumber/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,26 +60,29 @@
 # Helper Function (Library Use) | Removes all ANSI Codes from String
 def STRIP_ANSI(string):
     return re.sub(r'\033\[[0-9;]*m', '', string)
 
 
 # Helper Function (User Use) | Formats string with 
 class lumberjack:
-    def __init__(self, logFile=None, logParameter: list = CONST.DEFAULT_LOG_PARAM, logPrint=False):
+    def __init__(self, logFile=None, logParameter: list = CONST.DEFAULT_LOG_PARAM, silent=False):
         self.logFile = open(logFile, "w") if logFile else None
         self.DICT = {}
+        self.SILENT = silent
         for i in range(len(logParameter)):
             logPrefix = f"{logParameter[i][1]}[{logParameter[i][0].center(CONST.PREFIX_SPACE, CONST.PREFIX_CHAR)}]{ANSI_MODI.END}"
             self.DICT[i] = (logPrefix, logParameter[i][1])                          # (Prefix w/ Formatting, ANSI Formatting) 
-            self.DICT[logParameter[i][0]] = (logPrefix, logParameter[i][1])         # (Additional Key for Prefix Input)
+            self.DICT[logParameter[i][0]] = (logPrefix, logParameter[i][1])
+                     # (Additional Key for Prefix Input)
     
     def logWriter(self, msg):
         if self.logFile:
             self.logFile.write(STRIP_ANSI(msg + "\n"))
 
     def log(self, msg: str, logLevel = "OK"):
         modiMsg = f"{self.DICT[logLevel][0]} {msg}{ANSI_MODI.END}"
         self.logWriter(modiMsg)
-        print(modiMsg)
+        if not self.SILENT:
+            print(modiMsg)
     
     def format(self, msg: str, logLevel = "OK"):
         return f"{self.DICT[logLevel][1]}{msg}{ANSI_MODI.END}"
```

### Comparing `pylumber-0.1.1/pylumber.egg-info/PKG-INFO` & `pylumber-0.1.2/pylumber.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pylumber
-Version: 0.1.1
+Version: 0.1.2
 Summary: Lumberjack for your Code, Logs, Prints, Errors and more.
 Author: Tim Yang (TimMUP)
 Author-email: thryang@outlook.com
 Keywords: python,logging,debugging,lumberjack
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE
 
-pyLumber is a Python library for logging and debugging. It is designed to be simple and easy to use.
+pyLumber is a Python library for logging and debugging. It is designed to be simple and easy to use, while being user friendly to those who are in a business setting.
```

### Comparing `pylumber-0.1.1/setup.py` & `pylumber-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Lumberjack for your Code, Logs, Prints, Errors and more.'
-LONG_DESCRIPTION = 'pyLumber is a Python library for logging and debugging. It is designed to be simple and easy to use.'
+LONG_DESCRIPTION = 'pyLumber is a Python library for logging and debugging. It is designed to be simple and easy to use, while being user friendly to those who are in a business setting.'
 
 setup(
     name="pylumber",
     version=VERSION,
     author="Tim Yang (TimMUP)",
     author_email="thryang@outlook.com",
     description=DESCRIPTION,
```

