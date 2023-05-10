# Comparing `tmp/sample-git-diffs-0.2.5.tar.gz` & `tmp/sample-git-diffs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample-git-diffs-0.2.5.tar", max compression
+gzip compressed data, was "sample-git-diffs-0.3.0.tar", max compression
```

## Comparing `sample-git-diffs-0.2.5.tar` & `sample-git-diffs-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      594 2023-05-10 12:18:37.061714 sample-git-diffs-0.2.5/README.md
--rw-r--r--   0        0        0      478 2023-05-10 12:19:42.467066 sample-git-diffs-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-16 14:02:59.160040 sample-git-diffs-0.2.5/sample_git_diffs/__init__.py
--rw-r--r--   0        0        0     2748 2023-01-16 15:12:27.387354 sample-git-diffs-0.2.5/sample_git_diffs/sample_git_diffs.py
--rw-r--r--   0        0        0     1386 2023-05-10 12:19:56.477429 sample-git-diffs-0.2.5/setup.py
--rw-r--r--   0        0        0     1189 2023-05-10 12:19:56.477583 sample-git-diffs-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      594 2023-05-10 12:18:37.061714 sample-git-diffs-0.3.0/README.md
+-rw-r--r--   0        0        0      523 2023-05-10 12:56:41.321425 sample-git-diffs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-16 14:02:59.160040 sample-git-diffs-0.3.0/sample_git_diffs/__init__.py
+-rw-r--r--   0        0        0     2748 2023-01-16 15:12:27.387354 sample-git-diffs-0.3.0/sample_git_diffs/sample_git_diffs.py
+-rw-r--r--   0        0        0     1818 2023-05-10 12:54:09.583903 sample-git-diffs-0.3.0/sample_git_diffs/to_md.py
+-rw-r--r--   0        0        0     1453 2023-05-10 12:56:51.966426 sample-git-diffs-0.3.0/setup.py
+-rw-r--r--   0        0        0     1189 2023-05-10 12:56:51.966778 sample-git-diffs-0.3.0/PKG-INFO
```

### Comparing `sample-git-diffs-0.2.5/README.md` & `sample-git-diffs-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sample-git-diffs-0.2.5/sample_git_diffs/sample_git_diffs.py` & `sample-git-diffs-0.3.0/sample_git_diffs/sample_git_diffs.py`

 * *Files identical despite different names*

### Comparing `sample-git-diffs-0.2.5/setup.py` & `sample-git-diffs-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pandas']
 
 entry_points = \
-{'console_scripts': ['sample-git-diffs = '
+{'console_scripts': ['diff2markdown = sample_git_diffs.to_md:cli',
+                     'sample-git-diffs = '
                      'sample_git_diffs.sample_git_diffs:cli']}
 
 setup_kwargs = {
     'name': 'sample-git-diffs',
-    'version': '0.2.5',
+    'version': '0.3.0',
     'description': '',
     'long_description': '# sample-git-diffs\n\n```\nSample git diffs uniformly wrt. number of changes per file. The output is formatted as a .diff file.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --n N                 Total number of diffs to be sampled\n  --diffstat DIFFSTAT   Custom git diff command for the sampling probabilities\n  --diffcommand DIFFCOMMAND\n                        Custom git diff command for the actual diff\n```\n\nFor example, if you want to draw a sample of 25 diffs from the folder data/, you run\n\n```\nsample-git-diffs --diffstat "git diff --stat data/" --n 25\n```',
     'author': 'ninpnin',
     'author_email': 'you@example.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ninpnin/sample-git-diffs',
```

### Comparing `sample-git-diffs-0.2.5/PKG-INFO` & `sample-git-diffs-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sample-git-diffs
-Version: 0.2.5
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/ninpnin/sample-git-diffs
 License: MIT
 Author: ninpnin
 Author-email: you@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

