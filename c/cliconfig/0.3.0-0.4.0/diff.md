# Comparing `tmp/cliconfig-0.3.0.tar.gz` & `tmp/cliconfig-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.3.0.tar", last modified: Mon May  8 22:58:14 2023, max compression
+gzip compressed data, was "cliconfig-0.4.0.tar", last modified: Wed May 10 02:19:33 2023, max compression
```

## Comparing `cliconfig-0.3.0.tar` & `cliconfig-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.605119 cliconfig-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.597119 cliconfig-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.597119 cliconfig-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-08 22:57:58.000000 cliconfig-0.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-08 22:57:58.000000 cliconfig-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 22:57:58.000000 cliconfig-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-08 22:58:14.601119 cliconfig-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-05-08 22:57:58.000000 cliconfig-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.597119 cliconfig-0.3.0/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-05-08 22:57:58.000000 cliconfig-0.3.0/cliconfig/processings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 22:58:14.000000 cliconfig-0.3.0/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/manipulate.md
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-08 22:57:58.000000 cliconfig-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-08 22:57:58.000000 cliconfig-0.3.0/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 22:57:58.000000 cliconfig-0.3.0/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-08 22:57:58.000000 cliconfig-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-08 22:57:58.000000 cliconfig-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 22:57:58.000000 cliconfig-0.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 22:57:58.000000 cliconfig-0.3.0/scripts/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 22:58:14.605119 cliconfig-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-08 22:57:58.000000 cliconfig-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 22:58:14.601119 cliconfig-0.3.0/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/configs/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/test_build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-08 22:57:58.000000 cliconfig-0.3.0/tests/test_process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.709150 cliconfig-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.697150 cliconfig-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.701150 cliconfig-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-10 02:19:15.000000 cliconfig-0.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-10 02:19:15.000000 cliconfig-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 02:19:15.000000 cliconfig-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-10 02:19:33.709150 cliconfig-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-10 02:19:15.000000 cliconfig-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.701150 cliconfig-0.4.0/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 02:19:33.000000 cliconfig-0.4.0/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14687 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.701150 cliconfig-0.4.0/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-10 02:19:15.000000 cliconfig-0.4.0/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.701150 cliconfig-0.4.0/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-10 02:19:33.000000 cliconfig-0.4.0/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-05-10 02:19:33.000000 cliconfig-0.4.0/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 02:19:33.000000 cliconfig-0.4.0/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 02:19:33.000000 cliconfig-0.4.0/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 02:19:33.000000 cliconfig-0.4.0/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.705150 cliconfig-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/manipulate.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-10 02:19:15.000000 cliconfig-0.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.705150 cliconfig-0.4.0/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 02:19:15.000000 cliconfig-0.4.0/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-10 02:19:15.000000 cliconfig-0.4.0/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-10 02:19:15.000000 cliconfig-0.4.0/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 02:19:15.000000 cliconfig-0.4.0/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 02:19:15.000000 cliconfig-0.4.0/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.705150 cliconfig-0.4.0/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-10 02:19:15.000000 cliconfig-0.4.0/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-10 02:19:15.000000 cliconfig-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 02:19:15.000000 cliconfig-0.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 02:19:15.000000 cliconfig-0.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.705150 cliconfig-0.4.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-10 02:19:15.000000 cliconfig-0.4.0/scripts/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 02:19:33.709150 cliconfig-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 02:19:15.000000 cliconfig-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.705150 cliconfig-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.705150 cliconfig-0.4.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.705150 cliconfig-0.4.0/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 02:19:33.705150 cliconfig-0.4.0/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/test_build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-10 02:19:15.000000 cliconfig-0.4.0/tests/test_tag_routines.py
```

### Comparing `cliconfig-0.3.0/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.4.0/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/.github/workflows/pydocstyle.yaml` & `cliconfig-0.4.0/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/.github/workflows/pylint.yaml` & `cliconfig-0.4.0/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/.github/workflows/tests.yaml` & `cliconfig-0.4.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/.pylintrc` & `cliconfig-0.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/CONTRIBUTING.md` & `cliconfig-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/LICENSE` & `cliconfig-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/PKG-INFO` & `cliconfig-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.3.0
+Version: 0.4.0
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -169,25 +169,30 @@
 ```
 
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ### Todo
 
-To do:
+Priority:
 
-- [ ] log warning when `None` is used in CLI (considered as string a by PyYAML)
-
-Done:
-
-- [x] add `merge_config_file` to merge from path (= `merge_config` that includes
-  config loading)
-- [x] add `clean_pre_flat` to solve conflicting flatten and unflatten parameters
-  before flattening the config
-- [x] avoid changing keys order in merge_config
+- [ ] add a routine to check if a tag is in a key and robust to all other tags possible
+- [ ] add an integration test with all built-in processing (and more)
+- [ ] add `ProcessCleanTags` that raise en error when a tag is encountered in a key on
+  postmerge.
+
+Secondary:
+
+- [ ] add `make_processing_cond` to make a processing that ensure a condition on
+  a parameter across merged configs
+- [ ] add `make_processing_keep_status` to make a processing that keep the status of
+  a parameter across merged configs. The status can be any python object returned by
+  a function that takes the parameter as input
+- [ ] add `ProcessSelect` (with tag "@select") to select a subconfig (or parameter)
+  and delete the others configs at the same level (to clean the global config)
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.3.0/README.md` & `cliconfig-0.4.0/cliconfig.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: cliconfig
+Version: 0.4.0
+Summary: Merge your config files and set parameters from the command line in a simple way.
+Author-email: Valentin Goldite <valentin.goldite@gmail.com>
+Project-URL: Source, https://github.com/valentingol/cliconfig
+Keywords: logging,machine,learning
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CLI Config
 
 Lightweight library that provides routines to merge your configs (optionally nested)
 and set parameters from command line. It also prevents you from adding new parameters
 if not desired. Finally, it provides helper routines to manage flatten dicts, unflatten
 (= nested) dicts or a mix of both, save config, load, display, etc.
 
@@ -157,25 +169,30 @@
 ```
 
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ### Todo
 
-To do:
-
-- [ ] log warning when `None` is used in CLI (considered as string a by PyYAML)
-
-Done:
+Priority:
 
-- [x] add `merge_config_file` to merge from path (= `merge_config` that includes
-  config loading)
-- [x] add `clean_pre_flat` to solve conflicting flatten and unflatten parameters
-  before flattening the config
-- [x] avoid changing keys order in merge_config
+- [ ] add a routine to check if a tag is in a key and robust to all other tags possible
+- [ ] add an integration test with all built-in processing (and more)
+- [ ] add `ProcessCleanTags` that raise en error when a tag is encountered in a key on
+  postmerge.
+
+Secondary:
+
+- [ ] add `make_processing_cond` to make a processing that ensure a condition on
+  a parameter across merged configs
+- [ ] add `make_processing_keep_status` to make a processing that keep the status of
+  a parameter across merged configs. The status can be any python object returned by
+  a function that takes the parameter as input
+- [ ] add `ProcessSelect` (with tag "@select") to select a subconfig (or parameter)
+  and delete the others configs at the same level (to clean the global config)
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.3.0/cliconfig/__init__.py` & `cliconfig-0.4.0/cliconfig/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""CLI Config.
+"""CLI Config: build your configuration from CLI by merging with processing.
 
 Copyright (C) 2023  Valentin Goldité
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the MIT License.
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `cliconfig-0.3.0/cliconfig/build_config.py` & `cliconfig-0.4.0/cliconfig/build_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Functions to manipulate config as dict with yaml files and CLI."""
 import sys
 from typing import Any, Dict, List, Optional
 
 from cliconfig.cli_parser import parse_cli
 from cliconfig.dict_routines import unflatten
 from cliconfig.process_routines import (
-    Processing,
     load_processing,
     merge_flat_paths_processing,
     merge_flat_processing,
 )
+from cliconfig.processing.base import Processing
 
 
 def make_config(
     *default_config_paths: str,
     processing_list: Optional[List[Processing]] = None,
 ) -> Dict[str, Any]:
     r"""Make a config from default configs and CLI arguments and apply processing.
```

### Comparing `cliconfig-0.3.0/cliconfig/cli_parser.py` & `cliconfig-0.4.0/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/cliconfig/dict_routines.py` & `cliconfig-0.4.0/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/cliconfig/process_routines.py` & `cliconfig-0.4.0/cliconfig/process_routines.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,12 @@
 """Routines to manipulate dictionaries with processing."""
 from typing import Any, Dict, List, Union
 
 from cliconfig.dict_routines import _flat_before_merge, load_dict, merge_flat, save_dict
-
-
-class Processing():
-    """Processing base class."""
-
-    def __init__(self) -> None:
-        self.premerge_order = 0.0
-        self.postmerge_order = 0.0
-        self.presave_order = 0.0
-        self.postload_order = 0.0
-
-    # pylint: disable=unused-argument
-    def premerge(
-        self,
-        flat_dict: Dict[str, Any],
-        processing_list: list,  # noqa
-    ) -> Dict[str, Any]:
-        """Pre-merge processing.
-
-        Function that can be applied to the flat dict to modify it
-        before merging . It takes a flat dict and returns a flat dict.
-        """
-        return flat_dict
-
-    # pylint: disable=unused-argument
-    def postmerge(
-        self,
-        flat_dict: Dict[str, Any],
-        processing_list: list,  # noqa
-    ) -> Dict[str, Any]:
-        """Post-merge processing.
-
-        Function that can be applied to the flat dict to modify it
-        after merging . It takes a flat dict and returns a flat dict.
-        """
-        return flat_dict
-
-    # pylint: disable=unused-argument
-    def presave(
-        self,
-        flat_dict: Dict[str, Any],
-        processing_list: list,  # noqa
-    ) -> Dict[str, Any]:
-        """Pre-save processing.
-
-        Function applied to the flat dict to modify it before
-        saving it. It takes a flat dict and returns a flat dict.
-        """
-        return flat_dict
-
-    # pylint: disable=unused-argument
-    def postload(
-        self,
-        flat_dict: Dict[str, Any],
-        processing_list: list,  # noqa
-    ) -> Dict[str, Any]:
-        """Post-load processing.
-
-        Function applied to the flat dict to modify it after
-        loading it. It takes a flat dict and returns a flat dict.
-        """
-        return flat_dict
+from cliconfig.processing.base import Processing
 
 
 def merge_flat_processing(
     dict1: Dict[str, Any],
     dict2: Dict[str, Any],
     processing_list: List[Processing],
     *,
```

### Comparing `cliconfig-0.3.0/cliconfig/processings.py` & `cliconfig-0.4.0/cliconfig/processing/builtin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,201 +1,277 @@
-"""Example of useful processing classes.
+"""Built-in processing classes.
 
 Classes to apply pre-merge, post-merge, pre-save and post-load modifications
 to dict with processing routines (found in cliconfig.process_routines).
 """
+# pylint: disable=unused-argument
 from typing import Any, Dict
 
-from cliconfig.process_routines import Processing, merge_flat_paths_processing
+from cliconfig.process_routines import (
+    merge_flat_paths_processing,
+    merge_flat_processing,
+)
+from cliconfig.processing._type_parser import _parse_type
+from cliconfig.processing.base import Processing
+from cliconfig.tag_routines import clean_all_tags, clean_tag
 
 
 class ProcessMerge(Processing):
-    """Merge dict just in time with '@merge_after' and '@merge_before' tags.
+    """Merge dicts just in time with '@merge_after/_before/_add' tags.
 
-    Tag your key with '@merge_after' or '@merge_before' to load the dict
-    corresponding to a path and merge it just before or after the current
-    dicturation. The processing is a pre-merge processing only and occurs before
+    Tag your key with '@merge_after', '@merge_before' or @merge_add to load
+    the dict corresponding to the value (path) and merge it just before or after
+    the current dict.
+
+    * '@merge_add' merges the dict corresponding to the path by allowing ONLY new keys
+      It is a security check when you want to add a dict completely new
+      It is a typical usage for a default config splitted in several files.
+    * '@merge_after' merge the dict corresponding to the path on the current dict
+    * '@merge_before' merge the current dict on the dict corresponding to the path
+
+    The processing is a pre-merge processing only and occurs before
     most of the other processing.
     Pre-merge order: -20.0
 
     Examples
     --------
     .. code-block:: yaml
 
         --- # config1.yaml
         a:
           b: 1
           b_path@merge_after: dict2.yaml
         --- # config2.yaml
         a.b: 2
+        c_path@merge_add: config3.yaml
+        --- # config3.yaml
+        c: 3
+
+    Before merging, the config1 is interpreted as the dict:
+
+    .. code-block:: python
+
+        {'a': {'b': 2, 'b_path': 'config2.yaml'}, 'c_path': 'config3.yaml', 'c': 3}`
+
+    If you replace '@merge_after' by '@merge_before', it will be:
+
+    .. code-block:: python
 
-    Before merging, the config1 is interpreted as the dict
-    `{'a': {'b': 2, 'b_path': 'config2.yaml'}` If you replace '@merge_after'
-    by '@merge_before', it will be `{'a': {'b': 1, 'b_path': 'config2.yaml'}`
-    instead.
+        {'a': {'b': 1, 'b_path': 'config2.yaml'}, 'c_path': 'config3.yaml', 'c': 3}`
+
+    Finally, if you replace '@merge_after' by '@merge_add', it will raises an
+    error because the key 'a.b' already exists in the dict.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.premerge_order = -20.0
 
     def premerge(
         self,
         flat_dict: Dict[str, Any],
         processing_list: list,
     ) -> Dict[str, Any]:
         """Pre-merge processing."""
         items = list(flat_dict.items())
         for flat_key, val in items:
-            if flat_key.endswith('@merge_after'):
-                # NOTE: we allow new keys here fore more flexibility but we note that
-                # the merge following this pre-merge will avoid the creation of
-                # new keys if needed.
+            end_key = flat_key.split('.')[-1]
+            if "@merge_after" in end_key:
                 if not isinstance(val, str) or not val.endswith('.yaml'):
                     raise ValueError(
                         "Key with '@merge_after' tag must be associated "
                         "to a string corresponding to a *yaml* file."
                         f"The problem occurs at key: {flat_key}"
                     )
                 # Remove the tag in the dict
-                flat_dict[flat_key[:-len('@merge_after')]] = val
                 del flat_dict[flat_key]
+                flat_dict[clean_tag(flat_key, 'merge_after')] = val
                 # Merge + process the dicts
+                # NOTE: we allow new keys with security because the merge
+                # following this pre-merge will avoid the creation of
+                # new keys if needed.
                 flat_dict = merge_flat_paths_processing(
                     flat_dict,
                     val,
                     processing_list=processing_list,
                     allow_new_keys=True,
                     preprocess_first=False,  # Already processed
                 )
-            if flat_key.endswith('@merge_before'):
-                # NOTE: we allow new keys here fore more flexibility but we note that
-                # the merge following this pre-merge will avoid the creation of
-                # new keys if needed.
+            elif "@merge_before" in end_key:
                 if not isinstance(val, str) or not val.endswith('.yaml'):
                     raise ValueError(
                         "Key with '@merge_before' tag must be associated "
                         "to a string corresponding to a *yaml* file."
                         f"The problem occurs at key: {flat_key}"
                     )
-                # Remove the tag in the key
-                flat_dict[flat_key[:-len('@merge_before')]] = val
+                # Remove the tag in the dict
                 del flat_dict[flat_key]
+                flat_dict[clean_tag(flat_key, 'merge_before')] = val
                 # Merge + process the dicts
                 flat_dict = merge_flat_paths_processing(
                     val,
                     flat_dict,
                     processing_list=processing_list,
                     allow_new_keys=True,
                     preprocess_second=False,  # Already processed
                 )
+            elif "@merge_add" in end_key:
+                if not isinstance(val, str) or not val.endswith('.yaml'):
+                    raise ValueError(
+                        "Key with '@merge_add' tag must be associated "
+                        "to a string corresponding to a *yaml* file."
+                        f"The problem occurs at key: {flat_key}"
+                    )
+                # Remove the tag in the dict
+                del flat_dict[flat_key]
+                flat_dict[clean_tag(flat_key, 'merge_add')] = val
+                # Pre-merge process the dict
+                flat_dict_to_merge = merge_flat_paths_processing(
+                    {},
+                    val,
+                    processing_list=processing_list,
+                    allow_new_keys=True,
+                    preprocess_first=False,  # Already processed
+                    postprocess=False,
+                )
+                for key in flat_dict_to_merge:
+                    if key in flat_dict:
+                        raise ValueError(
+                            f"@merge_add doest not allow to add already "
+                            f"existing keys but key '{key}' is found in both "
+                            "dicts. Use @merge_after or @merge_before if you "
+                            "want to merge this key, or check your key names."
+                        )
+                # Merge the dicts (order is not important by construction)
+                flat_dict = merge_flat_processing(
+                    flat_dict,
+                    flat_dict_to_merge,
+                    processing_list=processing_list,
+                    allow_new_keys=True,
+                    preprocess_first=False,  # Already processed
+                    preprocess_second=False,  # Already processed
+                    postprocess=True,
+                )
         return flat_dict
 
 
 class ProcessCopy(Processing):
     """Copy a value with '@copy' tag.
 
     Tag your key with '@copy' and with value the name of the flat key to copy.
     This processing is a pre-merge processing only and occurs after most of
     the other pre-merge processing.
-    Pre-merge order: 20.0
+    Pre-merge order: 10.0
 
     Examples
     --------
     .. code-block:: yaml
 
         # config.yaml
         a:
           b: 1
           c@copy: a.b
 
     Before merging, the config is interpreted as the dict
-    `{'a': {'b': 1, 'c': 1}}`.
+
+    .. code-block:: python
+
+        {'a': {'b': 1, 'c': 1}}
     """
 
     def __init__(self) -> None:
         super().__init__()
-        self.premerge_order = 20.0
+        self.premerge_order = 10.0
 
-    # pylint: disable=unused-argument
     def premerge(
         self,
         flat_dict: Dict[str, Any],
         processing_list: list,  # noqa
     ) -> Dict[str, Any]:
         """Pre-merge processing."""
         items = list(flat_dict.items())
         for flat_key, val in items:
-            if flat_key.endswith('@copy'):
-                if not isinstance(val, str):
+            key = flat_key.split(".")[-1]
+            if "@copy" in key:
+                if not isinstance(val, str) or val not in flat_dict:
                     raise ValueError(
                         "Key with '@copy' tag must be associated "
-                        "to a string corresponding to a flat key."
-                        f"The problem occurs at key: {flat_key}"
+                        "to a string corresponding to an existing flat key. "
+                        f"The problem occurs at key: {flat_key} with value: {val}"
                     )
                 # Remove the tag and update the dict
-                flat_dict[flat_key[:-len('@copy')]] = flat_dict[val]
+                flat_dict[clean_tag(flat_key, "copy")] = flat_dict[val]
                 del flat_dict[flat_key]
         return flat_dict
 
 
-class ProcessProtect(Processing):
-    """Make a value protected with '@protect' tag.
+class ProcessTyping(Processing):
+    """Force a type with '@type:mytype' tag. The type is preserved forever.
 
-    The protected value cannot be changed on merge as long as this processing
-    is used. Otherwise, it raises an error. This processing store protected
-    keys and values and remove the '@protect' tag. It always occurs before anything
-    else on pre-merge processing and after everything else on post-merge.
-    Pre-merge order: -40.0
-    Post-merge order: 40.0
+    Allow basic types (none, any, bool, int, float, str, list, dict), nested lists,
+    nested dicts, unions (with Union or the '|' symbol) and Optional.
+    It checks and store the type in premerge and check alls forced types on postmerge.
+    It always occurs last in premerge and postmerge.
+    Pre-merge order: 20.0
+    Post-merge order: 20.0
     """
 
     def __init__(self) -> None:
         super().__init__()
-        self.premerge_order = -40.0
-        self.postmerge_order = 40.0
-        self.protected_dict: Dict[str, Any] = {}
+        self.premerge_order = 20.0
+        self.postmerge_order = 20.0
+        self.forced_types: Dict[str, tuple] = {}
+        self.type_desc: Dict[str, str] = {}  # For error messages
 
-    # pylint: disable=unused-argument
     def premerge(
         self,
         flat_dict: Dict[str, Any],
-        processing_list: list,  # noqa
+        processing_list: list,  # noqa: ARG002
     ) -> Dict[str, Any]:
         """Pre-merge processing."""
         items = list(flat_dict.items())
         for flat_key, val in items:
-            if flat_key.endswith('@protect'):
-                new_key = flat_key[:-len('@protect')]
-                if new_key in flat_dict and self.protected_dict[new_key] != val:
-                    raise ValueError(
-                        f"Attempt to change a protected key (tagged by '@protect'): "
-                        f"{new_key}. Protected value: {self.protected_dict[new_key]}, "
-                        f"new value: {val}."
+            end_key = flat_key.split('.')[-1]
+            if "@type:" in end_key:
+                # Get the type description
+                trail = end_key.split("@type:")[-1]
+                type_desc = trail.split('@')[0]  # (in case of multiple tags)
+                expected_type = tuple(_parse_type(type_desc))
+                clean_key = clean_all_tags(flat_key)
+                if (clean_key in self.forced_types
+                        and set(self.forced_types[clean_key]) != set(expected_type)):
+                    raise ValueError(
+                        f"Find the tag '@type:{type_desc}' on a key that has already "
+                        "been associated to an other type: "
+                        f"{self.type_desc[clean_key]}. "
+                        f"Find problem at key: {flat_key}"
                     )
-                # Remove the tag in the key
-                flat_dict[new_key] = val
+                if not isinstance(val, expected_type):
+                    raise ValueError(
+                        f"Key with '@type:{type_desc}' tag must be associated "
+                        f"to a value of type {type_desc}. Find the value: {val} "
+                        f"at key: {flat_key}"
+                    )
+                # Remove the tag
                 del flat_dict[flat_key]
-                # Store the protected key and value
-                self.protected_dict[flat_key[:-len('@protect')]] = val
+                flat_dict[clean_tag(flat_key, f'type:{type_desc}')] = val
+                # Add the forced type
+                self.forced_types[clean_key] = expected_type
+                self.type_desc[clean_key] = type_desc
         return flat_dict
 
-    # pylint: disable=unused-argument
     def postmerge(
         self,
         flat_dict: Dict[str, Any],
-        processing_list: list,  # noqa
+        processing_list: list,  # noqa: ARG002
     ) -> Dict[str, Any]:
         """Post-merge processing."""
-        for key, val in self.protected_dict.items():
-            if key not in flat_dict:
-                raise ValueError(
-                    f"Protected key (tagged by '@protect') {key} has been removed "
-                    f"after merge. Protected value: {val}, new value: nothing."
-                )
-
-            if flat_dict[key] != val:
+        for key, expected_type in self.forced_types.items():
+            if key in flat_dict and not isinstance(flat_dict[key], expected_type):
+                type_desc = self.type_desc[key]
                 raise ValueError(
-                    f"Protected key (tagged by '@protect') {key} has been changed "
-                    f"after merge. Protected value: {val}, new value: {flat_dict[key]}."
+                    f"Key previously tagged with '@type:{type_desc}' must be "
+                    f"associated to a value of type {type_desc}. Find the "
+                    f"value: {flat_dict[key]} of type {type(flat_dict[key])} "
+                    f"at key: {key}"
                 )
         return flat_dict
```

### Comparing `cliconfig-0.3.0/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: cliconfig
-Version: 0.3.0
-Summary: Merge your config files and set parameters from the command line in a simple way.
-Author-email: Valentin Goldite <valentin.goldite@gmail.com>
-Project-URL: Source, https://github.com/valentingol/cliconfig
-Keywords: logging,machine,learning
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CLI Config
 
 Lightweight library that provides routines to merge your configs (optionally nested)
 and set parameters from command line. It also prevents you from adding new parameters
 if not desired. Finally, it provides helper routines to manage flatten dicts, unflatten
 (= nested) dicts or a mix of both, save config, load, display, etc.
 
@@ -169,25 +157,30 @@
 ```
 
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ### Todo
 
-To do:
-
-- [ ] log warning when `None` is used in CLI (considered as string a by PyYAML)
-
-Done:
+Priority:
 
-- [x] add `merge_config_file` to merge from path (= `merge_config` that includes
-  config loading)
-- [x] add `clean_pre_flat` to solve conflicting flatten and unflatten parameters
-  before flattening the config
-- [x] avoid changing keys order in merge_config
+- [ ] add a routine to check if a tag is in a key and robust to all other tags possible
+- [ ] add an integration test with all built-in processing (and more)
+- [ ] add `ProcessCleanTags` that raise en error when a tag is encountered in a key on
+  postmerge.
+
+Secondary:
+
+- [ ] add `make_processing_cond` to make a processing that ensure a condition on
+  a parameter across merged configs
+- [ ] add `make_processing_keep_status` to make a processing that keep the status of
+  a parameter across merged configs. The status can be any python object returned by
+  a function that takes the parameter as input
+- [ ] add `ProcessSelect` (with tag "@select") to select a subconfig (or parameter)
+  and delete the others configs at the same level (to clean the global config)
 
 ## License
 
 Copyright (C) 2023  Valentin Goldité
 
 This program is free software: you can redistribute it and/or modify it under the
 terms of the [MIT License](LICENSE). This program is distributed in the hope that
```

### Comparing `cliconfig-0.3.0/docs/Makefile` & `cliconfig-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/docs/cliconfig_api.rst` & `cliconfig-0.4.0/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/docs/conf.py` & `cliconfig-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/docs/edge_cases.md` & `cliconfig-0.4.0/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/docs/index.rst` & `cliconfig-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/docs/license.md` & `cliconfig-0.4.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/docs/make.bat` & `cliconfig-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/docs/manipulate.md` & `cliconfig-0.4.0/docs/manipulate.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/docs/quickstart.md` & `cliconfig-0.4.0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.4.0/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/github_actions_utils/pylint_manager.py` & `cliconfig-0.4.0/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/github_actions_utils/pytest_manager.py` & `cliconfig-0.4.0/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.4.0/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/pyproject.toml` & `cliconfig-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/scripts/pre-commit-checks.sh` & `cliconfig-0.4.0/scripts/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/tests/conftest.py` & `cliconfig-0.4.0/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Shared pytest fixtures."""
 from typing import Any, Dict
 
 import pytest
 
-from cliconfig.process_routines import Processing
+from cliconfig.processing.base import Processing
 
 
 class ProcessAdd1(Processing):
-    """Add 1 to values with tag "@add+1"."""
+    """Add 1 to values with tag "@add1"."""
 
     # pylint: disable=unused-argument
     def premerge(
         self,
         flat_dict: Dict[str, Any],
         processing_list: list,  # noqa
     ) -> Dict[str, Any]:
         """Pre-merge processing."""
         items = list(flat_dict.items())
         for key, value in items:
-            if key.endswith("@add+1"):
-                flat_dict[key[:-6]] = value + 1
+            if key.endswith("@add1"):
+                flat_dict[key[:-5]] = value + 1
                 del flat_dict[key]
         return flat_dict
 
     def presave(
         self,
         flat_dict: Dict[str, Any],
         processing_list: list
@@ -55,15 +55,15 @@
                 self.keep_vals[new_key] = value
         return flat_dict
 
     # pylint: disable=unused-argument
     def postmerge(
         self,
         flat_dict: Dict[str, Any],
-        processing_list: list, # noqa
+        processing_list: list,  # noqa
     ) -> Dict[str, Any]:
         """Post-merge processing."""
         for key, value in self.keep_vals.items():
             flat_dict[key] = value
         self.keep_vals = {}
         return flat_dict
 
@@ -78,15 +78,15 @@
             flat_dict[key] = value
         self.keep_vals = {}
         return flat_dict
 
 
 @pytest.fixture()
 def process_add1() -> ProcessAdd1:
-    """Return a processing object that adds 1 on tag "@add+1"."""
+    """Return a processing object that adds 1 on tag "@add1"."""
     return ProcessAdd1()
 
 
 @pytest.fixture()
 def process_keep() -> ProcessKeep:
     """Return a processing object that keep a value unchanged after the merge."""
     return ProcessKeep()
```

### Comparing `cliconfig-0.3.0/tests/test_build_config.py` & `cliconfig-0.4.0/tests/test_build_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/tests/test_cli_parser.py` & `cliconfig-0.4.0/tests/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/tests/test_dict_routines.py` & `cliconfig-0.4.0/tests/test_dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.3.0/tests/test_process_routines.py` & `cliconfig-0.4.0/tests/test_process_routines.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Tests for dict routines with preprocessing."""
 import shutil
 
 import pytest_check as check
 import yaml
 
 from cliconfig.process_routines import (
-    Processing,
     load_processing,
     merge_flat_paths_processing,
     merge_flat_processing,
     save_processing,
 )
+from cliconfig.processing.base import Processing
 from tests.conftest import ProcessAdd1, ProcessKeep
 
 
 def test_processing() -> None:
     """Test Processing."""
     in_dict = {"a.b": 1, "b": 2, "c.d.e": 3, "c.d.f": [2, 3]}
     base_process = Processing()
@@ -31,15 +31,15 @@
 
 def test_merge_flat_processing(
     process_add1: ProcessAdd1,
     process_keep: ProcessKeep,
 ) -> None:
     """Test merge_flat_processing."""
     dict1 = {"a": {"b": 1, "c": 2, "d@keep": 3}}
-    dict2 = {"a": {"b": 2, "c@add+1": 3, "d": 4}}
+    dict2 = {"a": {"b": 2, "c@add1": 3, "d": 4}}
     flat_dict = merge_flat_processing(
         dict1,
         dict2,
         processing_list=[process_add1, process_keep],
         allow_new_keys=False,
     )
     check.equal(
@@ -50,15 +50,15 @@
 
 
 def test_merge_flat_paths_processing(
     process_add1: ProcessAdd1,
     process_keep: ProcessKeep,
 ) -> None:
     """Test merge_flat_paths_processing."""
-    dict1 = {"param1@add+1": 0, "param2.param3@keep": 1}
+    dict1 = {"param1@add1": 0, "param2.param3@keep": 1}
     dict2 = {"param2.param3": 3}
     expected_dict = {"param1": 1, "param2.param3": 1}
     check.equal(
         merge_flat_paths_processing(
             "tests/configs/configtag1.yaml",
             "tests/configs/configtag2.yaml",
             [process_add1, process_keep],
@@ -79,15 +79,15 @@
 
 
 def test_save_processing(
     process_add1: ProcessAdd1,
     process_keep: ProcessKeep,
 ) -> None:
     """Test save_processing."""
-    in_dict = {"param1@add+1": 0, "param2.param3@add+1": 1}
+    in_dict = {"param1@add1": 0, "param2.param3@add1": 1}
     save_processing(in_dict, "tests/tmp/config.yaml", [process_add1, process_keep])
     with open("tests/tmp/config.yaml", "r", encoding="utf-8") as yaml_file:
         loaded_dict = yaml.safe_load(yaml_file)
     check.equal(loaded_dict, {"param1": 1, "param2.param3": 2})
     check.equal(process_keep.keep_vals, {})
     shutil.rmtree("tests/tmp")
```

