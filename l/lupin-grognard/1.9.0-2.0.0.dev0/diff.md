# Comparing `tmp/lupin-grognard-1.9.0.tar.gz` & `tmp/lupin-grognard-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lupin-grognard-1.9.0.tar", last modified: Wed Apr 19 07:44:20 2023, max compression
+gzip compressed data, was "lupin-grognard-2.0.0.dev0.tar", last modified: Wed May 10 10:17:57 2023, max compression
```

## Comparing `lupin-grognard-1.9.0.tar` & `lupin-grognard-2.0.0.dev0.tar`

### file list

```diff
@@ -1,46 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.575191 lupin-grognard-1.9.0/
--rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-1.9.0/LICENCE
--rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0      508 2023-04-19 07:44:20.576193 lupin-grognard-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.493409 lupin-grognard-1.9.0/lupin_grognard/
--rw-rw-rw-   0        0        0       23 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard/__init__.py
--rw-rw-rw-   0        0        0       79 2022-12-05 21:58:40.000000 lupin-grognard-1.9.0/lupin_grognard/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.517953 lupin-grognard-1.9.0/lupin_grognard/core/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/lupin_grognard/core/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-03-30 22:12:23.000000 lupin-grognard-1.9.0/lupin_grognard/core/check.py
--rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-1.9.0/lupin_grognard/core/cmd.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.522952 lupin-grognard-1.9.0/lupin_grognard/core/commit/
--rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/__init__.py
--rw-rw-rw-   0        0        0     7379 2023-03-31 14:48:46.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit.py
--rw-rw-rw-   0        0        0     1037 2023-02-07 15:57:39.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_error.py
--rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_reporter.py
--rw-rw-rw-   0        0        0     5739 2023-04-06 08:21:25.000000 lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_validator.py
--rw-rw-rw-   0        0        0     1319 2023-04-06 08:19:58.000000 lupin-grognard-1.9.0/lupin_grognard/core/config.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.526457 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/
--rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/__init__.py
--rw-rw-rw-   0        0        0    11845 2023-03-28 14:31:51.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/changelog.py
--rw-rw-rw-   0        0        0     1472 2023-03-17 11:16:03.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/jinja_generator.py
--rw-rw-rw-   0        0        0     4958 2023-03-30 13:35:56.000000 lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/reviewlog.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.528466 lupin-grognard-1.9.0/lupin_grognard/core/format/
--rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/__init__.py
--rw-rw-rw-   0        0        0     2709 2023-03-26 23:00:29.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/clang_format.py
--rw-rw-rw-   0        0        0     2598 2023-03-02 22:35:36.000000 lupin-grognard-1.9.0/lupin_grognard/core/format/cmake_format.py
--rw-rw-rw-   0        0        0     4040 2023-03-31 14:48:27.000000 lupin-grognard-1.9.0/lupin_grognard/core/git.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.530464 lupin-grognard-1.9.0/lupin_grognard/core/tools/
--rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/lupin_grognard/core/tools/__init__.py
--rw-rw-rw-   0        0        0     4128 2023-03-31 10:47:54.000000 lupin-grognard-1.9.0/lupin_grognard/core/tools/utils.py
--rw-rw-rw-   0        0        0     5854 2023-03-31 13:35:54.000000 lupin-grognard-1.9.0/lupin_grognard/run.py
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.575191 lupin-grognard-1.9.0/lupin_grognard/templates/
--rw-rw-rw-   0        0        0     1848 2023-03-28 13:46:34.000000 lupin-grognard-1.9.0/lupin_grognard/templates/changelog.j2
--rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-1.9.0/lupin_grognard/templates/reviewlog.j2
-drwxrwxrwx   0        0        0        0 2023-04-19 07:44:20.512439 lupin-grognard-1.9.0/lupin_grognard.egg-info/
--rw-rw-rw-   0        0        0      508 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1215 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      133 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-19 07:44:20.000000 lupin-grognard-1.9.0/lupin_grognard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      933 2023-04-19 07:44:20.577191 lupin-grognard-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.968841 lupin-grognard-2.0.0.dev0/
+-rw-rw-rw-   0        0        0     1091 2022-10-26 14:21:00.000000 lupin-grognard-2.0.0.dev0/LICENCE
+-rw-rw-rw-   0        0        0       36 2023-03-02 22:35:36.000000 lupin-grognard-2.0.0.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0      513 2023-05-10 10:17:57.968841 lupin-grognard-2.0.0.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-01-20 08:07:36.000000 lupin-grognard-2.0.0.dev0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.924955 lupin-grognard-2.0.0.dev0/lupin_grognard/
+-rw-rw-rw-   0        0        0       28 2023-05-10 10:17:57.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/__init__.py
+-rw-rw-rw-   0        0        0       77 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.949487 lupin-grognard-2.0.0.dev0/lupin_grognard/core/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/__init__.py
+-rw-rw-rw-   0        0        0     2183 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/check.py
+-rw-rw-rw-   0        0        0      912 2022-12-09 16:33:58.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/cmd.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.953546 lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/
+-rw-rw-rw-   0        0        0        0 2023-01-17 13:04:34.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/__init__.py
+-rw-rw-rw-   0        0        0     7379 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/commit.py
+-rw-rw-rw-   0        0        0     1037 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/commit_error.py
+-rw-rw-rw-   0        0        0     1816 2023-03-17 09:49:38.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/commit_reporter.py
+-rw-rw-rw-   0        0        0     5739 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/commit_validator.py
+-rw-rw-rw-   0        0        0     1319 2023-05-10 10:16:15.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/config.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.958543 lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/
+-rw-rw-rw-   0        0        0        0 2023-03-17 11:16:03.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/__init__.py
+-rw-rw-rw-   0        0        0    11923 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/changelog.py
+-rw-rw-rw-   0        0        0     1706 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/jinja_generator.py
+-rw-rw-rw-   0        0        0     5017 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/reviewlog.py
+-rw-rw-rw-   0        0        0     1625 2023-05-10 10:00:16.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/ros2_docs.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.960543 lupin-grognard-2.0.0.dev0/lupin_grognard/core/format/
+-rw-rw-rw-   0        0        0        0 2023-02-10 13:59:49.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/format/__init__.py
+-rw-rw-rw-   0        0        0     2709 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/format/clang_format.py
+-rw-rw-rw-   0        0        0     2598 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/format/cmake_format.py
+-rw-rw-rw-   0        0        0     4040 2023-03-31 14:48:27.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/git.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.961841 lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/
+-rw-rw-rw-   0        0        0        0 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.965842 lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/ros2/
+-rw-rw-rw-   0        0        0        0 2023-05-05 22:45:05.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/ros2/__init__.py
+-rw-rw-rw-   0        0        0     2654 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/ros2/interfaces.py
+-rw-rw-rw-   0        0        0     2265 2023-05-10 10:10:04.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/ros2/package.py
+-rw-rw-rw-   0        0        0    35591 2023-05-10 10:14:40.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/ros2/parser.py
+-rw-rw-rw-   0        0        0     4128 2023-03-31 10:47:54.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/utils.py
+-rw-rw-rw-   0        0        0     6314 2023-05-10 10:03:25.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/run.py
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.967842 lupin-grognard-2.0.0.dev0/lupin_grognard/templates/
+-rw-rw-rw-   0        0        0     1848 2023-05-04 13:34:03.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/templates/changelog.j2
+-rw-rw-rw-   0        0        0     3390 2023-03-24 10:41:51.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/templates/reviewlog.j2
+-rw-rw-rw-   0        0        0      438 2023-05-09 21:16:03.000000 lupin-grognard-2.0.0.dev0/lupin_grognard/templates/rosapi.j2
+drwxrwxrwx   0        0        0        0 2023-05-10 10:17:57.943485 lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/
+-rw-rw-rw-   0        0        0      513 2023-05-10 10:17:57.000000 lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1468 2023-05-10 10:17:57.000000 lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 10:17:57.000000 lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-10 10:17:57.000000 lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-11-23 21:32:45.000000 lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      133 2023-05-10 10:17:57.000000 lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 10:17:57.000000 lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      938 2023-05-10 10:17:57.974043 lupin-grognard-2.0.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0      171 2022-11-28 17:09:18.000000 lupin-grognard-2.0.0.dev0/setup.py
```

### Comparing `lupin-grognard-1.9.0/LICENCE` & `lupin-grognard-2.0.0.dev0/LICENCE`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/check.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/check.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 from typing import List
 
 from lupin_grognard.core.commit.commit import Commit
-from lupin_grognard.core.commit.commit_validator import CommitValidator
 from lupin_grognard.core.commit.commit_error import ErrorCount
+from lupin_grognard.core.commit.commit_validator import CommitValidator
 from lupin_grognard.core.config import MAJOR_COMMIT_TYPES
 
 
 def check_max_allowed_major_commits(
     commits_string: List[str], major_commit_limit: int
 ) -> bool:
     """Check if the number of major commits in `commits_string` exceeds `major_commit_limit`.
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/cmd.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/cmd.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/commit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from datetime import datetime
-from typing import Dict, List, Union, Tuple
+from typing import Dict, List, Tuple, Union
 
-from lupin_grognard.core.config import PATTERN, INITIAL_COMMIT
+from lupin_grognard.core.config import INITIAL_COMMIT, PATTERN
 from lupin_grognard.core.git import Git
 
 
 class Commit:
     def __init__(self, commit: str):
         self.commit = commit
         self.associated_closed_issue = None
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_error.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/commit_error.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from lupin_grognard.core.config import (
-    SUCCESS,
-    FAILED,
-    TITLE_FAILED,
     BODY_FAILED,
+    FAILED,
     MERGE_FAILED,
+    SUCCESS,
+    TITLE_FAILED,
 )
 
 
 class ErrorCount:
     def __init__(self):
         self.body_error = 0
         self.title_error = 0
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_reporter.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/commit_reporter.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/commit/commit_validator.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/commit/commit_validator.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/config.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/config.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/changelog.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/changelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import Any, Dict, List, Union
 
 from lupin_grognard.core.commit.commit import Commit
 from lupin_grognard.core.doc_generator.jinja_generator import JinjaGenerator
 from lupin_grognard.core.git import Git
 from lupin_grognard.core.tools.utils import info
 
@@ -12,24 +13,27 @@
         self.git = Git()
 
     def generate(self) -> None:
         """Generate changelog"""
         project_details = self._get_project_details()
         classified_commits = self._classify_commits()
         self._generate_file(
+            path=os.getcwd(),
             file_name="CHANGELOG",
             file_extension=".md",
             context={
                 "version_details": classified_commits,
                 "project_details": project_details,
             },
         )
 
-    def _generate_file(self, file_name: str, file_extension: str, context={}) -> None:
-        return super()._generate_file(file_name, file_extension, context)
+    def _generate_file(
+        self, path: str, file_name: str, file_extension: str, context: Dict
+    ) -> None:
+        return super()._generate_file(path, file_name, file_extension, context)
 
     def _get_project_details(self) -> Dict[str, Union[str, int]]:
         project_url = self.git.get_remote_origin_url()
         project_name = project_url.split("/")[-1]
         info(msg=f"Collecting data from {project_name}")
         branch_name = self.git.get_branch_name()
         commit_count = self._count_commits()
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/jinja_generator.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/jinja_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from jinja2 import (
     Environment,
     PackageLoader,
-    select_autoescape,
     Template,
-    TemplateNotFound,
     TemplateError,
+    TemplateNotFound,
     TemplateRuntimeError,
+    select_autoescape,
 )
 
 from lupin_grognard.core.tools.utils import die, info, write_file
 
 
 class JinjaGenerator:
     def __init__(self, *args):
@@ -23,16 +23,22 @@
                 trim_blocks=True,  # Removes unnecessary spaces before and after blocks and loop
                 lstrip_blocks=True,  # Removes unnecessary spaces before blocks and loop
             )
             return env.get_template(template_name)
         except TemplateNotFound:
             die(msg=f"Template 'lupin_grognard/templates/{template_name}' not found")
 
-    def _generate_file(self, file_name: str, file_extension: str, context={}) -> None:
-        info(msg=f"Generating {file_name}{file_extension} file")
+    def _generate_file(
+        self, path: str, file_name: str, file_extension: str, context={}
+    ) -> None:
         template = self._get_local_template(template_name=f"{file_name}.j2")
         try:
             content = template.render(context)
         except (TemplateError, TemplateRuntimeError) as e:
             die(msg=f"Error rendering Jinja2 template: {e}")
-        write_file(file=f"{file_name}{file_extension}", content=content)
+        if not path:
+            info(msg=f"Generating {file_name}{file_extension} file")
+            write_file(file=f"{file_name}{file_extension}", content=content)
+        else:
+            info(msg=f"Generating {path}/{file_name}{file_extension} file")
+            write_file(file=f"{path}/{file_name}{file_extension}", content=content)
         info(msg="File generated")
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/doc_generator/reviewlog.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/doc_generator/reviewlog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,44 @@
+import os
 import unicodedata
 from typing import Dict, List
 
 from lupin_grognard.core.commit.commit import Commit
-from lupin_grognard.core.tools.utils import info
 from lupin_grognard.core.doc_generator.jinja_generator import JinjaGenerator
 from lupin_grognard.core.git import Git
+from lupin_grognard.core.tools.utils import info
 
 
 class Reviewlog(JinjaGenerator):
     def __init__(self, commits: List[Commit]):
         self.commits = commits
         self.git = Git()
 
     def generate(self):
         project_url = self.git.get_remote_origin_url()
         project_name = project_url.split("/")[-1]
         info(msg=f"Collecting approvers report from {project_name}")
         approvers_report = self._get_approvers_report()
         approvers_participants = self._get_approvers_participants(approvers_report)
         self._generate_file(
+            path=os.getcwd(),
             file_name="REVIEWLOG",
             file_extension=".html",
             context={
                 "approvers_report": approvers_report,
                 "project_name": project_name,
                 "project_url": project_url,
                 "participants": approvers_participants,
             },
         )
 
     def _generate_file(
-        self, file_name: str, file_extension: str, context: Dict
+        self, path: str, file_name: str, file_extension: str, context: Dict
     ) -> None:
-        return super()._generate_file(file_name, file_extension, context)
+        return super()._generate_file(path, file_name, file_extension, context)
 
     def _normalize_string(self, string: str) -> str:
         return (
             unicodedata.normalize("NFD", string)
             .encode("ascii", "ignore")
             .decode("utf-8")
         )
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/format/clang_format.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/format/clang_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 import subprocess
 from typing import List, Optional
 
-from lupin_grognard.core.tools.utils import die, warn, info, check_if_file_exists
+from lupin_grognard.core.tools.utils import check_if_file_exists, die, info, warn
 
 
 class ClangFormatter:
     def __init__(self, name) -> None:
         self.name = name
 
     def format_c_cpp_files(self) -> None:
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/format/cmake_format.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/format/cmake_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import shutil
 import subprocess
 from typing import List
 
-from lupin_grognard.core.tools.utils import die, info, warn, check_if_file_exists
+from lupin_grognard.core.tools.utils import check_if_file_exists, die, info, warn
 
 
 class CMakeFormatter:
     def format_cmake_files(self) -> None:
         if not self._check_cmake_format_tool():
             die(
                 msg="could not find CMake-Format, install it from https://github.com/cheshirekow/cmake_format"
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/git.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/git.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/core/tools/utils.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/core/tools/utils.py`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/run.py` & `lupin-grognard-2.0.0.dev0/lupin_grognard/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 from typing import Optional
 
-from dotenv import load_dotenv
 import typer
+from dotenv import load_dotenv
 
 from lupin_grognard.__init__ import __version__
-from lupin_grognard.core.check import (
-    check_commit,
-    check_max_allowed_major_commits,
-)
+from lupin_grognard.core.check import check_commit, check_max_allowed_major_commits
 from lupin_grognard.core.commit.commit import Commit
 from lupin_grognard.core.doc_generator.changelog import Changelog
 from lupin_grognard.core.doc_generator.reviewlog import Reviewlog
+from lupin_grognard.core.doc_generator.ros2_docs import Ros2Docs
 from lupin_grognard.core.format.clang_format import ClangFormatter
 from lupin_grognard.core.format.cmake_format import CMakeFormatter
 from lupin_grognard.core.git import Git
+from lupin_grognard.core.tools.ros2.package import find_ros_packages
+
 from .core.tools.utils import (
     configure_logging,
     create_branch_list,
+    die,
     display_current_branch_name,
     display_number_of_commits_to_check,
     display_supported_commit_types,
     generate_commit_list,
     generate_commits_range_to_check,
-    die,
 )
 
 load_dotenv()
 GROG_BRANCHES = os.getenv("GROG_BRANCHES")
 GROG_MAX_ALLOWED_COMMITS = os.getenv("GROG_MAX_ALLOWED_COMMITS")
 GROG_DONT_CHECK_FOR_APPROVERS = os.getenv("GROG_DONT_CHECK_FOR_APPROVERS")
 GROG_CLANG_FORMAT = os.getenv("GROG_CLANG_FORMAT")
@@ -158,7 +158,20 @@
     configure_logging()
     git_log = Git().get_log()
     if git_log.stderr:
         die(f"git error {git_log.return_code}, {git_log.stderr}")
     commit_list = generate_commit_list(data=git_log.stdout)
     commits = Commit.add_additional_commit_info(commit_list=commit_list)
     Reviewlog(commits=commits).generate()
+
+
+@cli.command()
+def ros2docs(
+    path: str = typer.Option(..., "--path", "-p", help="path to ROS2 workspace")
+):
+    """Generate ROS2 documentation"""
+    configure_logging()
+
+    ros_packages = find_ros_packages(path)
+    for path in ros_packages:
+        api_doc = Ros2Docs(path=path)
+        api_doc.generate_api_docs()
```

### Comparing `lupin-grognard-1.9.0/lupin_grognard/templates/changelog.j2` & `lupin-grognard-2.0.0.dev0/lupin_grognard/templates/changelog.j2`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard/templates/reviewlog.j2` & `lupin-grognard-2.0.0.dev0/lupin_grognard/templates/reviewlog.j2`

 * *Files identical despite different names*

### Comparing `lupin-grognard-1.9.0/lupin_grognard.egg-info/SOURCES.txt` & `lupin-grognard-2.0.0.dev0/lupin_grognard.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 lupin_grognard/core/commit/commit_error.py
 lupin_grognard/core/commit/commit_reporter.py
 lupin_grognard/core/commit/commit_validator.py
 lupin_grognard/core/doc_generator/__init__.py
 lupin_grognard/core/doc_generator/changelog.py
 lupin_grognard/core/doc_generator/jinja_generator.py
 lupin_grognard/core/doc_generator/reviewlog.py
+lupin_grognard/core/doc_generator/ros2_docs.py
 lupin_grognard/core/format/__init__.py
 lupin_grognard/core/format/clang_format.py
 lupin_grognard/core/format/cmake_format.py
 lupin_grognard/core/tools/__init__.py
 lupin_grognard/core/tools/utils.py
+lupin_grognard/core/tools/ros2/__init__.py
+lupin_grognard/core/tools/ros2/interfaces.py
+lupin_grognard/core/tools/ros2/package.py
+lupin_grognard/core/tools/ros2/parser.py
 lupin_grognard/templates/changelog.j2
-lupin_grognard/templates/reviewlog.j2
+lupin_grognard/templates/reviewlog.j2
+lupin_grognard/templates/rosapi.j2
```

### Comparing `lupin-grognard-1.9.0/setup.cfg` & `lupin-grognard-2.0.0.dev0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7570 696e 2d67 726f 676e 6172   = lupin-grognar
-00000020: 640d 0a76 6572 7369 6f6e 203d 2031 2e39  d..version = 1.9
-00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
-00000040: 3d20 4c75 7069 6e20 6c69 6e74 6572 2074  = Lupin linter t
-00000050: 6f6f 6c0d 0a6c 6f6e 675f 6465 7363 7269  ool..long_descri
-00000060: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-00000070: 4144 4d45 2e6d 640d 0a6b 6579 776f 7264  ADME.md..keyword
-00000080: 7320 3d20 636c 692c 206c 696e 7465 720d  s = cli, linter.
-00000090: 0a6c 6963 656e 7365 203d 204d 4954 204c  .license = MIT L
-000000a0: 6963 656e 7365 0d0a 636c 6173 7369 6669  icense..classifi
-000000b0: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000000c0: 6d65 6e74 2053 7461 7475 7320 3a3a 2033  ment Status :: 3
-000000d0: 202d 2041 6c70 6861 0d0a 0949 6e74 656e   - Alpha...Inten
-000000e0: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-000000f0: 496e 666f 726d 6174 696f 6e20 5465 6368  Information Tech
-00000100: 6e6f 6c6f 6779 0d0a 0954 6f70 6963 203a  nology...Topic :
-00000110: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000120: 6f70 6d65 6e74 203a 3a20 5175 616c 6974  opment :: Qualit
-00000130: 7920 4173 7375 7261 6e63 650d 0a09 5072  y Assurance...Pr
-00000140: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000150: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000160: 332e 3130 0d0a 094c 6963 656e 7365 203a  3.10...License :
-00000170: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000180: 3a20 4d49 5420 4c69 6365 6e73 650d 0a0d  : MIT License...
-00000190: 0a5b 6f70 7469 6f6e 735d 0d0a 7a69 705f  .[options]..zip_
-000001a0: 7361 6665 203d 2046 616c 7365 0d0a 696e  safe = False..in
-000001b0: 636c 7564 655f 7061 636b 6167 655f 6461  clude_package_da
-000001c0: 7461 203d 2054 7275 650d 0a70 6163 6b61  ta = True..packa
-000001d0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-000001e0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000001f0: 3d33 2e31 300d 0a69 6e73 7461 6c6c 5f72  =3.10..install_r
-00000200: 6571 7569 7265 7320 3d20 0d0a 0974 7970  equires = ...typ
-00000210: 6572 5b61 6c6c 5d3d 3d30 2e36 2e31 0d0a  er[all]==0.6.1..
-00000220: 0970 7974 686f 6e2d 646f 7465 6e76 3d3d  .python-dotenv==
-00000230: 302e 3231 2e30 0d0a 0965 6d6f 6a69 3d3d  0.21.0...emoji==
-00000240: 322e 322e 300d 0a09 4a69 6e6a 6132 3d3d  2.2.0...Jinja2==
-00000250: 332e 312e 320d 0a09 636d 616b 656c 616e  3.1.2...cmakelan
-00000260: 673d 3d30 2e36 2e31 330d 0a09 5079 5941  g==0.6.13...PyYA
-00000270: 4d4c 3d3d 362e 300d 0a0d 0a5b 6f70 7469  ML==6.0....[opti
-00000280: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
-00000290: 7265 5d0d 0a74 6573 7420 3d20 0d0a 0970  re]..test = ...p
-000002a0: 7974 6573 743d 3d37 2e31 2e33 0d0a 0966  ytest==7.1.3...f
-000002b0: 6c61 6b65 383d 3d35 2e30 2e34 0d0a 0d0a  lake8==5.0.4....
-000002c0: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-000002d0: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-000002e0: 7363 7269 7074 7320 3d20 0d0a 0967 726f  scripts = ...gro
-000002f0: 6720 3d20 6c75 7069 6e5f 6772 6f67 6e61  g = lupin_grogna
-00000300: 7264 2e72 756e 3a63 6c69 0d0a 0d0a 5b6f  rd.run:cli....[o
-00000310: 7074 696f 6e73 2e70 6163 6b61 6765 5f64  ptions.package_d
-00000320: 6174 615d 0d0a 2a20 3d20 2a2e 636c 616e  ata]..* = *.clan
-00000330: 672d 666f 726d 6174 0d0a 0d0a 5b6f 7074  g-format....[opt
-00000340: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-00000350: 6e64 5d0d 0a65 7863 6c75 6465 203d 200d  nd]..exclude = .
-00000360: 0a09 6c75 7069 6e5f 6772 6f67 6e61 7264  ..lupin_grognard
-00000370: 2e74 6573 7473 2a0d 0a0d 0a5b 6567 675f  .tests*....[egg_
-00000380: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000390: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-000003a0: 300d 0a0d 0a                             0....
+00000020: 640d 0a76 6572 7369 6f6e 203d 2032 2e30  d..version = 2.0
+00000030: 2e30 2e64 6576 300d 0a64 6573 6372 6970  .0.dev0..descrip
+00000040: 7469 6f6e 203d 204c 7570 696e 206c 696e  tion = Lupin lin
+00000050: 7465 7220 746f 6f6c 0d0a 6c6f 6e67 5f64  ter tool..long_d
+00000060: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
+00000070: 653a 2052 4541 444d 452e 6d64 0d0a 6b65  e: README.md..ke
+00000080: 7977 6f72 6473 203d 2063 6c69 2c20 6c69  ywords = cli, li
+00000090: 6e74 6572 0d0a 6c69 6365 6e73 6520 3d20  nter..license = 
+000000a0: 4d49 5420 4c69 6365 6e73 650d 0a63 6c61  MIT License..cla
+000000b0: 7373 6966 6965 7273 203d 200d 0a09 4465  ssifiers = ...De
+000000c0: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
+000000d0: 203a 3a20 3320 2d20 416c 7068 610d 0a09   :: 3 - Alpha...
+000000e0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+000000f0: 6520 3a3a 2049 6e66 6f72 6d61 7469 6f6e  e :: Information
+00000100: 2054 6563 686e 6f6c 6f67 790d 0a09 546f   Technology...To
+00000110: 7069 6320 3a3a 2053 6f66 7477 6172 6520  pic :: Software 
+00000120: 4465 7665 6c6f 706d 656e 7420 3a3a 2051  Development :: Q
+00000130: 7561 6c69 7479 2041 7373 7572 616e 6365  uality Assurance
+00000140: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000150: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000160: 6e20 3a3a 2033 2e31 300d 0a09 4c69 6365  n :: 3.10...Lice
+00000170: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000180: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000190: 7365 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  se....[options].
+000001a0: 0a7a 6970 5f73 6166 6520 3d20 4661 6c73  .zip_safe = Fals
+000001b0: 650d 0a69 6e63 6c75 6465 5f70 6163 6b61  e..include_packa
+000001c0: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
+000001d0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+000001e0: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+000001f0: 7320 3d20 3e3d 332e 3130 0d0a 696e 7374  s = >=3.10..inst
+00000200: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
+00000210: 0a09 7479 7065 725b 616c 6c5d 3d3d 302e  ..typer[all]==0.
+00000220: 362e 310d 0a09 7079 7468 6f6e 2d64 6f74  6.1...python-dot
+00000230: 656e 763d 3d30 2e32 312e 300d 0a09 656d  env==0.21.0...em
+00000240: 6f6a 693d 3d32 2e32 2e30 0d0a 094a 696e  oji==2.2.0...Jin
+00000250: 6a61 323d 3d33 2e31 2e32 0d0a 0963 6d61  ja2==3.1.2...cma
+00000260: 6b65 6c61 6e67 3d3d 302e 362e 3133 0d0a  kelang==0.6.13..
+00000270: 0950 7959 414d 4c3d 3d36 2e30 0d0a 0d0a  .PyYAML==6.0....
+00000280: 5b6f 7074 696f 6e73 2e65 7874 7261 735f  [options.extras_
+00000290: 7265 7175 6972 655d 0d0a 7465 7374 203d  require]..test =
+000002a0: 200d 0a09 7079 7465 7374 3d3d 372e 312e   ...pytest==7.1.
+000002b0: 330d 0a09 666c 616b 6538 3d3d 352e 302e  3...flake8==5.0.
+000002c0: 340d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  4....[options.en
+000002d0: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
+000002e0: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
+000002f0: 0a09 6772 6f67 203d 206c 7570 696e 5f67  ..grog = lupin_g
+00000300: 726f 676e 6172 642e 7275 6e3a 636c 690d  rognard.run:cli.
+00000310: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000320: 6167 655f 6461 7461 5d0d 0a2a 203d 202a  age_data]..* = *
+00000330: 2e63 6c61 6e67 2d66 6f72 6d61 740d 0a0d  .clang-format...
+00000340: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000350: 6573 2e66 696e 645d 0d0a 6578 636c 7564  es.find]..exclud
+00000360: 6520 3d20 0d0a 096c 7570 696e 5f67 726f  e = ...lupin_gro
+00000370: 676e 6172 642e 7465 7374 732a 0d0a 0d0a  gnard.tests*....
+00000380: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000390: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000003a0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

