# Comparing `tmp/pytest-ansible-3.1.0.tar.gz` & `tmp/pytest-ansible-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-ansible-3.1.0.tar", last modified: Fri May  5 12:19:50 2023, max compression
+gzip compressed data, was "pytest-ansible-3.1.2.tar", last modified: Wed May 10 15:13:49 2023, max compression
```

## Comparing `pytest-ansible-3.1.0.tar` & `pytest-ansible-3.1.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.306345 pytest-ansible-3.1.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.306345 pytest-ansible-3.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.310345 pytest-ansible-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.310345 pytest-ansible-3.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/inventory
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.294345 pytest-ansible-3.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.314345 pytest-ansible-3.1.0/src/pytest_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/has_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.322345 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v29.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.326346 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v212.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v213.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v24.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v28.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v29.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/src/pytest_ansible/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.318345 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 12:19:50.000000 pytest-ansible-3.1.0/src/pytest_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_adhoc_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_host_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_module_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_module_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/test_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:19:50.330346 pytest-ansible-3.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tests/unit/test_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-05 12:19:31.000000 pytest-ansible-3.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.899414 pytest-ansible-3.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.887413 pytest-ansible-3.1.2/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.config/requirements-lock.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.config/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.891414 pytest-ansible-3.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.891414 pytest-ansible-3.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.891414 pytest-ansible-3.1.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-05-10 15:13:49.899414 pytest-ansible-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12923 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/inventory
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:13:49.899414 pytest-ansible-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.887413 pytest-ansible-3.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.891414 pytest-ansible-3.1.2/src/pytest_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 15:13:49.000000 pytest-ansible-3.1.2/src/pytest_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/has_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.895413 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v29.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.895413 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v212.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v24.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v28.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v29.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/src/pytest_ansible/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.891414 pytest-ansible-3.1.2/src/pytest_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-05-10 15:13:49.000000 pytest-ansible-3.1.2/src/pytest_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-10 15:13:49.000000 pytest-ansible-3.1.2/src/pytest_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:13:49.000000 pytest-ansible-3.1.2/src/pytest_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 15:13:49.000000 pytest-ansible-3.1.2/src/pytest_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-10 15:13:49.000000 pytest-ansible-3.1.2/src/pytest_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:13:49.000000 pytest-ansible-3.1.2/src/pytest_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.895413 pytest-ansible-3.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10102 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/test_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/test_adhoc_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/test_host_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/test_module_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/test_module_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/test_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:13:49.899414 pytest-ansible-3.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tests/unit/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-10 15:13:34.000000 pytest-ansible-3.1.2/tox.ini
```

### Comparing `pytest-ansible-3.1.0/.config/requirements-lock.txt` & `pytest-ansible-3.1.2/.config/requirements-lock.txt`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/.config/requirements.txt` & `pytest-ansible-3.1.2/.config/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --extra=docs --extra=test --no-annotate --output-file=.config/requirements.txt --resolver=backtracking --strip-extras --unsafe-package=ruamel-yaml-clib pyproject.toml
 #
-ansible-core==2.14.3
+ansible-core==2.13.9
 attrs==22.2.0
 cffi==1.15.1
 coverage==7.2.2
 cryptography==40.0.1
 exceptiongroup==1.1.1
 iniconfig==2.0.0
 jinja2==3.1.2
```

### Comparing `pytest-ansible-3.1.0/.flake8` & `pytest-ansible-3.1.2/.flake8`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/.github/workflows/release.yml` & `pytest-ansible-3.1.2/.github/workflows/release.yml`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     types: [published]
 
 jobs:
   pypi:
     name: Publish to PyPI registry
     environment: release
     runs-on: ubuntu-22.04
+    permissions:
+      id-token: write
 
     env:
       FORCE_COLOR: 1
       PY_COLORS: 1
       TOXENV: pkg
 
     steps:
@@ -35,9 +37,7 @@
       - name: Build dists
         run: python -m tox
 
       - name: Publish to pypi.org
         if: >- # "create" workflows run separately from "push" & "pull_request"
           github.event_name == 'release'
         uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          password: ${{ secrets.pypi_password }}
```

### Comparing `pytest-ansible-3.1.0/.github/workflows/tox.yml` & `pytest-ansible-3.1.2/.github/workflows/tox.yml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     outputs:
       matrix: ${{ steps.generate_matrix.outputs.matrix }}
     steps:
       - name: Determine matrix
         id: generate_matrix
         uses: coactions/dynamic-matrix@v1
         with:
-          min_python: "3.9"
+          min_python: "3.8"
           max_python: "3.11"
           other_names: |
             lint
             pkg
             devel
           platforms: linux
```

### Comparing `pytest-ansible-3.1.0/.gitignore` & `pytest-ansible-3.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/.pre-commit-config.yaml` & `pytest-ansible-3.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/HISTORY.md` & `pytest-ansible-3.1.2/HISTORY.md`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/LICENSE` & `pytest-ansible-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/PKG-INFO` & `pytest-ansible-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.1.0
+Version: 3.1.2
 Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
@@ -15,18 +15,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lock
 License-File: LICENSE
 
 # pytest-ansible
```

### Comparing `pytest-ansible-3.1.0/README.md` & `pytest-ansible-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/inventory` & `pytest-ansible-3.1.2/inventory`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/pyproject.toml` & `pytest-ansible-3.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "setuptools_scm[toml] >= 7.0.5", # required for "no-local-version" scheme
 
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 # https://peps.python.org/pep-0621/#readme
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 dynamic = ["version", "dependencies", "optional-dependencies"]
 name = "pytest-ansible"
 description = "Plugin for pytest to simplify calling ansible modules from tests or fixtures"
 readme = "README.md"
 authors = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 maintainers = [{ "name" = "Ansible by Red Hat", "email" = "info@ansible.com" }]
 license = { text = "MIT" }
@@ -22,14 +22,15 @@
   'License :: OSI Approved :: MIT License',
   'Operating System :: OS Independent',
   'Topic :: Software Development :: Testing',
   'Topic :: Software Development :: Quality Assurance',
   'Topic :: Utilities',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3',
+  'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
   'Programming Language :: Python :: 3.11',
 ]
 keywords = ["ansible", "testing", "pytest"]
 
 [project.entry-points.pytest11]
@@ -128,15 +129,15 @@
   "S",
   "SLF",
   "T",
   "TRY",
   "PTH",
   "TCH",
 ]
-target-version = "py39"
+target-version = "py38"
 # Same as Black.
 line-length = 88
 
 [tool.ruff.flake8-pytest-style]
 parametrize-values-type = "tuple"
 
 [tool.ruff.per-file-ignores]
```

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/errors.py` & `pytest-ansible-3.1.2/src/pytest_ansible/errors.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/fixtures.py` & `pytest-ansible-3.1.2/src/pytest_ansible/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/has_version.py` & `pytest-ansible-3.1.2/src/pytest_ansible/has_version.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/__init__.py` & `pytest-ansible-3.1.2/src/pytest_ansible/host_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v1.py` & `pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v1.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v2.py` & `pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v2.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v212.py` & `pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v212.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v213.py` & `pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v213.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v24.py` & `pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v24.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v28.py` & `pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v28.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/host_manager/v29.py` & `pytest-ansible-3.1.2/src/pytest_ansible/host_manager/v29.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/__init__.py` & `pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Define BaseModuleDispatcher class."""
 
-from collections.abc import Sequence
+from typing import Sequence
 
 from pytest_ansible.errors import AnsibleModuleError
 
 
 class BaseModuleDispatcher:
     """Fixme.."""
```

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v1.py` & `pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v1.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v2.py` & `pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v2.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v212.py` & `pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v212.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v213.py` & `pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v213.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v24.py` & `pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v24.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v28.py` & `pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v28.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/module_dispatcher/v29.py` & `pytest-ansible-3.1.2/src/pytest_ansible/module_dispatcher/v29.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/plugin.py` & `pytest-ansible-3.1.2/src/pytest_ansible/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/results.py` & `pytest-ansible-3.1.2/src/pytest_ansible/results.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible/units.py` & `pytest-ansible-3.1.2/src/pytest_ansible/units.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible.egg-info/PKG-INFO` & `pytest-ansible-3.1.2/src/pytest_ansible.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ansible
-Version: 3.1.0
+Version: 3.1.2
 Summary: Plugin for pytest to simplify calling ansible modules from tests or fixtures
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/pytest-ansible
 Project-URL: documentation, https://github.com/ansible-community/pytest-ansible
 Project-URL: repository, https://github.com/ansible-community/pytest-ansible
@@ -15,18 +15,19 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lock
 License-File: LICENSE
 
 # pytest-ansible
```

### Comparing `pytest-ansible-3.1.0/src/pytest_ansible.egg-info/SOURCES.txt` & `pytest-ansible-3.1.2/src/pytest_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/conftest.py` & `pytest-ansible-3.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/test_adhoc.py` & `pytest-ansible-3.1.2/tests/test_adhoc.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/test_adhoc_result.py` & `pytest-ansible-3.1.2/tests/test_adhoc_result.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/test_fixtures.py` & `pytest-ansible-3.1.2/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/test_host_manager.py` & `pytest-ansible-3.1.2/tests/test_host_manager.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/test_module_dispatcher.py` & `pytest-ansible-3.1.2/tests/test_module_dispatcher.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/test_module_result.py` & `pytest-ansible-3.1.2/tests/test_module_result.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/test_params.py` & `pytest-ansible-3.1.2/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `pytest-ansible-3.1.0/tests/unit/test_unit.py` & `pytest-ansible-3.1.2/tests/unit/test_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests specific to the unit test functionality."""
 
+from __future__ import annotations
 
 import logging
 import re
 import subprocess
 import sys
 from pathlib import Path
```

### Comparing `pytest-ansible-3.1.0/tox.ini` & `pytest-ansible-3.1.2/tox.ini`

 * *Files identical despite different names*

