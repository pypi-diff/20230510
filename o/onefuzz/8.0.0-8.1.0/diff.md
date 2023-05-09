# Comparing `tmp/onefuzz-8.0.0.tar.gz` & `tmp/onefuzz-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\onefuzz-8.0.0.tar", last modified: Wed Apr 12 01:46:38 2023, max compression
+gzip compressed data, was "dist\onefuzz-8.1.0.tar", last modified: Mon May  8 15:54:48 2023, max compression
```

## Comparing `onefuzz-8.0.0.tar` & `onefuzz-8.1.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/
--rw-rw-rw-   0        0        0     1162 2023-04-12 01:46:00.000000 onefuzz-8.0.0/LICENSE
--rw-rw-rw-   0        0        0      162 2023-04-12 01:46:00.000000 onefuzz-8.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2335 2023-04-12 01:46:38.000000 onefuzz-8.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-04-12 01:46:00.000000 onefuzz-8.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/azure-functions-example/
--rw-rw-rw-   0        0        0      297 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/README.md
--rw-rw-rw-   0        0        0      141 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/host.json
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/azure-functions-example/info/
--rw-rw-rw-   0        0        0      391 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/info/__init__.py
--rw-rw-rw-   0        0        0      319 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/info/function.json
--rw-rw-rw-   0        0        0       57 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/azure-functions-example/requirements.txt
--rw-rw-rw-   0        0        0     7557 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/domato.py
--rw-rw-rw-   0        0        0      773 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/get-running.py
--rw-rw-rw-   0        0        0     4649 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/honggfuzz.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/llvm-source-coverage/
--rw-rw-rw-   0        0        0       41 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/.gitignore
--rw-rw-rw-   0        0        0     7347 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/llvm-source-coverage/inputs/
--rw-rw-rw-   0        0        0        4 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/inputs/input.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/llvm-source-coverage/setup/
--rw-rw-rw-   0        0        0      398 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/setup/Makefile
--rw-rw-rw-   0        0        0     1556 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/setup/simple.c
--rw-rw-rw-   0        0        0     3277 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
--rw-rw-rw-   0        0        0     2963 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/source-coverage.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/examples/llvm-source-coverage/tools/
--rw-rw-rw-   0        0        0     1177 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/llvm-source-coverage/tools/source-coverage.sh
--rw-rw-rw-   0        0        0     2800 2023-04-12 01:46:00.000000 onefuzz-8.0.0/examples/oss-fuzz-target.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/extra/
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/extra/pyinstaller/
--rw-rw-rw-   0        0        0      200 2023-04-12 01:46:00.000000 onefuzz-8.0.0/extra/pyinstaller/hook-onefuzz.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/
--rw-rw-rw-   0        0        0      129 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/__init__.py
--rw-rw-rw-   0        0        0      431 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/__main__.py
--rw-rw-rw-   0        0        0      126 2023-04-12 01:46:01.000000 onefuzz-8.0.0/onefuzz/__version__.py
--rw-rw-rw-   0        0        0    67292 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/api.py
--rw-rw-rw-   0        0        0     1059 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/azcopy.py
--rw-rw-rw-   0        0        0     2982 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/azure_identity_credential_adapter.py
--rw-rw-rw-   0        0        0    22112 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/backend.py
--rw-rw-rw-   0        0        0    20501 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/data/
--rw-rw-rw-   0        0        0     1223 2023-04-12 01:46:37.000000 onefuzz-8.0.0/onefuzz/data/licenses.json
--rw-rw-rw-   0        0        0     1004 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/data/privacy.txt
--rw-rw-rw-   0        0        0    29481 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/debug.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/job_templates/
--rw-rw-rw-   0        0        0        0 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/builder.py
--rw-rw-rw-   0        0        0     1723 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/cache.py
--rw-rw-rw-   0        0        0     6161 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/handlers.py
--rw-rw-rw-   0        0        0     3596 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/job_monitor.py
--rw-rw-rw-   0        0        0     3159 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/main.py
--rw-rw-rw-   0        0        0     1851 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/job_templates/manage.py
--rw-rw-rw-   0        0        0     1682 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/rdp.py
--rw-rw-rw-   0        0        0     3522 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/ssh.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/status/
--rw-rw-rw-   0        0        0        0 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/__init__.py
--rw-rw-rw-   0        0        0    13902 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/cache.py
--rw-rw-rw-   0        0        0     5152 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/cmd.py
--rw-rw-rw-   0        0        0      905 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/raw.py
--rw-rw-rw-   0        0        0     1856 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/signalr.py
--rw-rw-rw-   0        0        0     3009 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/top.py
--rw-rw-rw-   0        0        0     6255 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/status/top_view.py
--rw-rw-rw-   0        0        0     2882 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/template.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz/templates/
--rw-rw-rw-   0        0        0    10491 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/__init__.py
--rw-rw-rw-   0        0        0     6837 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/afl.py
--rw-rw-rw-   0        0        0    40759 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/libfuzzer.py
--rw-rw-rw-   0        0        0     8788 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/ossfuzz.py
--rw-rw-rw-   0        0        0     9530 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/radamsa.py
--rw-rw-rw-   0        0        0    10649 2023-04-12 01:46:00.000000 onefuzz-8.0.0/onefuzz/templates/regression.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1981 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      344 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-12 01:46:38.000000 onefuzz-8.0.0/onefuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2023-04-12 01:46:00.000000 onefuzz-8.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      101 2023-04-12 01:46:00.000000 onefuzz-8.0.0/requirements-lint.txt
--rw-rw-rw-   0        0        0      458 2023-04-12 01:46:01.000000 onefuzz-8.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-12 01:46:38.000000 onefuzz-8.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-04-12 01:46:00.000000 onefuzz-8.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 01:46:38.000000 onefuzz-8.0.0/tests/
--rw-rw-rw-   0        0        0        0 2023-04-12 01:46:00.000000 onefuzz-8.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-12 01:46:00.000000 onefuzz-8.0.0/tests/test_template_helper.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/
+-rw-rw-rw-   0        0        0     1162 2023-05-08 15:53:57.000000 onefuzz-8.1.0/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-05-08 15:53:57.000000 onefuzz-8.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2335 2023-05-08 15:54:48.000000 onefuzz-8.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1742 2023-05-08 15:53:57.000000 onefuzz-8.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/azure-functions-example/
+-rw-rw-rw-   0        0        0      297 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/README.md
+-rw-rw-rw-   0        0        0      141 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/host.json
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/azure-functions-example/info/
+-rw-rw-rw-   0        0        0      391 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/info/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/info/function.json
+-rw-rw-rw-   0        0        0       57 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/azure-functions-example/requirements.txt
+-rw-rw-rw-   0        0        0     7557 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/domato.py
+-rw-rw-rw-   0        0        0      773 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/get-running.py
+-rw-rw-rw-   0        0        0     4649 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/honggfuzz.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/llvm-source-coverage/
+-rw-rw-rw-   0        0        0       41 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/.gitignore
+-rw-rw-rw-   0        0        0     7347 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/llvm-source-coverage/inputs/
+-rw-rw-rw-   0        0        0        4 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/inputs/input.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/llvm-source-coverage/setup/
+-rw-rw-rw-   0        0        0      398 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/setup/Makefile
+-rw-rw-rw-   0        0        0     1556 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/setup/simple.c
+-rw-rw-rw-   0        0        0     3277 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
+-rw-rw-rw-   0        0        0     2963 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/source-coverage.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/examples/llvm-source-coverage/tools/
+-rw-rw-rw-   0        0        0     1177 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/llvm-source-coverage/tools/source-coverage.sh
+-rw-rw-rw-   0        0        0     2800 2023-05-08 15:53:57.000000 onefuzz-8.1.0/examples/oss-fuzz-target.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/extra/
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/extra/pyinstaller/
+-rw-rw-rw-   0        0        0      200 2023-05-08 15:53:57.000000 onefuzz-8.1.0/extra/pyinstaller/hook-onefuzz.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/
+-rw-rw-rw-   0        0        0      129 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/__main__.py
+-rw-rw-rw-   0        0        0      126 2023-05-08 15:53:58.000000 onefuzz-8.1.0/onefuzz/__version__.py
+-rw-rw-rw-   0        0        0    68842 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/api.py
+-rw-rw-rw-   0        0        0     1059 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/azcopy.py
+-rw-rw-rw-   0        0        0     2982 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/azure_identity_credential_adapter.py
+-rw-rw-rw-   0        0        0    22112 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/backend.py
+-rw-rw-rw-   0        0        0    20501 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/data/
+-rw-rw-rw-   0        0        0     1223 2023-05-08 15:54:47.000000 onefuzz-8.1.0/onefuzz/data/licenses.json
+-rw-rw-rw-   0        0        0     1004 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/data/privacy.txt
+-rw-rw-rw-   0        0        0    31082 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/debug.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/job_templates/
+-rw-rw-rw-   0        0        0        0 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/__init__.py
+-rw-rw-rw-   0        0        0     4095 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/builder.py
+-rw-rw-rw-   0        0        0     1723 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/cache.py
+-rw-rw-rw-   0        0        0     6161 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/handlers.py
+-rw-rw-rw-   0        0        0     3596 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/job_monitor.py
+-rw-rw-rw-   0        0        0     3159 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/main.py
+-rw-rw-rw-   0        0        0     1851 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/job_templates/manage.py
+-rw-rw-rw-   0        0        0     1682 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/rdp.py
+-rw-rw-rw-   0        0        0     3522 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/ssh.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/status/
+-rw-rw-rw-   0        0        0        0 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/cache.py
+-rw-rw-rw-   0        0        0     5152 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/cmd.py
+-rw-rw-rw-   0        0        0      905 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/raw.py
+-rw-rw-rw-   0        0        0     1856 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/signalr.py
+-rw-rw-rw-   0        0        0     3009 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/top.py
+-rw-rw-rw-   0        0        0     6255 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/status/top_view.py
+-rw-rw-rw-   0        0        0     2882 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/template.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz/templates/
+-rw-rw-rw-   0        0        0    10491 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/__init__.py
+-rw-rw-rw-   0        0        0     6837 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/afl.py
+-rw-rw-rw-   0        0        0    42155 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/libfuzzer.py
+-rw-rw-rw-   0        0        0     8788 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/ossfuzz.py
+-rw-rw-rw-   0        0        0     9530 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/radamsa.py
+-rw-rw-rw-   0        0        0    10649 2023-05-08 15:53:57.000000 onefuzz-8.1.0/onefuzz/templates/regression.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1981 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      344 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-08 15:54:48.000000 onefuzz-8.1.0/onefuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2023-05-08 15:53:57.000000 onefuzz-8.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      101 2023-05-08 15:53:57.000000 onefuzz-8.1.0/requirements-lint.txt
+-rw-rw-rw-   0        0        0      458 2023-05-08 15:53:58.000000 onefuzz-8.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 15:54:48.000000 onefuzz-8.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-05-08 15:53:57.000000 onefuzz-8.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 15:54:48.000000 onefuzz-8.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-08 15:53:57.000000 onefuzz-8.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-05-08 15:53:57.000000 onefuzz-8.1.0/tests/test_template_helper.py
```

### Comparing `onefuzz-8.0.0/LICENSE` & `onefuzz-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/PKG-INFO` & `onefuzz-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.0.0
+Version: 8.1.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.0.0/README.md` & `onefuzz-8.1.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/domato.py` & `onefuzz-8.1.0/examples/domato.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/get-running.py` & `onefuzz-8.1.0/examples/get-running.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/honggfuzz.py` & `onefuzz-8.1.0/examples/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/llvm-source-coverage/README.md` & `onefuzz-8.1.0/examples/llvm-source-coverage/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/llvm-source-coverage/setup/simple.c` & `onefuzz-8.1.0/examples/llvm-source-coverage/setup/simple.c`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py` & `onefuzz-8.1.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/llvm-source-coverage/source-coverage.py` & `onefuzz-8.1.0/examples/llvm-source-coverage/source-coverage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/llvm-source-coverage/tools/source-coverage.sh` & `onefuzz-8.1.0/examples/llvm-source-coverage/tools/source-coverage.sh`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/examples/oss-fuzz-target.py` & `onefuzz-8.1.0/examples/oss-fuzz-target.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/api.py` & `onefuzz-8.1.0/onefuzz/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,28 @@
     def get(self, container: primitives.Container, filename: str) -> bytes:
         """get a file from a container"""
         self.logger.debug("getting file from container: %s:%s", container, filename)
         client = self._get_client(container)
         downloaded = client.download_blob(filename)
         return downloaded
 
+    def download(
+        self, container: primitives.Container, blob_name: str, file_path: Optional[str]
+    ) -> "None":
+        """download a container file to a local path"""
+        self.logger.debug("getting file from container: %s:%s", container, blob_name)
+        client = self._get_client(container)
+        downloaded = client.download_blob(blob_name)
+        local_file = file_path if file_path else blob_name
+        with open(local_file, "wb") as handle:
+            handle.write(downloaded)
+        self.logger.debug(
+            f"downloaded blob {blob_name} from container {container} to {local_file}"
+        )
+
     def upload_file(
         self,
         container: primitives.Container,
         file_path: str,
         blob_name: Optional[str] = None,
     ) -> None:
         """uploads a file to a container"""
@@ -1293,14 +1307,32 @@
             "POST",
             models.Pool,
             data=requests.PoolCreate(
                 name=name, os=os, arch=arch, managed=managed, object_id=object_id
             ),
         )
 
+    def update(
+        self,
+        name: str,
+        object_id: Optional[UUID] = None,
+    ) -> models.Pool:
+        """
+        Update a worker pool
+
+        :param str name: Name of the worker-pool
+        """
+        self.logger.debug("create worker pool")
+
+        return self._req_model(
+            "PATCH",
+            models.Pool,
+            data=requests.PoolUpdate(name=name, object_id=object_id),
+        )
+
     def get_config(self, pool_name: primitives.PoolName) -> models.AgentConfig:
         """Get the agent configuration for the pool"""
 
         pool = self.get(pool_name)
 
         if pool.config is None:
             raise Exception("Missing AgentConfig in response")
@@ -1729,14 +1761,29 @@
 
     def post(
         self, req: requests.TemplateValidationPost
     ) -> responses.TemplateValidationResponse:
         return self._req_model("POST", responses.TemplateValidationResponse, data=req)
 
 
+class Events(Endpoint):
+    """Interact with Onefuzz events"""
+
+    endpoint = "events"
+
+    def get(self, event_id: UUID_EXPANSION) -> events.EventGetResponse:
+        """Get an event's payload by id"""
+        self.logger.debug("get event: %s", event_id)
+        return self._req_model(
+            "GET",
+            events.EventGetResponse,
+            data=requests.EventsGet(event_id=event_id),
+        )
+
+
 class Command:
     def __init__(self, onefuzz: "Onefuzz", logger: logging.Logger):
         self.onefuzz = onefuzz
         self.logger = logger
 
 
 class Utils(Command):
@@ -1820,14 +1867,15 @@
         self.pools = Pool(self)
         self.scalesets = Scaleset(self)
         self.nodes = Node(self)
         self.webhooks = Webhooks(self)
         self.tools = Tools(self)
         self.instance_config = InstanceConfigCmd(self)
         self.validate_scriban = ValidateScriban(self)
+        self.events = Events(self)
 
         # these are externally developed cli modules
         self.template = Template(self, self.logger)
         self.debug = Debug(self, self.logger)
         self.status = Status(self, self.logger)
         self.utils = Utils(self, self.logger)
```

### Comparing `onefuzz-8.0.0/onefuzz/azcopy.py` & `onefuzz-8.1.0/onefuzz/azcopy.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/azure_identity_credential_adapter.py` & `onefuzz-8.1.0/onefuzz/azure_identity_credential_adapter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/backend.py` & `onefuzz-8.1.0/onefuzz/backend.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/cli.py` & `onefuzz-8.1.0/onefuzz/cli.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/data/licenses.json` & `onefuzz-8.1.0/onefuzz/data/licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {'1': "{'Version': '6.6.0'}", '3': "{'Version': '5.10.1'}"}*

```diff
@@ -5,27 +5,27 @@
         "URL": "https://altgraph.readthedocs.io",
         "Version": "0.17.3"
     },
     {
         "License": "Apache Software License",
         "Name": "importlib-metadata",
         "URL": "https://github.com/python/importlib_metadata",
-        "Version": "6.3.0"
+        "Version": "6.6.0"
     },
     {
         "License": "MIT",
         "Name": "pefile",
         "URL": "https://github.com/erocarrera/pefile",
         "Version": "2023.2.7"
     },
     {
         "License": "GNU General Public License v2 (GPLv2)",
         "Name": "pyinstaller",
         "URL": "https://www.pyinstaller.org/",
-        "Version": "5.10.0"
+        "Version": "5.10.1"
     },
     {
         "License": "UNKNOWN",
         "Name": "pyinstaller-hooks-contrib",
         "URL": "https://github.com/pyinstaller/pyinstaller-hooks-contrib",
         "Version": "2023.2"
     },
```

### Comparing `onefuzz-8.0.0/onefuzz/data/privacy.txt` & `onefuzz-8.1.0/onefuzz/data/privacy.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/debug.py` & `onefuzz-8.1.0/onefuzz/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 # Licensed under the MIT License.
 
 import json
 import logging
 import os
 import tempfile
 import time
+import uuid
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 from urllib.parse import urlparse
 from uuid import UUID
 
 import jmespath
 from azure.applicationinsights import ApplicationInsightsDataClient
 from azure.applicationinsights.models import QueryBody
 from azure.identity import AzureCliCredential
 from azure.storage.blob import ContainerClient
-from onefuzztypes import models, requests
+from onefuzztypes import models, requests, responses
 from onefuzztypes.enums import ContainerType, TaskType
 from onefuzztypes.models import BlobRef, Job, NodeAssignment, Report, Task, TaskConfig
 from onefuzztypes.primitives import Container, Directory, PoolName
 from onefuzztypes.responses import TemplateValidationResponse
 
-from onefuzz.api import UUID_EXPANSION, Command, Onefuzz
+from onefuzz.api import UUID_EXPANSION, Command, Endpoint, Onefuzz
 
 from .azure_identity_credential_adapter import AzureIdentityCredentialAdapter
 from .backend import wait
 from .rdp import rdp_connect
 from .ssh import ssh_connect
 
 EMPTY_SHA256 = "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"
@@ -771,14 +772,15 @@
         *,
         report_container_type: ContainerType = ContainerType.unique_reports,
         crash_name: str = "fake-crash-sample",
     ) -> None:
         """Inject a report into the specified crash reporting task"""
 
         task = self.onefuzz.tasks.get(task_id)
+
         crashes = self._get_container(task, ContainerType.crashes)
         reports = self._get_container(task, report_container_type)
 
         if crashes is None:
             raise Exception("task does not have a crashes container")
 
         if reports is None:
@@ -788,45 +790,86 @@
 
         with tempfile.TemporaryDirectory() as tempdir:
             file_path = os.path.join(tempdir, crash_name)
             with open(file_path, "w") as handle:
                 handle.write("")
             self.onefuzz.containers.files.upload_file(crashes, file_path, crash_name)
 
-        report = Report(
-            input_blob=BlobRef(
-                account=self._get_storage_account(crashes),
-                container=crashes,
-                name=crash_name,
+        input_blob_ref = BlobRef(
+            account=self._get_storage_account(crashes),
+            container=crashes,
+            name=crash_name,
+        )
+
+        target_exe = task.config.task.target_exe if task.config.task.target_exe else ""
+        report = self._create_report(
+            task.job_id, task.task_id, target_exe, input_blob_ref
+        )
+
+        with tempfile.TemporaryDirectory() as tempdir:
+            file_path = os.path.join(tempdir, "report.json")
+            with open(file_path, "w") as handle:
+                handle.write(report.json())
+
+            self.onefuzz.containers.files.upload_file(
+                reports, file_path, crash_name + ".json"
+            )
+
+    def test_template(
+        self, task_id: UUID_EXPANSION, notificationConfig: models.NotificationConfig
+    ) -> responses.NotificationTestResponse:
+        """Test a notification template"""
+        endpoint = Endpoint(self.onefuzz)
+        task = self.onefuzz.tasks.get(task_id)
+        input_blob_ref = BlobRef(
+            account="dummy-storage-account",
+            container="test-notification-crashes",
+            name="fake-crash-sample",
+        )
+
+        report = self._create_report(
+            task.job_id, task.task_id, "fake_target.exe", input_blob_ref
+        )
+        report.report_url = "https://dummy-container.blob.core.windows.net/dummy-reports/dummy-report.json"
+
+        return endpoint._req_model(
+            "POST",
+            responses.NotificationTestResponse,
+            data=requests.NotificationTest(
+                report=report,
+                notification=models.Notification(
+                    container=Container("test-notification-reports"),
+                    notification_id=uuid.uuid4(),
+                    config=notificationConfig.config,
+                ),
             ),
-            executable=task.config.task.target_exe,
+            alternate_endpoint="notifications/test",
+        )
+
+    def _create_report(
+        self, job_id: UUID, task_id: UUID, target_exe: str, input_blob_ref: BlobRef
+    ) -> Report:
+        return Report(
+            input_blob=input_blob_ref,
+            executable=target_exe,
             crash_type="fake crash report",
             crash_site="fake crash site",
             call_stack=["#0 fake", "#1 call", "#2 stack"],
             call_stack_sha256=ZERO_SHA256,
             input_sha256=EMPTY_SHA256,
             asan_log="fake asan log",
             task_id=task_id,
-            job_id=task.job_id,
+            job_id=job_id,
             minimized_stack=[],
             minimized_stack_function_names=[],
             tool_name="libfuzzer",
             tool_version="1.2.3",
             onefuzz_version="1.2.3",
         )
 
-        with tempfile.TemporaryDirectory() as tempdir:
-            file_path = os.path.join(tempdir, "report.json")
-            with open(file_path, "w") as handle:
-                handle.write(report.json())
-
-            self.onefuzz.containers.files.upload_file(
-                reports, file_path, crash_name + ".json"
-            )
-
 
 class Debug(Command):
     """Debug running jobs"""
 
     def __init__(self, onefuzz: Any, logger: logging.Logger):
         super().__init__(onefuzz, logger)
         self.scalesets = DebugScaleset(onefuzz, logger)
```

### Comparing `onefuzz-8.0.0/onefuzz/job_templates/builder.py` & `onefuzz-8.1.0/onefuzz/job_templates/builder.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/job_templates/cache.py` & `onefuzz-8.1.0/onefuzz/job_templates/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/job_templates/handlers.py` & `onefuzz-8.1.0/onefuzz/job_templates/handlers.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/job_templates/job_monitor.py` & `onefuzz-8.1.0/onefuzz/job_templates/job_monitor.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/job_templates/main.py` & `onefuzz-8.1.0/onefuzz/job_templates/main.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/job_templates/manage.py` & `onefuzz-8.1.0/onefuzz/job_templates/manage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/rdp.py` & `onefuzz-8.1.0/onefuzz/rdp.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/ssh.py` & `onefuzz-8.1.0/onefuzz/ssh.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/status/cache.py` & `onefuzz-8.1.0/onefuzz/status/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/status/cmd.py` & `onefuzz-8.1.0/onefuzz/status/cmd.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/status/raw.py` & `onefuzz-8.1.0/onefuzz/status/raw.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/status/signalr.py` & `onefuzz-8.1.0/onefuzz/status/signalr.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/status/top.py` & `onefuzz-8.1.0/onefuzz/status/top.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/status/top_view.py` & `onefuzz-8.1.0/onefuzz/status/top_view.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/template.py` & `onefuzz-8.1.0/onefuzz/template.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/templates/__init__.py` & `onefuzz-8.1.0/onefuzz/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/templates/afl.py` & `onefuzz-8.1.0/onefuzz/templates/afl.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/templates/libfuzzer.py` & `onefuzz-8.1.0/onefuzz/templates/libfuzzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,24 +61,32 @@
         tags: Optional[Dict[str, str]] = None,
         check_retry_count: Optional[int] = None,
         crash_report_timeout: Optional[int] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         colocate_secondary_tasks: bool = True,
-        check_fuzzer_help: bool = True,
+        check_fuzzer_help: bool = False,
+        no_check_fuzzer_help: bool = False,
         expect_crash_on_failure: bool = False,
         minimized_stack_depth: Optional[int] = None,
         module_allowlist: Optional[str] = None,
         source_allowlist: Optional[str] = None,
         analyzer_exe: Optional[str] = None,
         analyzer_options: Optional[List[str]] = None,
         analyzer_env: Optional[Dict[str, str]] = None,
         tools: Optional[Container] = None,
     ) -> None:
+        if check_fuzzer_help:
+            self.logger.warning(
+                "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
+            )
+        check_fuzzer_help = not no_check_fuzzer_help
+        del no_check_fuzzer_help
+
         target_options = target_options or []
 
         regression_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.unique_reports, containers[ContainerType.unique_reports]),
             (
@@ -344,15 +352,16 @@
         readonly_inputs: Optional[Container] = None,
         dryrun: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         colocate_secondary_tasks: bool = True,
-        check_fuzzer_help: bool = True,
+        check_fuzzer_help: bool = False,
+        no_check_fuzzer_help: bool = False,
         expect_crash_on_failure: bool = False,
         minimized_stack_depth: Optional[int] = None,
         module_allowlist: Optional[File] = None,
         source_allowlist: Optional[File] = None,
         analyzer_exe: Optional[str] = None,
         analyzer_options: Optional[List[str]] = None,
         analyzer_env: Optional[Dict[str, str]] = None,
@@ -363,14 +372,21 @@
         """
         Basic libfuzzer job
 
         :param bool ensemble_sync_delay: Specify duration between
             syncing inputs during ensemble fuzzing (0 to disable).
         """
 
+        if check_fuzzer_help:
+            self.logger.warning(
+                "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
+            )
+        check_fuzzer_help = not no_check_fuzzer_help
+        del no_check_fuzzer_help
+
         # verify containers exist
         if existing_inputs:
             self.onefuzz.containers.get(existing_inputs)
 
         if readonly_inputs:
             self.onefuzz.containers.get(readonly_inputs)
 
@@ -508,20 +524,27 @@
         wait_for_files: Optional[List[ContainerType]] = None,
         extra_files: Optional[List[File]] = None,
         existing_inputs: Optional[List[Container]] = None,
         dryrun: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         preserve_existing_outputs: bool = False,
-        check_fuzzer_help: bool = True,
+        check_fuzzer_help: bool = False,
+        no_check_fuzzer_help: bool = False,
         extra_container: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         libfuzzer merge task
         """
+        if check_fuzzer_help:
+            self.logger.warning(
+                "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
+            )
+        check_fuzzer_help = not no_check_fuzzer_help
+        del no_check_fuzzer_help
 
         # verify containers exist
         if existing_inputs:
             for existing_container in existing_inputs:
                 self.onefuzz.containers.get(existing_container)
         elif not inputs:
             self.logger.error(
@@ -866,21 +889,28 @@
         wait_for_files: Optional[List[ContainerType]] = None,
         existing_inputs: Optional[Container] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         crash_report_timeout: Optional[int] = 1,
         check_retry_count: Optional[int] = 300,
-        check_fuzzer_help: bool = True,
+        check_fuzzer_help: bool = False,
+        no_check_fuzzer_help: bool = False,
         extra_container: Optional[Container] = None,
         crashes: Optional[Container] = None,
     ) -> Optional[Job]:
         """
         libfuzzer tasks, wrapped via qemu-user (PREVIEW FEATURE)
         """
+        if check_fuzzer_help:
+            self.logger.warning(
+                "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
+            )
+        check_fuzzer_help = not no_check_fuzzer_help
+        del no_check_fuzzer_help
 
         self.logger.warning(
             "qemu_user jobs are a preview feature and may change in the future"
         )
 
         pool = self.onefuzz.pools.get(pool_name)
         if pool.os != OS.linux:
```

### Comparing `onefuzz-8.0.0/onefuzz/templates/ossfuzz.py` & `onefuzz-8.1.0/onefuzz/templates/ossfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/templates/radamsa.py` & `onefuzz-8.1.0/onefuzz/templates/radamsa.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz/templates/regression.py` & `onefuzz-8.1.0/onefuzz/templates/regression.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/onefuzz.egg-info/PKG-INFO` & `onefuzz-8.1.0/onefuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.0.0
+Version: 8.1.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.0.0/onefuzz.egg-info/SOURCES.txt` & `onefuzz-8.1.0/onefuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/setup.py` & `onefuzz-8.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.0.0/tests/test_template_helper.py` & `onefuzz-8.1.0/tests/test_template_helper.py`

 * *Files identical despite different names*

