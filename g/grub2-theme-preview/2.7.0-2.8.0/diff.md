# Comparing `tmp/grub2-theme-preview-2.7.0.tar.gz` & `tmp/grub2-theme-preview-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grub2-theme-preview-2.7.0.tar", last modified: Sun May  8 13:09:57 2022, max compression
+gzip compressed data, was "grub2-theme-preview-2.8.0.tar", last modified: Wed May 10 11:36:17 2023, max compression
```

## Comparing `grub2-theme-preview-2.7.0.tar` & `grub2-theme-preview-2.8.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-05-08 13:09:57.946613 grub2-theme-preview-2.7.0/
--rw-r--r--   0 sping     (1000) sping     (1000)       30 2022-03-09 21:19:26.000000 grub2-theme-preview-2.7.0/.flake8
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-05-08 13:09:57.942613 grub2-theme-preview-2.7.0/.github/
--rw-r--r--   0 sping     (1000) sping     (1000)      510 2022-03-10 03:18:03.000000 grub2-theme-preview-2.7.0/.github/dependabot.yml
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-05-08 13:09:57.943613 grub2-theme-preview-2.7.0/.github/workflows/
--rw-r--r--   0 sping     (1000) sping     (1000)     2044 2022-05-08 12:26:59.000000 grub2-theme-preview-2.7.0/.github/workflows/pre_commit_detect_outdated.yml
--rw-r--r--   0 sping     (1000) sping     (1000)      880 2022-05-08 12:26:59.000000 grub2-theme-preview-2.7.0/.github/workflows/pre_commit_run.yml
--rw-r--r--   0 sping     (1000) sping     (1000)     1229 2022-05-08 12:26:59.000000 grub2-theme-preview-2.7.0/.github/workflows/python_test_suite.yml
--rw-r--r--   0 sping     (1000) sping     (1000)       34 2022-03-10 03:18:03.000000 grub2-theme-preview-2.7.0/.gitignore
--rw-r--r--   0 sping     (1000) sping     (1000)       28 2022-03-09 21:19:26.000000 grub2-theme-preview-2.7.0/.isort.cfg
--rw-r--r--   0 sping     (1000) sping     (1000)      697 2022-05-08 12:26:59.000000 grub2-theme-preview-2.7.0/.pre-commit-config.yaml
--rw-r--r--   0 sping     (1000) sping     (1000)      126 2022-03-09 21:19:26.000000 grub2-theme-preview-2.7.0/.style.yapf
--rw-r--r--   0 sping     (1000) sping     (1000)      291 2020-03-01 15:20:22.000000 grub2-theme-preview-2.7.0/Makefile
--rw-r--r--   0 sping     (1000) sping     (1000)     5049 2022-05-08 13:09:57.946613 grub2-theme-preview-2.7.0/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     3909 2022-05-08 13:09:01.000000 grub2-theme-preview-2.7.0/README.md
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-05-08 13:09:57.944613 grub2-theme-preview-2.7.0/grub2_theme_preview/
--rw-r--r--   0 sping     (1000) sping     (1000)        6 2015-01-12 12:31:14.000000 grub2-theme-preview-2.7.0/grub2_theme_preview/.gitignore
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2015-01-12 12:25:16.000000 grub2-theme-preview-2.7.0/grub2_theme_preview/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    20190 2022-05-08 13:09:01.000000 grub2-theme-preview-2.7.0/grub2_theme_preview/__main__.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-05-08 13:09:57.945613 grub2-theme-preview-2.7.0/grub2_theme_preview/tests/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2022-03-10 03:18:03.000000 grub2-theme-preview-2.7.0/grub2_theme_preview/tests/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     5249 2022-05-08 13:09:01.000000 grub2-theme-preview-2.7.0/grub2_theme_preview/tests/test_main.py
--rw-r--r--   0 sping     (1000) sping     (1000)      169 2022-05-08 13:09:13.000000 grub2-theme-preview-2.7.0/grub2_theme_preview/version.py
--rw-r--r--   0 sping     (1000) sping     (1000)      573 2015-06-30 19:32:04.000000 grub2-theme-preview-2.7.0/grub2_theme_preview/which.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-05-08 13:09:57.945613 grub2-theme-preview-2.7.0/grub2_theme_preview.egg-info/
--rw-r--r--   0 sping     (1000) sping     (1000)     5049 2022-05-08 13:09:56.000000 grub2-theme-preview-2.7.0/grub2_theme_preview.egg-info/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)      766 2022-05-08 13:09:57.000000 grub2-theme-preview-2.7.0/grub2_theme_preview.egg-info/SOURCES.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        1 2022-05-08 13:09:57.000000 grub2-theme-preview-2.7.0/grub2_theme_preview.egg-info/dependency_links.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       74 2022-05-08 13:09:57.000000 grub2-theme-preview-2.7.0/grub2_theme_preview.egg-info/entry_points.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       20 2022-05-08 13:09:57.000000 grub2-theme-preview-2.7.0/grub2_theme_preview.egg-info/top_level.txt
--rw-r--r--   0 sping     (1000) sping     (1000)      264 2022-05-08 12:26:59.000000 grub2-theme-preview-2.7.0/requirements.txt
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-05-08 13:09:57.945613 grub2-theme-preview-2.7.0/screenshots/
--rw-r--r--   0 sping     (1000) sping     (1000)   191492 2020-03-01 15:55:36.000000 grub2-theme-preview-2.7.0/screenshots/grub2-theme-preview__gutsblack-archlinux.png
--rw-r--r--   0 sping     (1000) sping     (1000)       38 2022-05-08 13:09:57.946613 grub2-theme-preview-2.7.0/setup.cfg
--rwxr-xr-x   0 sping     (1000) sping     (1000)     1739 2022-03-09 21:19:26.000000 grub2-theme-preview-2.7.0/setup.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-05-10 11:36:17.519554 grub2-theme-preview-2.8.0/
+-rw-r--r--   0 sping     (1000) sping     (1000)       30 2022-03-09 21:19:26.000000 grub2-theme-preview-2.8.0/.flake8
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-05-10 11:36:17.512555 grub2-theme-preview-2.8.0/.github/
+-rw-r--r--   0 sping     (1000) sping     (1000)      510 2022-03-10 03:18:03.000000 grub2-theme-preview-2.8.0/.github/dependabot.yml
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-05-10 11:36:17.513554 grub2-theme-preview-2.8.0/.github/workflows/
+-rw-r--r--   0 sping     (1000) sping     (1000)     2177 2023-05-09 20:24:02.000000 grub2-theme-preview-2.8.0/.github/workflows/pre_commit_detect_outdated.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)      991 2023-05-10 11:26:10.000000 grub2-theme-preview-2.8.0/.github/workflows/pre_commit_run.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     1315 2023-05-09 20:24:02.000000 grub2-theme-preview-2.8.0/.github/workflows/python_test_suite.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)       34 2022-03-10 03:18:03.000000 grub2-theme-preview-2.8.0/.gitignore
+-rw-r--r--   0 sping     (1000) sping     (1000)       28 2022-03-09 21:19:26.000000 grub2-theme-preview-2.8.0/.isort.cfg
+-rw-r--r--   0 sping     (1000) sping     (1000)      696 2023-05-09 20:24:02.000000 grub2-theme-preview-2.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 sping     (1000) sping     (1000)      126 2022-10-26 13:29:35.000000 grub2-theme-preview-2.8.0/.style.yapf
+-rw-r--r--   0 sping     (1000) sping     (1000)      291 2020-03-01 15:20:22.000000 grub2-theme-preview-2.8.0/Makefile
+-rw-r--r--   0 sping     (1000) sping     (1000)     5433 2023-05-10 11:36:17.518555 grub2-theme-preview-2.8.0/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)     4262 2023-04-17 23:27:34.000000 grub2-theme-preview-2.8.0/README.md
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-05-10 11:36:17.516554 grub2-theme-preview-2.8.0/grub2_theme_preview/
+-rw-r--r--   0 sping     (1000) sping     (1000)        6 2015-01-12 12:31:14.000000 grub2-theme-preview-2.8.0/grub2_theme_preview/.gitignore
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2015-01-12 12:25:16.000000 grub2-theme-preview-2.8.0/grub2_theme_preview/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    20271 2023-05-10 11:32:59.000000 grub2-theme-preview-2.8.0/grub2_theme_preview/__main__.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-05-10 11:36:17.518555 grub2-theme-preview-2.8.0/grub2_theme_preview/tests/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2022-03-10 03:18:03.000000 grub2-theme-preview-2.8.0/grub2_theme_preview/tests/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     5249 2022-05-08 13:09:01.000000 grub2-theme-preview-2.8.0/grub2_theme_preview/tests/test_main.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      169 2023-05-10 11:35:26.000000 grub2-theme-preview-2.8.0/grub2_theme_preview/version.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      573 2015-06-30 19:32:04.000000 grub2-theme-preview-2.8.0/grub2_theme_preview/which.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-05-10 11:36:17.517555 grub2-theme-preview-2.8.0/grub2_theme_preview.egg-info/
+-rw-r--r--   0 sping     (1000) sping     (1000)     5433 2023-05-10 11:36:17.000000 grub2-theme-preview-2.8.0/grub2_theme_preview.egg-info/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)      766 2023-05-10 11:36:17.000000 grub2-theme-preview-2.8.0/grub2_theme_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        1 2023-05-10 11:36:17.000000 grub2-theme-preview-2.8.0/grub2_theme_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       74 2023-05-10 11:36:17.000000 grub2-theme-preview-2.8.0/grub2_theme_preview.egg-info/entry_points.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       20 2023-05-10 11:36:17.000000 grub2-theme-preview-2.8.0/grub2_theme_preview.egg-info/top_level.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)      275 2023-05-09 20:24:02.000000 grub2-theme-preview-2.8.0/requirements.txt
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-05-10 11:36:17.518555 grub2-theme-preview-2.8.0/screenshots/
+-rw-r--r--   0 sping     (1000) sping     (1000)   191492 2020-03-01 15:55:36.000000 grub2-theme-preview-2.8.0/screenshots/grub2-theme-preview__gutsblack-archlinux.png
+-rw-r--r--   0 sping     (1000) sping     (1000)       38 2023-05-10 11:36:17.519554 grub2-theme-preview-2.8.0/setup.cfg
+-rwxr-xr-x   0 sping     (1000) sping     (1000)     1789 2022-11-15 12:29:35.000000 grub2-theme-preview-2.8.0/setup.py
```

### Comparing `grub2-theme-preview-2.7.0/.github/workflows/pre_commit_detect_outdated.yml` & `grub2-theme-preview-2.8.0/.github/workflows/pre_commit_detect_outdated.yml`

 * *Files 26% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 permissions:
   contents: write
   pull-requests: write
 
 jobs:
   pre_commit_detect_outdated:
     name: Detect outdated pre-commit hooks
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3.0.2
+      - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab  # v3.5.2
 
-      - name: Set up Python 3.10
-        uses: actions/setup-python@v3.1.2
+      - name: Set up Python 3.11
+        uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b  # v4.6.0
         with:
-          python-version: '3.10'
+          python-version: 3.11
 
       - name: Install pre-commit
         run: |-
           pip install \
             --disable-pip-version-check \
             --no-warn-script-location \
             --user \
@@ -37,15 +37,15 @@
       - name: Check for outdated hooks
         run: |-
           pre-commit autoupdate
           git diff -- .pre-commit-config.yaml
 
       - name: Create pull request from changes (if any)
         id: create-pull-request
-        uses: peter-evans/create-pull-request@v4
+        uses: peter-evans/create-pull-request@284f54f989303d2699d373481a0cfa13ad5a6666  # v5.0.1
         with:
           author: 'pre-commit <pre-commit@tools.invalid>'
           base: master
           body: |-
             For your consideration.
 
             :warning: Please **CLOSE AND RE-OPEN** this pull request so that [further workflow runs get triggered](https://github.com/peter-evans/create-pull-request/blob/main/docs/concepts-guidelines.md#triggering-further-workflow-runs) for this pull request.
```

### Comparing `grub2-theme-preview-2.7.0/.github/workflows/pre_commit_run.yml` & `grub2-theme-preview-2.8.0/.github/workflows/pre_commit_run.yml`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 on:
 - pull_request
 - push
 
 jobs:
   run_pre_commit:
     name: Run pre-commit on all files
-    runs-on: ubuntu-18.04
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3.0.2
+      - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab  # v3.5.2
 
       - name: Set up Python 3.8
-        uses: actions/setup-python@v3.1.2
+        uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b  # v4.6.0
         with:
           python-version: 3.8
 
       - name: Install pre-commit
         run: |-
           pip install \
             --disable-pip-version-check \
@@ -30,8 +30,8 @@
 
       - name: Install pre-commit hooks
         run: |-
           pre-commit install --install-hooks
 
       - name: Run pre-commit on all files
         run: |-
-          pre-commit run --all-files
+          pre-commit run --all-files --show-diff-on-failure
```

### Comparing `grub2-theme-preview-2.7.0/.github/workflows/python_test_suite.yml` & `grub2-theme-preview-2.8.0/.github/workflows/python_test_suite.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 - push
 
 jobs:
   python_test_suite:
     name: Run Python test suite
     strategy:
       matrix:
-        python-version: [3.7, '3.10']  # no particular need for in-between versions
-    runs-on: ubuntu-20.04
+        python-version: [3.7, 3.11]  # no particular need for in-between versions
+    runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3.0.2
+      - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab  # v3.5.2
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3.1.2
+        uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b  # v4.6.0
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install build dependencies
         run: |-
           set -x
           sudo apt-get update
```

### Comparing `grub2-theme-preview-2.7.0/.pre-commit-config.yaml` & `grub2-theme-preview-2.8.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Copyright (c) 2022 Sebastian Pipping <sebastian@pipping.org>
 # Licensed under GPL v2 or later
 
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.1
+    rev: v3.3.2
     hooks:
       - id: pyupgrade
         args: ['--py37-plus']
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: check-merge-conflict
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 3.9.2
+  - repo: https://github.com/PyCQA/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/google/yapf
-    rev: v0.32.0
+    rev: v0.33.0
     hooks:
       - id: yapf
```

### Comparing `grub2-theme-preview-2.7.0/PKG-INFO` & `grub2-theme-preview-2.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: grub2-theme-preview
-Version: 2.7.0
+Version: 2.8.0
 Summary: Preview a GRUB 2.x theme using KVM/QEMU
 Home-page: https://github.com/hartwork/grub2-theme-preview
-Download-URL: https://github.com/hartwork/grub2-theme-preview/archive/2.7.0.tar.gz
+Download-URL: https://github.com/hartwork/grub2-theme-preview/archive/2.8.0.tar.gz
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: GPL v2 or later
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Boot
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Run Python test suite](https://github.com/hartwork/grub2-theme-preview/actions/workflows/python_test_suite.yml/badge.svg)](https://github.com/hartwork/grub2-theme-preview/actions/workflows/python_test_suite.yml)
+
+
 # About
 
 **grub2-theme-preview** came into life when I was looking around for
 available GRUB 2.x themes and wanted a way to quickly see a theme
 in action without rebooting real hardware.
 
 It takes a theme folder (or just a single picture),
@@ -110,9 +114,7 @@
 
 debugging arguments:
   --debug               enable debugging output
   --plain-rescue-image  use unprocessed GRUB rescue image with no theme
                         patched in; useful for checking if a plain GRUB rescue
                         image shows up a GRUB shell, successfully.
 ```
-
-
```

### Comparing `grub2-theme-preview-2.7.0/README.md` & `grub2-theme-preview-2.8.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Run Python test suite](https://github.com/hartwork/grub2-theme-preview/actions/workflows/python_test_suite.yml/badge.svg)](https://github.com/hartwork/grub2-theme-preview/actions/workflows/python_test_suite.yml)
+
+
 # About
 
 **grub2-theme-preview** came into life when I was looking around for
 available GRUB 2.x themes and wanted a way to quickly see a theme
 in action without rebooting real hardware.
 
 It takes a theme folder (or just a single picture),
```

### Comparing `grub2-theme-preview-2.7.0/grub2_theme_preview/__main__.py` & `grub2-theme-preview-2.8.0/grub2_theme_preview/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,14 +377,15 @@
         candidates = [omvf_image]
     else:
         candidates = [
             '/usr/share/edk2-ovmf/OVMF_CODE.fd',  # Gentoo and its derivatives
             '/usr/share/edk2-ovmf/x64/OVMF_CODE.fd',  # Arch Linux and its derivatives
             '/usr/share/OVMF/OVMF_CODE.fd',  # Debian and its derivatives
             '/usr/share/edk2/ovmf/OVMF_CODE.fd',  # Fedora (and its derivatives?)
+            '/usr/share/qemu/edk2-x86_64-code.fd',  # Void Linux
         ]
 
     for candidate in candidates:
         if os.path.exists(candidate):
             return candidate, None, []
     else:
         return None, '/usr/share/[..]/OVMF_CODE.fd', ['edk2-ovmf', 'ovmf']
@@ -521,16 +522,15 @@
                     run_command += ['-display', options.qemu_display]
                 if options.qemu_vga is not None:
                     run_command += ['-vga', options.qemu_vga]
                 if options.qemu_full_screen:
                     run_command.append('-full-screen')
                 if is_efi_host:
                     run_command += [
-                        '-bios',
-                        omvf_image_path,
+                        '-drive', f'if=pflash,format=raw,readonly,file={omvf_image_path}'
                     ]
 
                 print('INFO: Please give GRUB a moment to show up in QEMU...')
 
                 qemu_exit_code = _run(run_command, options.verbose)
 
                 if qemu_exit_code not in (0, _KILL_BY_SIGNAL + signal.SIGINT):
```

### Comparing `grub2-theme-preview-2.7.0/grub2_theme_preview/tests/test_main.py` & `grub2-theme-preview-2.8.0/grub2_theme_preview/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `grub2-theme-preview-2.7.0/grub2_theme_preview/which.py` & `grub2-theme-preview-2.8.0/grub2_theme_preview/which.py`

 * *Files identical despite different names*

### Comparing `grub2-theme-preview-2.7.0/grub2_theme_preview.egg-info/PKG-INFO` & `grub2-theme-preview-2.8.0/grub2_theme_preview.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: grub2-theme-preview
-Version: 2.7.0
+Version: 2.8.0
 Summary: Preview a GRUB 2.x theme using KVM/QEMU
 Home-page: https://github.com/hartwork/grub2-theme-preview
-Download-URL: https://github.com/hartwork/grub2-theme-preview/archive/2.7.0.tar.gz
+Download-URL: https://github.com/hartwork/grub2-theme-preview/archive/2.8.0.tar.gz
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: GPL v2 or later
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: System :: Boot
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+[![Run Python test suite](https://github.com/hartwork/grub2-theme-preview/actions/workflows/python_test_suite.yml/badge.svg)](https://github.com/hartwork/grub2-theme-preview/actions/workflows/python_test_suite.yml)
+
+
 # About
 
 **grub2-theme-preview** came into life when I was looking around for
 available GRUB 2.x themes and wanted a way to quickly see a theme
 in action without rebooting real hardware.
 
 It takes a theme folder (or just a single picture),
@@ -110,9 +114,7 @@
 
 debugging arguments:
   --debug               enable debugging output
   --plain-rescue-image  use unprocessed GRUB rescue image with no theme
                         patched in; useful for checking if a plain GRUB rescue
                         image shows up a GRUB shell, successfully.
 ```
-
-
```

### Comparing `grub2-theme-preview-2.7.0/grub2_theme_preview.egg-info/SOURCES.txt` & `grub2-theme-preview-2.8.0/grub2_theme_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grub2-theme-preview-2.7.0/screenshots/grub2-theme-preview__gutsblack-archlinux.png` & `grub2-theme-preview-2.8.0/screenshots/grub2-theme-preview__gutsblack-archlinux.png`

 * *Files identical despite different names*

### Comparing `grub2-theme-preview-2.7.0/setup.py` & `grub2-theme-preview-2.8.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,12 +36,13 @@
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: System :: Boot',
         'Topic :: Utilities',
     ],
 )
```

