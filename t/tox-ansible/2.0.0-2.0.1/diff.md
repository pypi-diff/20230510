# Comparing `tmp/tox-ansible-2.0.0.tar.gz` & `tmp/tox-ansible-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-ansible-2.0.0.tar", last modified: Wed May 10 16:25:50 2023, max compression
+gzip compressed data, was "tox-ansible-2.0.1.tar", last modified: Wed May 10 18:00:07 2023, max compression
```

## Comparing `tox-ansible-2.0.0.tar` & `tox-ansible-2.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.180768 tox-ansible-2.0.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.config/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.184768 tox-ansible-2.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.184768 tox-ansible-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/workflows/run.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.184768 tox-ansible-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/integration.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/sanity.ini
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/tox-ansible.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/unit.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.176768 tox-ansible-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.188768 tox-ansible-2.0.0/src/tox_ansible/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/src/tox_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/src/tox_ansible/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.188768 tox-ansible-2.0.0/src/tox_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.188768 tox-ansible-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.176768 tox-ansible-2.0.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.176768 tox-ansible-2.0.0/tests/fixtures/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.188768 tox-ansible-2.0.0/tests/fixtures/integration/test_basic/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/fixtures/integration/test_basic/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/fixtures/integration/test_basic/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/tests/fixtures/integration/test_user_provided/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/fixtures/integration/test_user_provided/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/fixtures/integration/test_user_provided/tox-ansible.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/integration/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/integration/test_user_provided.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.948205 tox-ansible-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.940204 tox-ansible-2.0.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.config/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.940204 tox-ansible-2.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.940204 tox-ansible-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.github/workflows/run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-10 18:00:07.948205 tox-ansible-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.944205 tox-ansible-2.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/docs/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/docs/integration.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/docs/sanity.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/docs/tox-ansible.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/docs/unit.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:00:07.948205 tox-ansible-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.936205 tox-ansible-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.944205 tox-ansible-2.0.1/src/tox_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/src/tox_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 18:00:07.000000 tox-ansible-2.0.1/src/tox_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16117 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/src/tox_ansible/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.944205 tox-ansible-2.0.1/src/tox_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-10 18:00:07.000000 tox-ansible-2.0.1/src/tox_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 18:00:07.000000 tox-ansible-2.0.1/src/tox_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:00:07.000000 tox-ansible-2.0.1/src/tox_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 18:00:07.000000 tox-ansible-2.0.1/src/tox_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-10 18:00:07.000000 tox-ansible-2.0.1/src/tox_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 18:00:07.000000 tox-ansible-2.0.1/src/tox_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.944205 tox-ansible-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.936205 tox-ansible-2.0.1/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.936205 tox-ansible-2.0.1/tests/fixtures/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.944205 tox-ansible-2.0.1/tests/fixtures/integration/test_basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/fixtures/integration/test_basic/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/fixtures/integration/test_basic/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.944205 tox-ansible-2.0.1/tests/fixtures/integration/test_user_provided/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/fixtures/integration/test_user_provided/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/fixtures/integration/test_user_provided/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:00:07.944205 tox-ansible-2.0.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/integration/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tests/integration/test_user_provided.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-10 17:59:52.000000 tox-ansible-2.0.1/tox.ini
```

### Comparing `tox-ansible-2.0.0/.flake8` & `tox-ansible-2.0.1/.flake8`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/.github/workflows/release.yml` & `tox-ansible-2.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/.github/workflows/run.yml` & `tox-ansible-2.0.1/.github/workflows/run.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/.github/workflows/tox.yml` & `tox-ansible-2.0.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/.gitignore` & `tox-ansible-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/.pre-commit-config.yaml` & `tox-ansible-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/LICENSE` & `tox-ansible-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/PKG-INFO` & `tox-ansible-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.0
+Version: 2.0.1
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tox-ansible-2.0.0/README.md` & `tox-ansible-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/cspell.config.yaml` & `tox-ansible-2.0.1/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/docs/galaxy.yml` & `tox-ansible-2.0.1/docs/galaxy.yml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/docs/integration.ini` & `tox-ansible-2.0.1/docs/integration.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/docs/sanity.ini` & `tox-ansible-2.0.1/docs/sanity.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/docs/unit.ini` & `tox-ansible-2.0.1/docs/unit.ini`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/pyproject.toml` & `tox-ansible-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/requirements.txt` & `tox-ansible-2.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/src/tox_ansible/plugin.py` & `tox-ansible-2.0.1/src/tox_ansible/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 {integration, sanity, unit}-py3.10-{2.12, 2.13, 2.14, milestone, devel}
 {integration, sanity, unit}-py3.11-{2.14, milestone, devel}
 """
 TOX_WORK_DIR = Path()
 OUR_DEPS = [
     "pytest",
     "pytest-xdist",
-    "git+https://github.com/ansible-community/pytest-ansible.git",
+    "pytest-ansible",
 ]
 
 T = TypeVar("T", bound=ConfigSet)
 
 
 class AnsibleConfigSet(ConfigSet):
     """The ansible configuration."""
```

### Comparing `tox-ansible-2.0.0/src/tox_ansible.egg-info/PKG-INFO` & `tox-ansible-2.0.1/src/tox_ansible.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ansible
-Version: 2.0.0
+Version: 2.0.1
 Summary: A radical approach to testing ansible content
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Keywords: ansible,collections,tox
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `tox-ansible-2.0.0/src/tox_ansible.egg-info/SOURCES.txt` & `tox-ansible-2.0.1/src/tox_ansible.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/tests/conftest.py` & `tox-ansible-2.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/tests/integration/test_basic.py` & `tox-ansible-2.0.1/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/tests/integration/test_user_provided.py` & `tox-ansible-2.0.1/tests/integration/test_user_provided.py`

 * *Files identical despite different names*

### Comparing `tox-ansible-2.0.0/tox.ini` & `tox-ansible-2.0.1/tox.ini`

 * *Files identical despite different names*

