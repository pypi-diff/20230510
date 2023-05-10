# Comparing `tmp/iqm-cortex-cli-4.1.tar.gz` & `tmp/iqm-cortex-cli-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqm-cortex-cli-4.1.tar", last modified: Wed May  3 14:16:58 2023, max compression
+gzip compressed data, was "iqm-cortex-cli-4.2.tar", last modified: Wed May 10 08:50:49 2023, max compression
```

## Comparing `iqm-cortex-cli-4.1.tar` & `iqm-cortex-cli-4.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.440132 iqm-cortex-cli-4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/.github/workflows/tag_and_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/DEVELOPMENT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_static/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_templates/autosummary-class-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_templates/autosummary-module-template.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/_templates/versioning.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/docs/readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.444132 iqm-cortex-cli-4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/src/cortex_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    26350 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/cortex_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/src/cortex_cli/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-03 14:16:58.000000 iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tag-from-pipeline.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_auth_login_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_auth_logout_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_auth_status_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/cortex_cli_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 14:16:58.448132 iqm-cortex-cli-4.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/resources/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/resources/tokens.json
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tests/token_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-03 14:16:26.000000 iqm-cortex-cli-4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.432315 iqm-cortex-cli-4.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.424315 iqm-cortex-cli-4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.428315 iqm-cortex-cli-4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/.github/workflows/tag_and_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/DEVELOPMENT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-10 08:50:49.432315 iqm-cortex-cli-4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.428315 iqm-cortex-cli-4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.424315 iqm-cortex-cli-4.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.428315 iqm-cortex-cli-4.2/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)   618471 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/_static/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.428315 iqm-cortex-cli-4.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/_templates/autosummary-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/_templates/autosummary-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/_templates/versioning.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/docs/readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      199 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:50:49.432315 iqm-cortex-cli-4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.424315 iqm-cortex-cli-4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.428315 iqm-cortex-cli-4.2/src/cortex_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/src/cortex_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/src/cortex_cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26447 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/src/cortex_cli/cortex_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/src/cortex_cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/src/cortex_cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/src/cortex_cli/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.432315 iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-05-10 08:50:49.000000 iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-10 08:50:49.000000 iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:50:49.000000 iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 08:50:49.000000 iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-10 08:50:49.000000 iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 08:50:49.000000 iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tag-from-pipeline.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.432315 iqm-cortex-cli-4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/cortex_cli_auth_login_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/cortex_cli_auth_logout_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/cortex_cli_auth_status_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/cortex_cli_init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/cortex_cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:50:49.432315 iqm-cortex-cli-4.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/resources/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/resources/tokens.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tests/token_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-10 08:50:16.000000 iqm-cortex-cli-4.2/tox.ini
```

### Comparing `iqm-cortex-cli-4.1/.github/workflows/ci.yml` & `iqm-cortex-cli-4.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/.github/workflows/publish.yml` & `iqm-cortex-cli-4.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/.github/workflows/tag_and_release.yml` & `iqm-cortex-cli-4.2/.github/workflows/tag_and_release.yml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/CHANGELOG.rst` & `iqm-cortex-cli-4.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 Changelog
 =========
 
+Version 4.2
+===========
+
+* Fix ``init`` command non-interactive mode failing for some orders of options `#44 <https://github.com/iqm-finland/cortex-cli/pull/44>`_
+
 Version 4.1
 ===========
 
 * Generate license information for dependencies on every release `#44 <https://github.com/iqm-finland/cortex-cli/pull/44>`_
 
 Version 4.0
 ===========
```

### Comparing `iqm-cortex-cli-4.1/DEVELOPMENT.rst` & `iqm-cortex-cli-4.2/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/LICENSE.rst` & `iqm-cortex-cli-4.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/PKG-INFO` & `iqm-cortex-cli-4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 4.1
+Version: 4.2
 Summary: CLI for managing user authentication when using IQM quantum computers
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-4.1/README.rst` & `iqm-cortex-cli-4.2/README.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/docs/Makefile` & `iqm-cortex-cli-4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/docs/_static/images/favicon.ico` & `iqm-cortex-cli-4.2/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/docs/_static/images/logo.png` & `iqm-cortex-cli-4.2/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/docs/_templates/autosummary-class-template.rst` & `iqm-cortex-cli-4.2/docs/_templates/autosummary-class-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/docs/_templates/autosummary-module-template.rst` & `iqm-cortex-cli-4.2/docs/_templates/autosummary-module-template.rst`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/docs/_templates/page.html` & `iqm-cortex-cli-4.2/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/docs/_templates/versioning.html` & `iqm-cortex-cli-4.2/docs/_templates/versioning.html`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/docs/conf.py` & `iqm-cortex-cli-4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/pyproject.toml` & `iqm-cortex-cli-4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/src/cortex_cli/__init__.py` & `iqm-cortex-cli-4.2/src/cortex_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/src/cortex_cli/auth.py` & `iqm-cortex-cli-4.2/src/cortex_cli/auth.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/src/cortex_cli/cortex_cli.py` & `iqm-cortex-cli-4.2/src/cortex_cli/cortex_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,19 @@
     Args:
         ctx: click context
         param: click prompt param object
         path: path provided by user
     Returns:
         str: confirmed and finalized path
     """
-    if ctx.obj and param.name in ctx.obj:
+    if ctx.obj is None:
+        ctx.obj = {}
+    if param.name in ctx.obj:
         return path
-    ctx.obj = {param.name: True}
+    ctx.obj[param.name] = True
 
     # File doesn't exist, no need to confirm overwriting
     if not Path(path).is_file():
         return path
 
     # File exists, so user must either overwrite or enter a new path
     while True:
@@ -209,15 +211,17 @@
     Args:
         ctx: click context
         param: click prompt param object
         base_url (str): auth server base URL to validate
     Returns:
         str: validated auth server base URL
     """
-    if ctx.obj and param.name in ctx.obj:
+    if ctx.obj is None:
+        ctx.obj = {}
+    if param.name in ctx.obj:
         return base_url
 
     is_valid = False
     while not is_valid:
         try:
             master = requests.get(f'{base_url}/realms/master', timeout=AUTH_REQUESTS_TIMEOUT)
             assert master.status_code == 200
@@ -239,15 +243,17 @@
     Args:
         ctx: click context
         param: click prompt param object
         realm (str): name of the realm
     Returns:
         str: validated realm name
     """
-    if ctx.obj and param.name in ctx.obj:
+    if ctx.obj is None:
+        ctx.obj = {}
+    if param.name in ctx.obj:
         return realm
 
     base_url = ctx.obj.get('auth_server_url', None)
     if base_url is None:
         raise click.UsageError('Can not set realm name before setting auth server URL.')
 
     is_valid = False
```

### Comparing `iqm-cortex-cli-4.1/src/cortex_cli/models.py` & `iqm-cortex-cli-4.2/src/cortex_cli/models.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/src/cortex_cli/token_manager.py` & `iqm-cortex-cli-4.2/src/cortex_cli/token_manager.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/PKG-INFO` & `iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqm-cortex-cli
-Version: 4.1
+Version: 4.2
 Summary: CLI for managing user authentication when using IQM quantum computers
 Author-email: IQM Finland Oy <developers@meetiqm.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `iqm-cortex-cli-4.1/src/iqm_cortex_cli.egg-info/SOURCES.txt` & `iqm-cortex-cli-4.2/src/iqm_cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tag-from-pipeline.sh` & `iqm-cortex-cli-4.2/tag-from-pipeline.sh`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tests/auth_test.py` & `iqm-cortex-cli-4.2/tests/auth_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tests/conftest.py` & `iqm-cortex-cli-4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tests/cortex_cli_auth_login_test.py` & `iqm-cortex-cli-4.2/tests/cortex_cli_auth_login_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tests/cortex_cli_auth_logout_test.py` & `iqm-cortex-cli-4.2/tests/cortex_cli_auth_logout_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tests/cortex_cli_auth_status_test.py` & `iqm-cortex-cli-4.2/tests/cortex_cli_auth_status_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tests/cortex_cli_init_test.py` & `iqm-cortex-cli-4.2/tests/cortex_cli_init_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,46 +11,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Tests for Cortex CLI's init command
 """
 
+import itertools
 import json
 import os
 from pathlib import Path
 
 from click.testing import CliRunner
 from mockito import unstub
+import pytest
 
 from cortex_cli.cortex_cli import cortex_cli
 from tests.conftest import expect_process_terminate, prepare_auth_server_urls
 
 
-def test_init_saves_config_file(config_dict):
+@pytest.mark.parametrize('first_option', ['--config-file', '--tokens-file', '--auth-server-url', '--client-id'])
+def test_init_saves_config_file(config_dict, first_option):
     """
     Tests that ``cortex init`` produces config file.
+
+    Having different options as first one is tested since it can affect the initialization of ``click.Context``.
+    Specifying ``realm`` before ``auth-server-url`` is not allowed, so that case is not included.
     """
     prepare_auth_server_urls(config_dict)
     runner = CliRunner()
     with runner.isolated_filesystem():
+        options_map = {
+            '--config-file': 'config.json',
+            '--tokens-file': config_dict['tokens_file'],
+            '--auth-server-url': config_dict['auth_server_url'],
+            '--realm': config_dict['realm'],
+            '--client-id': config_dict['client_id'],
+        }
         result = runner.invoke(
             cortex_cli,
             [
                 'init',
-                '--config-file',
-                'config.json',
-                '--tokens-file',
-                config_dict['tokens_file'],
-                '--auth-server-url',
-                config_dict['auth_server_url'],
-                '--realm',
-                config_dict['realm'],
-                '--client-id',
-                config_dict['client_id'],
+                first_option,
+                options_map[first_option],
+                *itertools.chain.from_iterable([item for item in options_map.items() if item[0] != first_option]),
             ],
         )
         assert result.exit_code == 0
         assert 'Cortex CLI initialized successfully' in result.output
         with open('config.json', 'r', encoding='utf-8') as config_file:
             loaded_config = json.load(config_file)
             assert loaded_config == config_dict
```

### Comparing `iqm-cortex-cli-4.1/tests/cortex_cli_test.py` & `iqm-cortex-cli-4.2/tests/cortex_cli_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tests/resources/tokens.json` & `iqm-cortex-cli-4.2/tests/resources/tokens.json`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tests/token_manager_test.py` & `iqm-cortex-cli-4.2/tests/token_manager_test.py`

 * *Files identical despite different names*

### Comparing `iqm-cortex-cli-4.1/tox.ini` & `iqm-cortex-cli-4.2/tox.ini`

 * *Files identical despite different names*

