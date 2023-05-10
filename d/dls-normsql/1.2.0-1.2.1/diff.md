# Comparing `tmp/dls-normsql-1.2.0.tar.gz` & `tmp/dls-normsql-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-normsql-1.2.0.tar", last modified: Sun May  7 04:47:35 2023, max compression
+gzip compressed data, was "dls-normsql-1.2.1.tar", last modified: Tue May  9 12:59:55 2023, max compression
```

## Comparing `dls-normsql-1.2.0.tar` & `dls-normsql-1.2.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.764743 dls-normsql-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.752743 dls-normsql-1.2.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-07 04:47:35.760743 dls-normsql-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.752743 dls-normsql-1.2.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.756743 dls-normsql-1.2.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.760743 dls-normsql-1.2.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.760743 dls-normsql-1.2.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 04:47:35.764743 dls-normsql-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.752743 dls-normsql-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.760743 dls-normsql-1.2.0/src/dls_normsql/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/src/dls_normsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/src/dls_normsql/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-07 04:47:35.000000 dls-normsql-1.2.0/src/dls_normsql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/src/dls_normsql/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/src/dls_normsql/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/src/dls_normsql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/src/dls_normsql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/src/dls_normsql/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/src/dls_normsql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.760743 dls-normsql-1.2.0/src/dls_normsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-07 04:47:35.000000 dls-normsql-1.2.0/src/dls_normsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 04:47:35.000000 dls-normsql-1.2.0/src/dls_normsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 04:47:35.000000 dls-normsql-1.2.0/src/dls_normsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 04:47:35.000000 dls-normsql-1.2.0/src/dls_normsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 04:47:35.000000 dls-normsql-1.2.0/src/dls_normsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 04:47:35.000000 dls-normsql-1.2.0/src/dls_normsql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:35.760743 dls-normsql-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/tests/my_table_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/tests/test_backup_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-07 04:47:25.000000 dls-normsql-1.2.0/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.222048 dls-normsql-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.214048 dls-normsql-1.2.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.214048 dls-normsql-1.2.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.214048 dls-normsql-1.2.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.214048 dls-normsql-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.214048 dls-normsql-1.2.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.214048 dls-normsql-1.2.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.218048 dls-normsql-1.2.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.218048 dls-normsql-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.218048 dls-normsql-1.2.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-09 12:59:55.222048 dls-normsql-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.218048 dls-normsql-1.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.214048 dls-normsql-1.2.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.218048 dls-normsql-1.2.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.218048 dls-normsql-1.2.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.218048 dls-normsql-1.2.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 12:59:55.222048 dls-normsql-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.214048 dls-normsql-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.218048 dls-normsql-1.2.1/src/dls_normsql/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/src/dls_normsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/src/dls_normsql/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-09 12:59:55.000000 dls-normsql-1.2.1/src/dls_normsql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21378 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/src/dls_normsql/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/src/dls_normsql/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/src/dls_normsql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/src/dls_normsql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/src/dls_normsql/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/src/dls_normsql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.222048 dls-normsql-1.2.1/src/dls_normsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-05-09 12:59:55.000000 dls-normsql-1.2.1/src/dls_normsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-09 12:59:55.000000 dls-normsql-1.2.1/src/dls_normsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 12:59:55.000000 dls-normsql-1.2.1/src/dls_normsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-09 12:59:55.000000 dls-normsql-1.2.1/src/dls_normsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-09 12:59:55.000000 dls-normsql-1.2.1/src/dls_normsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 12:59:55.000000 dls-normsql-1.2.1/src/dls_normsql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:55.222048 dls-normsql-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/tests/my_table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/tests/test_backup_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-09 12:59:45.000000 dls-normsql-1.2.1/tests/test_database.py
```

### Comparing `dls-normsql-1.2.0/.dae-devops/Makefile` & `dls-normsql-1.2.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.dae-devops/docs/conventions.rst` & `dls-normsql-1.2.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.dae-devops/docs/developing.rst` & `dls-normsql-1.2.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.dae-devops/docs/devops.rst` & `dls-normsql-1.2.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.dae-devops/docs/docs_structure.rst` & `dls-normsql-1.2.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.dae-devops/docs/installing.rst` & `dls-normsql-1.2.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.dae-devops/docs/testing.rst` & `dls-normsql-1.2.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.devcontainer/Dockerfile` & `dls-normsql-1.2.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.devcontainer/devcontainer.json` & `dls-normsql-1.2.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.github/CONTRIBUTING.rst` & `dls-normsql-1.2.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.github/actions/install_requirements/action.yml` & `dls-normsql-1.2.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.github/dependabot.yml` & `dls-normsql-1.2.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.github/pages/make_switcher.py` & `dls-normsql-1.2.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.github/workflows/code.yml` & `dls-normsql-1.2.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.github/workflows/docs.yml` & `dls-normsql-1.2.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.github/workflows/docs_clean.yml` & `dls-normsql-1.2.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.github/workflows/linkcheck.yml` & `dls-normsql-1.2.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.gitignore` & `dls-normsql-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.gitlab-ci.yml` & `dls-normsql-1.2.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/.vscode/launch.json` & `dls-normsql-1.2.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/LICENSE` & `dls-normsql-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/PKG-INFO` & `dls-normsql-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 1.2.0
+Version: 1.2.1
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-1.2.0/README.rst` & `dls-normsql-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/docs/conf.py` & `dls-normsql-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/docs/images/dls-favicon.ico` & `dls-normsql-1.2.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/docs/images/dls-logo.svg` & `dls-normsql-1.2.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/pyproject.toml` & `dls-normsql-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/src/dls_normsql/__main__.py` & `dls-normsql-1.2.1/src/dls_normsql/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/src/dls_normsql/aiosqlite.py` & `dls-normsql-1.2.1/src/dls_normsql/aiosqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
                     Tablenames.REVISION, [{"number": self.LATEST_REVISION}]
                 )
                 # TODO: Set permission on sqlite file from configuration.
                 os.chmod(self.__filename, 0o666)
 
             # Emit the name of the database file for positive confirmation on console.
             logger.info(
-                f"{callsign(self)} database file is {self.__filename} revision {self.LATEST_REVISION}"
+                f"{callsign(self)} database file is {self.__filename} code revision {self.LATEST_REVISION}"
             )
 
     # ----------------------------------------------------------------------------------------
     async def apply_revisions(self):
         """
         Apply revision updates to databse if needed.
         """
@@ -144,15 +144,15 @@
                     f"could not get revision, presuming legacy database with no table: {exception}"
                 )
                 old_revision = 0
 
             if old_revision < self.LATEST_REVISION:
                 # Backup before applying revisions.
                 logger.debug(
-                    f"[BKREVL] backing up before updating to revision {self.LATEST_REVISION}"
+                    f"[BKREVL] backing up before updating from revision {old_revision} to revision {self.LATEST_REVISION}"
                 )
 
                 await self.backup()
 
                 for revision in range(old_revision, self.LATEST_REVISION):
                     logger.debug(f"updating to revision {revision+1}")
                     await self.apply_revision(revision + 1)
@@ -160,16 +160,16 @@
                     Tablenames.REVISION,
                     {"number": self.LATEST_REVISION},
                     "1 = 1",
                     why="update database revision",
                 )
             else:
                 logger.debug(
-                    f"[BKREVL] no need to update old revision {old_revision}"
-                    f" which matches latest revision {self.LATEST_REVISION}"
+                    f"[BKREVL] no need to update persistent revision {old_revision}"
+                    f" which matches code revision {self.LATEST_REVISION}"
                 )
 
     # ----------------------------------------------------------------------------------------
     async def apply_revision(self, revision):
         logger.debug(f"updating to revision {revision}")
         # Updating to revision 1 presumably means
         # this is a legacy database with no revision table in it.
```

### Comparing `dls-normsql-1.2.0/src/dls_normsql/constants.py` & `dls-normsql-1.2.1/src/dls_normsql/constants.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/src/dls_normsql/databases.py` & `dls-normsql-1.2.1/src/dls_normsql/databases.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/src/dls_normsql/version.py` & `dls-normsql-1.2.1/src/dls_normsql/version.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/src/dls_normsql.egg-info/PKG-INFO` & `dls-normsql-1.2.1/src/dls_normsql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-normsql
-Version: 1.2.0
+Version: 1.2.1
 Summary: Normalized API over various sql libraries.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-normsql-1.2.0/src/dls_normsql.egg-info/SOURCES.txt` & `dls-normsql-1.2.1/src/dls_normsql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/tests/base_tester.py` & `dls-normsql-1.2.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/tests/conftest.py` & `dls-normsql-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/tests/my_table_definition.py` & `dls-normsql-1.2.1/tests/my_table_definition.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/tests/test_backup_restore.py` & `dls-normsql-1.2.1/tests/test_backup_restore.py`

 * *Files identical despite different names*

### Comparing `dls-normsql-1.2.0/tests/test_database.py` & `dls-normsql-1.2.1/tests/test_database.py`

 * *Files identical despite different names*

