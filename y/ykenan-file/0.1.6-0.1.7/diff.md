# Comparing `tmp/ykenan_file-0.1.6.tar.gz` & `tmp/ykenan_file-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.1.6.tar", last modified: Sun Apr 30 11:46:14 2023, max compression
+gzip compressed data, was "ykenan_file-0.1.7.tar", last modified: Wed May 10 07:25:39 2023, max compression
```

## Comparing `ykenan_file-0.1.6.tar` & `ykenan_file-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 11:46:14.686725 ykenan_file-0.1.6/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      829 2023-04-30 11:46:14.685723 ykenan_file-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.6/README.md
--rw-rw-rw-   0        0        0      676 2023-04-30 11:45:23.000000 ykenan_file-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 11:46:14.686725 ykenan_file-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-30 11:46:14.662724 ykenan_file-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-30 11:46:14.674723 ykenan_file-0.1.6/src/ykenan_file/
--rw-rw-rw-   0        0        0    23874 2023-04-30 11:45:10.000000 ykenan_file-0.1.6/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.6/src/ykenan_file/util.py
-drwxrwxrwx   0        0        0        0 2023-04-30 11:46:14.683723 ykenan_file-0.1.6/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      829 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-30 11:46:14.000000 ykenan_file-0.1.6/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 07:25:39.428038 ykenan_file-0.1.7/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      829 2023-05-10 07:25:39.427040 ykenan_file-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-04-21 09:34:27.000000 ykenan_file-0.1.7/README.md
+-rw-rw-rw-   0        0        0      676 2023-05-10 07:24:54.000000 ykenan_file-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       32 2023-03-22 07:40:08.000000 ykenan_file-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 07:25:39.428038 ykenan_file-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 07:25:39.411038 ykenan_file-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 07:25:39.415037 ykenan_file-0.1.7/src/ykenan_file/
+-rw-rw-rw-   0        0        0    23488 2023-05-10 07:24:54.000000 ykenan_file-0.1.7/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0      157 2023-04-06 01:49:10.000000 ykenan_file-0.1.7/src/ykenan_file/util.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:25:39.426037 ykenan_file-0.1.7/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      829 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-10 07:25:39.000000 ykenan_file-0.1.7/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.1.6/LICENSE` & `ykenan_file-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.1.6/PKG-INFO` & `ykenan_file-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.1.6
+Version: 0.1.7
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_file-0.1.6/pyproject.toml` & `ykenan_file-0.1.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.1.6/src/ykenan_file/__init__.py` & `ykenan_file-0.1.7/src/ykenan_file/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 # -*- coding: UTF-8 -*-
 
-import itertools
 import os
 
 import pandas as pd
 from ykenan_log import Logger
 from pandas import DataFrame
 
 '''
@@ -21,15 +20,15 @@
 
     def __init__(self, sep='\t',
                  line_terminator="\n",
                  encoding: str = 'utf_8_sig',
                  index: bool = False,
                  header: bool = True,
                  sheet_name='new_sheet',
-                 log_file: str = "ykenan_file",
+                 log_file: str = "YKenan_file",
                  is_form_log_file: bool = True):
         """
         Initialization creation information, public information
         :param sep: File Separator
         :param line_terminator: File Line Break
         :param encoding: Document code
         :param index: Whether there is a row index
@@ -358,20 +357,20 @@
         """
         file_content = self.read_file(*files)
         self.log.debug(f"Start merging files {files} ...")
         pd_concat = pd.concat(file_content, join=join, ignore_index=True)
         pd.DataFrame(pd_concat).to_csv(output_file, encoding=encoding, sep=self.sep, index=index)
 
 
-class staticMethod:
+class StaticMethod:
     """
     文件或者路径的静态方法
     """
 
-    def __init__(self, log_file: str = "ykenan_file", is_form_log_file: bool = True):
+    def __init__(self, log_file: str = "YKenan_file", is_form_log_file: bool = True):
         """
         :param log_file: Path to form a log file
         :param is_form_log_file: Is a log file formed
         """
         self.log = Logger(name="YKenan file", log_path=log_file, is_form_file=is_form_log_file)
 
     def read_file_line(self, path: str, mode: str = 'r', encoding: str = "utf-8") -> list:
@@ -567,36 +566,28 @@
         dict_: dict = {}
         with os.scandir(path) as it:
             for entry in it:
                 entry: os.DirEntry
                 # 判断是否满足情况
                 if suffix is None or entry.name.endswith(suffix):
                     if type_ == 0:
-                        dict_ = dict(itertools.chain(dict_.items(), {
-                            entry.name: entry.path
-                        }.items()))
                         contents.append(entry.name)
+                        dict_.update({entry.name: entry.path})
                     elif type_ == 1:
                         # 此处判断不能和 type_ == 1 连写，因为需要进行提示 ValueError("type input error, type is 0 or 1 or 2.")
                         if entry.is_file():
-                            dict_ = dict(itertools.chain(dict_.items(), {
-                                entry.name: entry.path
-                            }.items()))
                             files.append(entry.name)
+                            dict_.update({entry.name: entry.path})
                     elif type_ == 2:
                         if entry.is_dir():
-                            dict_ = dict(itertools.chain(dict_.items(), {
-                                entry.name: entry.path
-                            }.items()))
                             dirs.append(entry.name)
+                            dict_.update({entry.name: entry.path})
                     else:
                         raise ValueError("type input error, type is 0 or 1 or 2.")
-        dict_ = dict(itertools.chain(dict_.items(), {
-            "name": contents if type_ == 0 else files if type_ == 1 else dirs
-        }.items()))
+        dict_.update({"name": contents if type_ == 0 else files if type_ == 1 else dirs})
         return dict_
 
     def entry_files_dict(self, path: str) -> dict:
         """
         Obtain all files in the specified path
         :param path: path
         :return: files
```

### Comparing `ykenan_file-0.1.6/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.1.7/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.1.6
+Version: 0.1.7
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

