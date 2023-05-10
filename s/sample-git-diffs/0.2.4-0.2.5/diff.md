# Comparing `tmp/sample-git-diffs-0.2.4.tar.gz` & `tmp/sample-git-diffs-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample-git-diffs-0.2.4.tar", max compression
+gzip compressed data, was "sample-git-diffs-0.2.5.tar", max compression
```

## Comparing `sample-git-diffs-0.2.4.tar` & `sample-git-diffs-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      441 2023-01-16 14:40:19.027075 sample-git-diffs-0.2.4/README.md
--rw-r--r--   0        0        0      478 2023-05-08 10:00:22.968024 sample-git-diffs-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-16 14:02:59.160040 sample-git-diffs-0.2.4/sample_git_diffs/__init__.py
--rw-r--r--   0        0        0     2748 2023-01-16 15:12:27.387354 sample-git-diffs-0.2.4/sample_git_diffs/sample_git_diffs.py
--rw-r--r--   0        0        0     1228 2023-05-08 10:00:27.534187 sample-git-diffs-0.2.4/setup.py
--rw-r--r--   0        0        0     1036 2023-05-08 10:00:27.534374 sample-git-diffs-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      594 2023-05-10 12:18:37.061714 sample-git-diffs-0.2.5/README.md
+-rw-r--r--   0        0        0      478 2023-05-10 12:19:42.467066 sample-git-diffs-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-16 14:02:59.160040 sample-git-diffs-0.2.5/sample_git_diffs/__init__.py
+-rw-r--r--   0        0        0     2748 2023-01-16 15:12:27.387354 sample-git-diffs-0.2.5/sample_git_diffs/sample_git_diffs.py
+-rw-r--r--   0        0        0     1386 2023-05-10 12:19:56.477429 sample-git-diffs-0.2.5/setup.py
+-rw-r--r--   0        0        0     1189 2023-05-10 12:19:56.477583 sample-git-diffs-0.2.5/PKG-INFO
```

### Comparing `sample-git-diffs-0.2.4/sample_git_diffs/sample_git_diffs.py` & `sample-git-diffs-0.2.5/sample_git_diffs/sample_git_diffs.py`

 * *Files identical despite different names*

### Comparing `sample-git-diffs-0.2.4/setup.py` & `sample-git-diffs-0.2.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 entry_points = \
 {'console_scripts': ['sample-git-diffs = '
                      'sample_git_diffs.sample_git_diffs:cli']}
 
 setup_kwargs = {
     'name': 'sample-git-diffs',
-    'version': '0.2.4',
+    'version': '0.2.5',
     'description': '',
-    'long_description': '# sample-git-diffs\n\n```\nSample git diffs uniformly wrt. number of changes per file. The output is formatted as a .diff file.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --n N                 Total number of diffs to be sampled\n  --diffstat DIFFSTAT   Custom git diff command for the sampling probabilities\n  --diffcommand DIFFCOMMAND\n                        Custom git diff command for the actual diff\n```\n',
+    'long_description': '# sample-git-diffs\n\n```\nSample git diffs uniformly wrt. number of changes per file. The output is formatted as a .diff file.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --n N                 Total number of diffs to be sampled\n  --diffstat DIFFSTAT   Custom git diff command for the sampling probabilities\n  --diffcommand DIFFCOMMAND\n                        Custom git diff command for the actual diff\n```\n\nFor example, if you want to draw a sample of 25 diffs from the folder data/, you run\n\n```\nsample-git-diffs --diffstat "git diff --stat data/" --n 25\n```',
     'author': 'ninpnin',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ninpnin/sample-git-diffs',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `sample-git-diffs-0.2.4/PKG-INFO` & `sample-git-diffs-0.2.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-git-diffs
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Home-page: https://github.com/ninpnin/sample-git-diffs
 License: MIT
 Author: ninpnin
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,7 +25,12 @@
   -h, --help            show this help message and exit
   --n N                 Total number of diffs to be sampled
   --diffstat DIFFSTAT   Custom git diff command for the sampling probabilities
   --diffcommand DIFFCOMMAND
                         Custom git diff command for the actual diff
 ```
 
+For example, if you want to draw a sample of 25 diffs from the folder data/, you run
+
+```
+sample-git-diffs --diffstat "git diff --stat data/" --n 25
+```
```

