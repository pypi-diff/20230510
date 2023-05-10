# Comparing `tmp/pyutils_basstal-0.4.2.tar.gz` & `tmp/pyutils_basstal-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutils_basstal-0.4.2.tar", last modified: Sat May  6 09:08:10 2023, max compression
+gzip compressed data, was "pyutils_basstal-0.4.3.tar", last modified: Wed May 10 06:00:38 2023, max compression
```

## Comparing `pyutils_basstal-0.4.2.tar` & `pyutils_basstal-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 09:08:10.764166 pyutils_basstal-0.4.2/
--rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1473 2023-05-06 09:08:10.763168 pyutils_basstal-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      609 2022-12-30 10:22:58.000000 pyutils_basstal-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 09:08:10.745216 pyutils_basstal-0.4.2/pyutils/
--rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.2/pyutils/__init__.py
--rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.2/pyutils/autoupgrade.py
--rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.2/pyutils/executor.py
--rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.2/pyutils/fsext.py
--rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.2/pyutils/shorthand.py
--rw-rw-rw-   0        0        0     5159 2023-05-06 09:04:36.000000 pyutils_basstal-0.4.2/pyutils/simplelogger.py
--rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.2/pyutils/templite.py
-drwxrwxrwx   0        0        0        0 2023-05-06 09:08:10.763168 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/
--rw-rw-rw-   0        0        0     1473 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 09:08:10.000000 pyutils_basstal-0.4.2/pyutils_basstal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 09:08:10.764166 pyutils_basstal-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     8820 2023-05-06 09:07:56.000000 pyutils_basstal-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:00:38.776602 pyutils_basstal-0.4.3/
+-rw-rw-rw-   0        0        0     1100 2022-06-01 03:28:45.000000 pyutils_basstal-0.4.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1473 2023-05-10 06:00:38.775604 pyutils_basstal-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-05-10 05:03:43.000000 pyutils_basstal-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 06:00:38.755658 pyutils_basstal-0.4.3/pyutils/
+-rw-rw-rw-   0        0        0       69 2022-07-14 05:30:09.000000 pyutils_basstal-0.4.3/pyutils/__init__.py
+-rw-rw-rw-   0        0        0     6438 2023-04-25 07:11:32.000000 pyutils_basstal-0.4.3/pyutils/autoupgrade.py
+-rw-rw-rw-   0        0        0    24035 2023-04-24 09:26:17.000000 pyutils_basstal-0.4.3/pyutils/executor.py
+-rw-rw-rw-   0        0        0    16192 2023-04-24 09:44:47.000000 pyutils_basstal-0.4.3/pyutils/fsext.py
+-rw-rw-rw-   0        0        0      658 2022-11-11 09:12:56.000000 pyutils_basstal-0.4.3/pyutils/shorthand.py
+-rw-rw-rw-   0        0        0     6209 2023-05-10 05:59:40.000000 pyutils_basstal-0.4.3/pyutils/simplelogger.py
+-rw-rw-rw-   0        0        0     5397 2023-04-24 09:27:14.000000 pyutils_basstal-0.4.3/pyutils/templite.py
+drwxrwxrwx   0        0        0        0 2023-05-10 06:00:38.775604 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/
+-rw-rw-rw-   0        0        0     1473 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 06:00:38.000000 pyutils_basstal-0.4.3/pyutils_basstal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 06:00:38.776602 pyutils_basstal-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     8847 2023-05-10 05:35:50.000000 pyutils_basstal-0.4.3/setup.py
```

### Comparing `pyutils_basstal-0.4.2/LICENSE.txt` & `pyutils_basstal-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.2/PKG-INFO` & `pyutils_basstal-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutils_basstal
-Version: 0.4.2
+Version: 0.4.3
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.4.2/README.md` & `pyutils_basstal-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.2/pyutils/autoupgrade.py` & `pyutils_basstal-0.4.3/pyutils/autoupgrade.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.2/pyutils/executor.py` & `pyutils_basstal-0.4.3/pyutils/executor.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.2/pyutils/fsext.py` & `pyutils_basstal-0.4.3/pyutils/fsext.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.2/pyutils/shorthand.py` & `pyutils_basstal-0.4.3/pyutils/shorthand.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.2/pyutils/simplelogger.py` & `pyutils_basstal-0.4.3/pyutils/simplelogger.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # ruff: noqa: E501
 
 import os
 import logging
 import pyutils.shorthand as shd
 import sys
+import re
+from colorama import Fore, Style
 
 ######################
 ######################
 #       Log          #
 ######################
 ######################
 
@@ -30,31 +32,44 @@
     _info_logger.addHandler(logging.StreamHandler(sys.stdout))
     _info_logger.propagate = False
 
     __hanlder_cache = {}
 
     @staticmethod
     def _color_message(message, color_code, bold=False):
-        if shd.is_win():
-            os.system('')
-        bold_code = '\033[1m' if bold else ''
-        return f'{bold_code}\033[{color_code}m{message}\033[0m'
+        os.system('')
+        # Map color_code to actual color
+        color_map = {
+            '31': Fore.RED,
+            '32': Fore.GREEN,
+            '33': Fore.YELLOW,
+            '34': Fore.BLUE,
+            '35': Fore.MAGENTA,
+            '36': Fore.CYAN,
+            '37': Fore.WHITE
+        }
+        color = color_map.get(str(color_code), Fore.RESET)
+
+        if bold:
+            return f'{Style.BRIGHT}{color}{message}{Style.RESET_ALL}'
+        else:
+            return f'{color}{message}{Style.RESET_ALL}'
 
     @staticmethod
     def _preprocess_message(message: str):
         if not shd.is_win():
             message = message.replace('=>', '➜').replace('<=', '✔')
 
-        if message.endswith('\r\n') or message.endswith('\n'):
-            message = message.rstrip()
-        return message
+        return message.rstrip('\r\n')
 
     @staticmethod
-    def info(message, _):
+    def info(message, bold=False, color_code=None):
         message = SimpleLogger._preprocess_message(message)
+        if color_code is not None or bold is not False:
+            message = SimpleLogger._color_message(message, color_code, bold)
         SimpleLogger._info_logger.info(message)
 
     @staticmethod
     def warning(message, bold=False):
         message = SimpleLogger._preprocess_message(message)
         message = SimpleLogger._color_message(message, 33, bold)
         SimpleLogger._info_logger.warning(message)
@@ -68,34 +83,47 @@
         SimpleLogger._logger.error(message)
 
     @staticmethod
     def addFileHandler(file_path):
         if file_path in SimpleLogger.__hanlder_cache:
             return
         file_handler = logging.FileHandler(file_path)
+
+        class NoEscapeSeqFormatter(logging.Formatter):
+            _ansi_escape = re.compile(r'(\x9B|\x1B\[)[0-?]*[ -/]*[@-~]')
+
+            def format(self, record):
+                record.msg = self._ansi_escape.sub('', record.getMessage())
+                return super().format(record)
+
+        file_handler.setFormatter(NoEscapeSeqFormatter('%(asctime)s - %(levelname)s - %(message)s', datefmt='%H:%M:%S'))
         SimpleLogger.__hanlder_cache[file_path] = file_handler
         SimpleLogger._logger.addHandler(file_handler)
         SimpleLogger._info_logger.addHandler(file_handler)
 
     @staticmethod
     def removeFileHander(file_path):
+        SimpleLogger.removeFileHandler(file_path)
+
+    @staticmethod
+    def removeFileHandler(file_path):
         if file_path in SimpleLogger.__hanlder_cache:
             return
         file_handler = SimpleLogger.__hanlder_cache[file_path]
         SimpleLogger._logger.removeHandler(file_handler)
         SimpleLogger._info_logger.removeHandler(file_handler)
         file_handler.close()
         del SimpleLogger.__hanlder_cache[file_path]
 
 
 logger = SimpleLogger._logger
 
 
-def info(message, bold=False):
-    SimpleLogger.info(message, bold)
+def info(message, bold=False, color_code=None):
+    SimpleLogger.info(message, bold, color_code)
 
 
 def warning(message, bold=False):
     SimpleLogger.warning(message, bold)
 
 
 def error(message, bold=False):
```

### Comparing `pyutils_basstal-0.4.2/pyutils/templite.py` & `pyutils_basstal-0.4.3/pyutils/templite.py`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.2/pyutils_basstal.egg-info/PKG-INFO` & `pyutils_basstal-0.4.3/pyutils_basstal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutils-basstal
-Version: 0.4.2
+Version: 0.4.3
 Summary: self used py utils
 Home-page: https://github.com/basstal/pyutils
 Author: basstal
 Author-email: 330475004@qq.com
 License: UNKNOWN
 Keywords: utils,development
 Platform: UNKNOWN
```

### Comparing `pyutils_basstal-0.4.2/pyutils_basstal.egg-info/SOURCES.txt` & `pyutils_basstal-0.4.3/pyutils_basstal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyutils_basstal-0.4.2/setup.py` & `pyutils_basstal-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="pyutils_basstal",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.4.2",  # Required
+    version="0.4.3",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="self used py utils",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -128,15 +128,17 @@
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=[
         "charade",
         "semantic_version",
         "beautifulsoup4",
         "deprecated",
-        "pyyaml"],  # Optional
+        "pyyaml",
+        "colorama"
+    ],  # Optional
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
```

