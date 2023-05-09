# Comparing `tmp/anastasia_logging-1.0.0.tar.gz` & `tmp/anastasia_logging-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anastasia_logging-1.0.0.tar", max compression
+gzip compressed data, was "anastasia_logging-1.1.0.tar", max compression
```

## Comparing `anastasia_logging-1.0.0.tar` & `anastasia_logging-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     5060 2023-05-09 20:36:45.058591 anastasia_logging-1.0.0/README.md
--rw-r--r--   0        0        0     5497 2023-05-09 20:30:52.179481 anastasia_logging-1.0.0/anastasia_logging/__init__.py
--rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.0.0/anastasia_logging/codes/__init__.py
--rw-r--r--   0        0        0      879 2023-05-09 16:53:34.979124 anastasia_logging-1.0.0/anastasia_logging/codes/standard.py
--rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.0.0/anastasia_logging/codes/standard_errors.py
--rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.0.0/anastasia_logging/codes/standard_info.py
--rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.0.0/anastasia_logging/codes/standard_warning.py
--rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.0.0/anastasia_logging/env/__init__.py
--rw-r--r--   0        0        0      553 2023-05-09 20:13:45.495205 anastasia_logging-1.0.0/anastasia_logging/env/env_variables.py
--rw-r--r--   0        0        0    10259 2023-05-09 20:16:26.872345 anastasia_logging-1.0.0/anastasia_logging/logger.py
--rw-r--r--   0        0        0      285 2023-05-09 20:32:20.208251 anastasia_logging-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5503 1970-01-01 00:00:00.000000 anastasia_logging-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5178 2023-05-09 22:05:50.063920 anastasia_logging-1.1.0/README.md
+-rw-r--r--   0        0        0     7637 2023-05-09 22:00:04.916726 anastasia_logging-1.1.0/anastasia_logging/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-09 14:56:24.294304 anastasia_logging-1.1.0/anastasia_logging/codes/__init__.py
+-rw-r--r--   0        0        0      879 2023-05-09 16:53:34.979124 anastasia_logging-1.1.0/anastasia_logging/codes/standard.py
+-rw-r--r--   0        0        0       92 2023-05-08 16:28:55.501019 anastasia_logging-1.1.0/anastasia_logging/codes/standard_errors.py
+-rw-r--r--   0        0        0       55 2023-05-08 16:28:55.505019 anastasia_logging-1.1.0/anastasia_logging/codes/standard_info.py
+-rw-r--r--   0        0        0      118 2023-05-08 16:28:55.505019 anastasia_logging-1.1.0/anastasia_logging/codes/standard_warning.py
+-rw-r--r--   0        0        0       47 2023-05-09 20:12:08.106577 anastasia_logging-1.1.0/anastasia_logging/env/__init__.py
+-rw-r--r--   0        0        0      553 2023-05-09 20:13:45.495205 anastasia_logging-1.1.0/anastasia_logging/env/env_variables.py
+-rw-r--r--   0        0        0    10259 2023-05-09 20:16:26.872345 anastasia_logging-1.1.0/anastasia_logging/logger.py
+-rw-r--r--   0        0        0      285 2023-05-09 22:03:42.910744 anastasia_logging-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5621 1970-01-01 00:00:00.000000 anastasia_logging-1.1.0/PKG-INFO
```

### Comparing `anastasia_logging-1.0.0/README.md` & `anastasia_logging-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,20 @@
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] WARNING: <W100> I am a dataset warning
 ```
 
 If a code is already predefined and no message is introduced, a default message will appear according to code declared.
 
 ## **3. Versioning** ##
 
+### v1.1.0 ###
+
+* Features:
+
+    * Function basicConfig equivalent from logging implemented for root AnastasiaLogger
+
 ### v1.0.0 ###
 
 * Features:
 
     * Anastasia *Logger* Class abstraction
     * Standar code description definitions for INFO, WARNING and ERROR
     * Predefined AnastasiaLogger parameters loaded from environment variables
```

### Comparing `anastasia_logging-1.0.0/anastasia_logging/__init__.py` & `anastasia_logging-1.1.0/anastasia_logging/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,17 +24,85 @@
 ```
 
 """
 
 from typing import Optional
 from .logger import AnastasiaLogger
 
+CRITICAL = 50
+FATAL = CRITICAL
+ERROR = 40
+WARNING = 30
+WARN = WARNING
+INFO = 20
+DEBUG = 10
+NOTSET = 0
+
 # Equivalent to RootLogger from logging but doesn't override it
 anastasia_logger = AnastasiaLogger()
 
+def basicConfig(filename: str=None, filemode: str = None, format: str=None, datefmt: str=None, level: int=None, handlers=None, **kwargs) -> None:
+    """
+    Do basic configuration for Anastasia logging system, similar to logging base root function.
+
+    Attributes
+    ----------
+
+    filename : Optional[str]
+        Specifies that a FileHandler be created, using the specified filename, rather than a StreamHandler.
+
+    filemode : Optional[str]
+        Specifies the mode to open the file, if filename is specified (if filemode is unspecified, it defaults to 'a').
+
+    format : Optional[str]
+        Use the specified format string for the handler.
+
+    datefmt : Optional[str]
+        Use the specified date/time format.
+
+    level : Optional[str]
+        Set the root logger level to the specified level.
+
+    handlers : Iterable[Handlers]
+        If specified, this should be an iterable of already created handlers, which will be added to the root handler.
+        Any handler in the list which does not have a formatter assigned will be assigned the formatter created in this function.
+
+    """
+    from logging import Formatter, FileHandler, StreamHandler
+
+    if isinstance(filemode, type(None)):
+        filemode = 'a'
+    if isinstance(format, type(None)):
+        format = anastasia_logger.formatter._fmt
+    if isinstance(datefmt, type(None)):
+        datefmt = anastasia_logger.formatter.datefmt
+    if isinstance(level, type(None)):
+        level = anastasia_logger.level
+    if isinstance(handlers, type(None)):
+        handlers = []
+
+    while anastasia_logger.hasHandlers():
+        anastasia_logger.removeHandler(anastasia_logger.handlers[0])
+    
+    fmt = Formatter(format, datefmt)
+    anastasia_logger.setLevel(level)
+
+    if not handlers:
+        if filename:
+            h = FileHandler(filename, filemode)
+        else:
+            h = StreamHandler()
+        handlers = [h]
+
+    for h in handlers:
+        if h.formatter is None:
+            h.setFormatter(fmt)
+        anastasia_logger.addHandler(h)
+    
+
 def override_logging(based_on: Optional[AnastasiaLogger] = None) -> None:
     """
     Modify base root logging with Anastasia logging format
 
     Attributes
     ----------
```

### Comparing `anastasia_logging-1.0.0/anastasia_logging/codes/standard.py` & `anastasia_logging-1.1.0/anastasia_logging/codes/standard.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.0.0/anastasia_logging/env/env_variables.py` & `anastasia_logging-1.1.0/anastasia_logging/env/env_variables.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.0.0/anastasia_logging/logger.py` & `anastasia_logging-1.1.0/anastasia_logging/logger.py`

 * *Files identical despite different names*

### Comparing `anastasia_logging-1.0.0/PKG-INFO` & `anastasia_logging-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anastasia-logging
-Version: 1.0.0
+Version: 1.1.0
 Summary: Anastasia Logging Standarization
 Author: anastasiaai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -123,14 +123,20 @@
 OUTPUT => 2023-05-08 11:55:27 UTC/GMT-0400 | [ANASTASIA-JOB] WARNING: <W100> I am a dataset warning
 ```
 
 If a code is already predefined and no message is introduced, a default message will appear according to code declared.
 
 ## **3. Versioning** ##
 
+### v1.1.0 ###
+
+* Features:
+
+    * Function basicConfig equivalent from logging implemented for root AnastasiaLogger
+
 ### v1.0.0 ###
 
 * Features:
 
     * Anastasia *Logger* Class abstraction
     * Standar code description definitions for INFO, WARNING and ERROR
     * Predefined AnastasiaLogger parameters loaded from environment variables
```

