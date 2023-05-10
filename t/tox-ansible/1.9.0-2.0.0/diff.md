# Comparing `tmp/tox-ansible-1.9.0.tar.gz` & `tmp/tox-ansible-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox-ansible-1.9.0.tar", last modified: Sun Feb 19 22:38:15 2023, max compression
+gzip compressed data, was "tox-ansible-2.0.0.tar", last modified: Wed May 10 16:25:50 2023, max compression
```

## Comparing `tox-ansible-1.9.0.tar` & `tox-ansible-2.0.0.tar`

### file list

```diff
@@ -1,230 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.782583 tox-ansible-1.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (122)      589 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.782583 tox-ansible-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      432 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (122)     5969 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1301 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      228 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (122)      357 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    13870 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12774 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/TODO.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/galaxy.yml
--rw-r--r--   0 runner    (1001) docker     (122)      250 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1434 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.770583 tox-ansible-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.782583 tox-ansible-1.9.0/src/tox_ansible/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.782583 tox-ansible-1.9.0/src/tox_ansible/ansible/
--rw-r--r--   0 runner    (1001) docker     (122)     7538 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2684 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/ansible/scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.782583 tox-ansible-1.9.0/src/tox_ansible/filter/
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1500 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/filter/base_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/filter/by_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/filter/by_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     3148 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.782583 tox-ansible-1.9.0/src/tox_ansible/matrix/
--rw-r--r--   0 runner    (1001) docker     (122)     1823 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/matrix/axes.py
--rw-r--r--   0 runner    (1001) docker     (122)     4153 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/options.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/tox_ansible_test_case.py
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/tox_base_case.py
--rw-r--r--   0 runner    (1001) docker     (122)     6016 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/tox_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1807 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/tox_lint_case.py
--rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/tox_molecule_case.py
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/src/tox_ansible/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.782583 tox-ansible-1.9.0/src/tox_ansible.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13870 2023-02-19 22:38:15.000000 tox-ansible-1.9.0/src/tox_ansible.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5518 2023-02-19 22:38:15.000000 tox-ansible-1.9.0/src/tox_ansible.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-19 22:38:15.000000 tox-ansible-1.9.0/src/tox_ansible.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-02-19 22:38:15.000000 tox-ansible-1.9.0/src/tox_ansible.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-19 22:38:15.000000 tox-ansible-1.9.0/src/tox_ansible.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-02-19 22:38:15.000000 tox-ansible-1.9.0/src/tox_ansible.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-19 22:38:15.000000 tox-ansible-1.9.0/src/tox_ansible.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.770583 tox-ansible-1.9.0/tests/fixtures/collection/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/molecule/one/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/molecule/one/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/molecule/two/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/molecule/two/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/molecule/name_mismatch/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/molecule/name_mismatch/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/molecule/openstack/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/molecule/openstack/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/roles/complex/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/collection/roles/no_tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/roles/no_tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/roles/no_tests/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/collection/roles/simple/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/collection/roles/simple/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/roles/simple/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/roles/simple/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/roles/simple/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/collection/roles/simple/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/roles/simple/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/collection/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/expand_collection/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection/ignored/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection/ignored/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/expand_collection/ignored/molecule/not_found/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection/ignored/molecule/not_found/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection/molecule_one.yml
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection/molecule_two.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection/roles/simple/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection/roles/simple/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/expand_collection/roles/simple/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection/roles/simple/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.786583 tox-ansible-1.9.0/tests/fixtures/expand_collection/roles/simple/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection/roles/simple/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/ignored/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/ignored/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/ignored/molecule/not_found/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/ignored/molecule/not_found/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/roles/simple/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/roles/simple/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/roles/simple/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/roles/simple/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/roles/simple/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/roles/simple/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_comma/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/ignored/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/ignored/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/ignored/molecule/not_found/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/ignored/molecule/not_found/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/roles/simple/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/roles/simple/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/roles/simple/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/roles/simple/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/roles/simple/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/roles/simple/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/expand_collection_newlines/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/has_deps/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/has_deps/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.774583 tox-ansible-1.9.0/tests/fixtures/has_deps/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/has_deps/molecule/one/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/has_deps/molecule/one/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/has_deps/molecule/two/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/has_deps/molecule/two/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/has_deps/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/has_deps/roles/simple/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/has_deps/roles/simple/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/has_deps/roles/simple/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/has_deps/roles/simple/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/has_deps/roles/simple/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/has_deps/roles/simple/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/has_deps/roles/simple/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      177 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/has_deps/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/is_precommit/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/molecule/one/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/molecule/one/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/molecule/two/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/molecule/two/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/molecule/name_mismatch/
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/molecule/name_mismatch/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/molecule/openstack/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/molecule/openstack/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/complex/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/no_tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/no_tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/no_tests/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/simple/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/simple/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/simple/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/simple/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/simple/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/simple/tasks/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/roles/simple/tasks/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/is_precommit/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/not_collection/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/not_collection/.config/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/not_collection/.config/molecule/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/not_collection/.config/molecule/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/not_collection/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/not_collection/molecule/one/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/not_collection/molecule/one/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/not_collection/molecule/two/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/not_collection/molecule/two/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)      590 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/not_collection/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/nothing/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/nothing/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.790583 tox-ansible-1.9.0/tests/fixtures/nothing/molecule/dont_find_me/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/nothing/molecule/dont_find_me/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/nothing/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/tests/fixtures/simplified/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/simplified/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/simplified/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/tests/fixtures/simplified/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/simplified/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/tests/fixtures/simplified/molecule/two/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/simplified/molecule/two/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/simplified/roles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/simplified/roles/myrole/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.778583 tox-ansible-1.9.0/tests/fixtures/simplified/roles/myrole/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/tests/fixtures/simplified/roles/myrole/molecule/another/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/simplified/roles/myrole/molecule/another/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/simplified/roles/myrole/molecule/another/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/tests/fixtures/simplified/roles/myrole/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/simplified/roles/myrole/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/simplified/roles/myrole/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (122)      162 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/fixtures/simplified/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-19 22:38:15.794582 tox-ansible-1.9.0/tests/sanity/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/sanity/ignore-2.10.txt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/sanity/ignore-2.9.txt
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/sanity/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_by_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_by_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_everything.py
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2106 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_tox_helper.py
--rw-r--r--   0 runner    (1001) docker     (122)     3115 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_tox_lint_case.py
--rw-r--r--   0 runner    (1001) docker     (122)     5251 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_tox_molecule_case.py
--rw-r--r--   0 runner    (1001) docker     (122)      419 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-02-19 22:37:57.000000 tox-ansible-1.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.180768 tox-ansible-2.0.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.config/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.184768 tox-ansible-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.184768 tox-ansible-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/workflows/run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.184768 tox-ansible-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/integration.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/sanity.ini
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/tox-ansible.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/docs/unit.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.176768 tox-ansible-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.188768 tox-ansible-2.0.0/src/tox_ansible/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/src/tox_ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/src/tox_ansible/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.188768 tox-ansible-2.0.0/src/tox_ansible.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9709 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 16:25:50.000000 tox-ansible-2.0.0/src/tox_ansible.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.188768 tox-ansible-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.176768 tox-ansible-2.0.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.176768 tox-ansible-2.0.0/tests/fixtures/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.188768 tox-ansible-2.0.0/tests/fixtures/integration/test_basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/fixtures/integration/test_basic/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/fixtures/integration/test_basic/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/tests/fixtures/integration/test_user_provided/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/fixtures/integration/test_user_provided/galaxy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/fixtures/integration/test_user_provided/tox-ansible.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 16:25:50.192768 tox-ansible-2.0.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/integration/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tests/integration/test_user_provided.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-10 16:25:30.000000 tox-ansible-2.0.0/tox.ini
```

### Comparing `tox-ansible-1.9.0/.pre-commit-config.yaml` & `tox-ansible-2.0.0/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,93 @@
+---
 repos:
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-  - repo: https://github.com/psf/black
-    rev: 23.1.0
-    hooks:
-      - id: black
-        language_version: python3
-  - repo: https://github.com/pre-commit/pre-commit-hooks.git
+  - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-      - id: end-of-file-fixer
-      - id: trailing-whitespace
-      - id: mixed-line-ending
-      - id: fix-byte-order-marker
-      - id: check-executables-have-shebangs
       - id: check-merge-conflict
+      - id: check-symlinks
       - id: debug-statements
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+      - id: end-of-file-fixer
+      - id: no-commit-to-branch
+        args: [--branch, main]
+      - id: trailing-whitespace
+
+  - repo: https://github.com/asottile/add-trailing-comma.git
+    rev: v2.4.0
+    hooks:
+      - id: add-trailing-comma
+        args:
+          - --py36-plus
+
+  - repo: https://github.com/Lucas-C/pre-commit-hooks.git
+    rev: v1.5.1
+    hooks:
+      - id: remove-tabs
+
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    # keep it before yamllint
+    rev: v3.0.0-alpha.6
     hooks:
-      - id: flake8
-  - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.29.0
+      - id: prettier
+        always_run: true
+        additional_dependencies:
+          - prettier
+          - prettier-plugin-toml
+          - prettier-plugin-sort-json
+
+  - repo: https://github.com/psf/black
+    rev: 23.3.0
     hooks:
-      - id: yamllint
-        files: \.(yaml|yml)$
-        types: [file, yaml]
-        entry: yamllint --strict
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.0.0
+      - id: black
+
+  - repo: https://github.com/tox-dev/tox-ini-fmt
+    rev: "1.3.0"
+    hooks:
+      - id: tox-ini-fmt
+
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.263"
+    hooks:
+      - id: ruff
+        args:
+          - "--exit-non-zero-on-fix"
+
+  - repo: https://github.com/streetsidesoftware/cspell-cli
+    rev: v6.31.0
+    hooks:
+      - id: cspell
+        name: Spell check with cspell
+
+  # untill ruff has parity with darglint
+  - repo: https://github.com/PyCQA/flake8.git
+    rev: 6.0.0
     hooks:
-      - id: mypy
-        # empty args needed in order to match mypy cli behavior
-        args: []
-        entry: mypy src/
-        pass_filenames: false
+      - id: flake8
+        language_version: python3
         additional_dependencies:
-          - py>=1.9.0
-          - types-PyYAML
-  - repo: https://github.com/PyCQA/pylint
-    rev: v2.15.10
+          - darglint
+          - flake8-docstrings
+
+  - repo: https://github.com/pycqa/pylint.git
+    rev: v3.0.0a6
     hooks:
       - id: pylint
+        args:
+          - --output-format=colorized
         additional_dependencies:
           - pytest
+          - tox
           - pyyaml
+
+  - repo: https://github.com/pre-commit/mirrors-mypy.git
+    rev: v1.2.0
+    hooks:
+      - id: mypy
+        additional_dependencies:
+          - pytest
           - tox
+          - types-PyYAML
+        args:
+          - src
+          - tests
+          - --python-version=3.8
+        pass_filenames: false
```

### Comparing `tox-ansible-1.9.0/LICENSE` & `tox-ansible-2.0.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright 2020
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2023 Bradley A. Thornton
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tox-ansible-1.9.0/tox.ini` & `tox-ansible-2.0.0/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,81 @@
 [tox]
-minversion = 3.18.0
-skipsdist = true
-ignore_path = tests
-envlist =
-    py3{6,7,8,9,10,11}
-    py3{6,7,8,9,10,11}-devel
+requires =
+    tox>=4.2
+env_list =
+    py
     lint
-    packaging
-    coverage
-
-[ansible]
-ansible = 2.9 2.10
+    pkg
+no_package = true
+skip_missing_interpreters = true
+work_dir = {env:TOX_WORK_DIR:.tox}
 
 [testenv]
-usedevelop = true
+description = Run pytest under {basepython} ({envpython})
 deps =
-    testfixtures
-    coverage
-    pytest
-    pytest-cov
-    pytest-mock
-    devel: tox>=4.0.0a3
-passenv =
+    --editable .[test]
+pass_env =
+    CI
+    CONTAINER_*
     DOCKER_*
-    CONTAINERS_*
-setenv =
-    COVERAGE_FILE={env:COVERAGE_FILE:.coverage.{basepython}}
+    GITHUB_*
+    HOME
+    PYTEST_*
+    SSH_AUTH_SOCK
+    TERM
+    USER
+set_env =
+    COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}/.coverage.{envname}}
+    COVERAGE_PROCESS_START = {toxinidir}/pyproject.toml
+    FORCE_COLOR = 1
+    PIP_CONSTRAINT = {toxinidir}/requirements.txt
+    PRE_COMMIT_COLOR = always
+    TERM = xterm-256color
 commands =
-    pytest --cov=src --cov-report=term-missing {posargs:.}
+    coverage run -m pytest {posargs}
+    sh -c "coverage combine -q .tox/.coverage.* && coverage xml || true && coverage report"
 allowlist_externals =
-    bash
+    coverage
+    rm
+    sh
+envlist = lint, py, packaging, report, clean
 
-[testenv:coverage]
-parallel_show_output = true
-depends = py3{6,7,8,9}
-setenv =
+[testenv:lint]
+description = Enforce quality standards under {basepython} ({envpython})
+deps =
+    --editable .
+    pre-commit
 commands =
-    coverage combine
-    coverage report -m
+    pre-commit run --show-diff-on-failure --all-files
+install_command = pip install {opts} {packages}
 
-[testenv:lint]
+[testenv:pkg]
+description =
+    Do packaging/distribution
 skip_install = true
 deps =
-    pre_commit
+    build>=0.9
+    twine >= 4.0.2  # pyup: ignore
+set_env =
 commands =
-    python -m pre_commit run {posargs:--all}
+    rm -rfv {toxinidir}/dist/
+    python -m build \
+      --outdir {toxinidir}/dist/ \
+      {toxinidir}
+    sh -c "python -m twine check --strict {toxinidir}/dist/*"
 
-[testenv:packaging]
-usedevelop = false
+[testenv:clean]
+description = Erase coverage data
 skip_install = true
 deps =
-    collective.checkdocs >= 0.2
-    pep517 >= 0.5.0
-    twine >= 2.0.0
+    coverage[toml]
 commands =
-    bash -c "rm -rf {toxinidir}/dist/ {toxinidir}/build/ && mkdir -p {toxinidir}/dist/"
-    python -m pep517.build \
-      --source \
-      --binary \
-      --out-dir {toxinidir}/dist/ \
-      {toxinidir}
-    twine check dist/*
+    coverage erase
 
-[flake8]
-exclude = .tox/,.venv/,dist/,build/,.eggs/
-# To match black
-max-line-length = 88
+[testenv:report]
+description = Produce coverage report
+skip_install = true
+deps =
+    coverage[toml]
+commands =
+    coverage report
+    cat .tox/.tmp/.mypy/index.txt
```

