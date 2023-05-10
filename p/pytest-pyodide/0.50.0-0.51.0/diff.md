# Comparing `tmp/pytest-pyodide-0.50.0.tar.gz` & `tmp/pytest-pyodide-0.51.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-pyodide-0.50.0.tar", last modified: Thu Jan  5 18:01:49 2023, max compression
+gzip compressed data, was "pytest-pyodide-0.51.0.tar", last modified: Wed May 10 01:27:35 2023, max compression
```

## Comparing `pytest-pyodide-0.50.0.tar` & `pytest-pyodide-0.51.0.tar`

### file list

```diff
@@ -1,56 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.750112 pytest-pyodide-0.50.0/
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.746112 pytest-pyodide-0.50.0/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.github/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.746112 pytest-pyodide-0.50.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3179 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.github/workflows/filtermatrix.py
--rw-r--r--   0 runner    (1001) docker     (122)     5854 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.github/workflows/testall.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     3253 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    10632 2023-01-05 18:01:49.750112 pytest-pyodide-0.50.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10024 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.746112 pytest-pyodide-0.50.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/examples/test_install_package.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.746112 pytest-pyodide-0.50.0/examples/wheels/
--rw-r--r--   0 runner    (1001) docker     (122)    93002 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.742112 pytest-pyodide-0.50.0/pytest_pyodide/
--rw-r--r--   0 runner    (1001) docker     (122)      791 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/_decorator_in_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/copy_files_to_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)    13981 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8307 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/fixture.py
--rw-r--r--   0 runner    (1001) docker     (122)     9274 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/hook.py
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/node_test_driver.js
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)     5171 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/run_tests_inside_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)    16616 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)     3020 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/server.py
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/pytest_pyodide/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.746112 pytest-pyodide-0.50.0/pytest_pyodide.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10632 2023-01-05 18:01:49.000000 pytest-pyodide-0.50.0/pytest_pyodide.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1691 2023-01-05 18:01:49.000000 pytest-pyodide-0.50.0/pytest_pyodide.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-05 18:01:49.000000 pytest-pyodide-0.50.0/pytest_pyodide.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-01-05 18:01:49.000000 pytest-pyodide-0.50.0/pytest_pyodide.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-01-05 18:01:49.000000 pytest-pyodide-0.50.0/pytest_pyodide.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-01-05 18:01:49.000000 pytest-pyodide-0.50.0/pytest_pyodide.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1207 2023-01-05 18:01:49.750112 pytest-pyodide-0.50.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.750112 pytest-pyodide-0.50.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-05 18:01:49.750112 pytest-pyodide-0.50.0/tests/datafiles/
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/datafiles/in_pyodide_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     9613 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_copy_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_fixture.py
--rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_jsassert.py
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_marker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_run_in_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-01-05 18:01:17.000000 pytest-pyodide-0.50.0/tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.899367 pytest-pyodide-0.51.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      958 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3177 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/workflows/filtermatrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2023 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.github/workflows/testall.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     3384 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/COMPATIBILITY.md
+-rw-r--r--   0 runner    (1001) docker     (122)    10400 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9771 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1086 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/examples/test_install_package.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/examples/wheels/
+-rw-r--r--   0 runner    (1001) docker     (122)    93002 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.899367 pytest-pyodide-0.51.0/pytest_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (122)      791 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/_decorator_in_pyodide.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.899367 pytest-pyodide-0.51.0/pytest_pyodide/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/_templates/module_test.html
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/_templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5403 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/copy_files_to_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13997 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8300 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9186 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/hook.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/node_test_driver.js
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5171 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/run_tests_inside_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16829 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/server.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/pytest_pyodide/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10400 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1948 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-10 01:27:35.000000 pytest-pyodide-0.51.0/pytest_pyodide.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 01:27:35.903367 pytest-pyodide-0.51.0/tests/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/datafiles/in_pyodide_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9613 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (122)     3845 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_copy_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6204 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2225 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_jsassert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_marker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2160 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1484 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_run_in_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-05-10 01:27:13.000000 pytest-pyodide-0.51.0/tests/test_testing.py
```

### Comparing `pytest-pyodide-0.50.0/.github/workflows/build.yaml` & `pytest-pyodide-0.51.0/.github/workflows/build.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 jobs:
   test:
       uses: ./.github/workflows/testall.yaml
       with:
         build-artifact-name: none
         build-artifact-path: none
+        pyodide-versions: "[0.23.2,0.22.0,0.21.3]"
 
   deploy:
     runs-on: ubuntu-20.04
     if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
     environment: PyPi-deploy
     steps:
       - uses: actions/checkout@v3
@@ -31,15 +32,7 @@
           python -m pip install build twine
           python -m build .
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
-  lint:
-    runs-on: ubuntu-20.04
-    steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v3
-        with:
-          python-version: 3.10.2
-      - uses: pre-commit/action@v2.0.3
```

### Comparing `pytest-pyodide-0.50.0/.github/workflows/filtermatrix.py` & `pytest-pyodide-0.51.0/.github/workflows/filtermatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             ranges[key].append((key, v))
 
 l = list(ranges.values())
 
 config_list: "list[dict[str, Any]]" = []
 for conf in itertools.product(*l):
     dict_out = {}
-    for (key, v) in conf:
+    for key, v in conf:
         dict_out[key] = v
     config_list.append(dict_out)
 
 if "include" in matrix:
     for inc_spec in matrix["include"]:
         config_list.append(inc_spec)
```

### Comparing `pytest-pyodide-0.50.0/.github/workflows/main.yaml` & `pytest-pyodide-0.51.0/.github/workflows/main.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -131,20 +131,19 @@
         with:
           name: ${{ inputs.build-artifact-name }}
           path: ${{ inputs.build-artifact-path }}
 
       - name: Install pytest-pyodide
         shell: bash -l {0}
         run: |
-          ${{needs.get_versions.outputs.pythonexec}} -m pip install pytest-cov
           if [ -d "pytest_pyodide" ]; then
             # Currently we only install the package for dependencies.
             # We then uninstall it otherwise tests fails due to pytest hook being
             # registered twice.
-              ${{needs.get_versions.outputs.pythonexec}} -m pip install -e .
+              ${{needs.get_versions.outputs.pythonexec}} -m pip install -e ".[test]"
               ${{needs.get_versions.outputs.pythonexec}} -m pip uninstall -y pytest-pyodide
           else
               ${{needs.get_versions.outputs.pythonexec}} -m pip install pytest-pyodide
           fi
           which npm && npm install -g npm && npm update
           which npm && npm install node-fetch@2
       - name: Run tests
```

### Comparing `pytest-pyodide-0.50.0/.github/workflows/testall.yaml` & `pytest-pyodide-0.51.0/.github/workflows/testall.yaml`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/.pre-commit-config.yaml` & `pytest-pyodide-0.51.0/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-exclude: (^.*patches|.*\.cgi$|^packages/micropip/src/micropip/externals|^benchmark/benchmarks$)
 default_language_version:
   python: "3.10"
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
@@ -12,45 +11,27 @@
       - id: check-yaml
         exclude: .clang-format
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
 
-  - repo: https://github.com/PyCQA/isort
-    rev: "5.11.4"
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.254"
     hooks:
-      - id: isort
-
-  - repo: https://github.com/asottile/pyupgrade
-    rev: "v3.3.1"
-    hooks:
-      - id: pyupgrade
-        args: ["--py310-plus"]
-
-  - repo: https://github.com/hadialqattan/pycln
-    rev: "v2.1.2"
-    hooks:
-      - id: pycln
-        args: [--config=pyproject.toml]
-        stages: [manual]
+      - id: ruff
+        args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: "22.12.0"
+    rev: "23.1.0"
     hooks:
       - id: black
 
-  - repo: https://github.com/pycqa/flake8
-    rev: "6.0.0"
-    hooks:
-      - id: flake8
-        additional_dependencies: [flake8-bugbear]
-
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: "v0.991"
+    rev: "v1.1.1"
     hooks:
       - id: mypy
         exclude: (setup.py|^tests|conftest.py)
         args: []
         additional_dependencies: &mypy-deps
           - packaging
           - types-docutils
@@ -61,12 +42,15 @@
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: "v0.9.0.2"
     hooks:
       - id: shellcheck
 
   - repo: https://github.com/codespell-project/codespell
-    rev: "v2.2.2"
+    rev: "v2.2.4"
     hooks:
       - id: codespell
         args: ["-L", "te,slowy,aray,ba,nd,classs,crate,feld,lits"]
         exclude: ^benchmark/benchmarks/pystone_benchmarks/pystone\.py$
+
+ci:
+  autoupdate_schedule: "quarterly"
```

### Comparing `pytest-pyodide-0.50.0/CHANGELOG.md` & `pytest-pyodide-0.51.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## [0.51.0] - 2023-05-10
+
+- Added test templates files in the package.
+  [#87](https://github.com/pyodide/pytest-pyodide/pull/87)
+
 ## [0.50.0] - 2023-01-05
 
 - Add auto-setting of python version and runner version based on pyodide version.
   [#66](https://github.com/pyodide/pytest-pyodide/pull/66)
 
 - Add support for custom headers in the pytest web server code, by setting
   the `extra_headers` parameter in the `spawn_web_server` function.
```

### Comparing `pytest-pyodide-0.50.0/PKG-INFO` & `pytest-pyodide-0.51.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-pyodide
-Version: 0.50.0
+Version: 0.51.0
 Summary: "Pytest plugin for testing applications that use Pyodide"
 Home-page: https://github.com/pyodide/pytest-pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pytest-pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
 
 # pytest-pyodide
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pytest-pyodide.svg)](https://pypi.org/project/pytest-pyodide/)
 ![GHA](https://github.com/pyodide/pytest-pyodide/actions/workflows/main.yml/badge.svg)
 [![codecov](https://codecov.io/gh/pyodide/pytest-pyodide/branch/main/graph/badge.svg?token=U7tWHpJj5c)](https://codecov.io/gh/pyodide/pytest-pyodide)
 
@@ -296,20 +297,13 @@
 ## Examples
 
 See [`examples`](./examples).
 
 
 ## Compatible Pyodide versions
 
-
-Following versions of pytest-pyodide and Pyodide are tested in CI. Other versions may work, however with no guarantee.
-
-| pytest-pyodide | Tested Pyodide versions |
-|----------------|-------------------------|
-| 0.23.*         | 0.21.0                  |
-| 0.50.0         | 0.21.0, 0.22.0          |
-
+See [`compatibility table`](./COMPATIBILITY.md).
 
 ## License
 
 pytest-pyodide uses the [Mozilla Public License Version
 2.0](https://choosealicense.com/licenses/mpl-2.0/).
```

### Comparing `pytest-pyodide-0.50.0/README.md` & `pytest-pyodide-0.51.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -281,20 +281,13 @@
 ## Examples
 
 See [`examples`](./examples).
 
 
 ## Compatible Pyodide versions
 
-
-Following versions of pytest-pyodide and Pyodide are tested in CI. Other versions may work, however with no guarantee.
-
-| pytest-pyodide | Tested Pyodide versions |
-|----------------|-------------------------|
-| 0.23.*         | 0.21.0                  |
-| 0.50.0         | 0.21.0, 0.22.0          |
-
+See [`compatibility table`](./COMPATIBILITY.md).
 
 ## License
 
 pytest-pyodide uses the [Mozilla Public License Version
 2.0](https://choosealicense.com/licenses/mpl-2.0/).
```

### Comparing `pytest-pyodide-0.50.0/examples/test_install_package.py` & `pytest-pyodide-0.51.0/examples/test_install_package.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl` & `pytest-pyodide-0.51.0/examples/wheels/snowballstemmer-2.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/__init__.py` & `pytest-pyodide-0.51.0/pytest_pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/_decorator_in_pyodide.py` & `pytest-pyodide-0.51.0/pytest_pyodide/_decorator_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/copy_files_to_pyodide.py` & `pytest-pyodide-0.51.0/pytest_pyodide/copy_files_to_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/decorator.py` & `pytest-pyodide-0.51.0/pytest_pyodide/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         return PyodideHandle(self.selenium, ptr)
 
     def find_class(self, module: str, name: str) -> Any:
         """
         Catch exceptions that only exist in the pyodide environment and
         convert them to exception in the host.
         """
-        if module == "pyodide" and name == "JsException":
+        if module in ("pyodide", "pyodide.ffi") and name == "JsException":
             return JsException
         else:
             return super().find_class(module, name)
 
 
 class Pickler(pickle.Pickler):
     def persistent_id(self, obj: Any) -> Any:
@@ -373,15 +373,15 @@
                 and node.end_lineno > func_line_no
                 and node.lineno < func_line_no
             ):
                 it = iter(node.body)  # type: ignore[attr-defined]
                 continue
 
             # We also want the function definition for the current test
-            if not isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
+            if not isinstance(node, ast.FunctionDef | ast.AsyncFunctionDef):
                 continue
 
             if node.lineno < func_line_no:
                 continue
 
             if node.name != funcname:
                 raise RuntimeError(
```

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/fixture.py` & `pytest-pyodide-0.51.0/pytest_pyodide/fixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import contextlib
 import os
 from pathlib import Path
 
 import pytest
 
 from .runner import (
+    CHROME_FLAGS,
+    FIREFOX_FLAGS,
     NodeRunner,
     PlaywrightChromeRunner,
     PlaywrightFirefoxRunner,
     SeleniumChromeRunner,
     SeleniumFirefoxRunner,
     SeleniumSafariRunner,
     _BrowserBaseRunner,
@@ -34,19 +36,17 @@
                 "playwright not installed. try `pip install playwright && python -m playwright install`",
                 returncode=1,
             )
 
         with sync_playwright() as p:
             try:
                 chromium = p.chromium.launch(
-                    args=[
-                        "--js-flags=--expose-gc",
-                    ],
+                    args=CHROME_FLAGS,
                 )
-                firefox = p.firefox.launch()
+                firefox = p.firefox.launch(args=FIREFOX_FLAGS)
                 # webkit = p.webkit.launch()
             except Exception as e:
                 pytest.exit(f"playwright failed to launch\n{e}", returncode=1)
             try:
                 yield {
                     "chrome": chromium,
                     "firefox": firefox,
@@ -234,15 +234,14 @@
             selenium, script_timeout=parse_driver_timeout(request.node)
         ):
             yield selenium
 
 
 @pytest.fixture(scope="function")
 def console_html_fixture(request, runtime, web_server_main, playwright_browsers):
-
     if runtime == "node":
         pytest.skip("no support in node")
 
     with selenium_common(
         request,
         runtime,
         web_server_main,
```

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/hook.py` & `pytest-pyodide-0.51.0/pytest_pyodide/hook.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 
 def pytest_unconfigure(config):
     if config.option.run_in_pyodide:
         close_pyodide_browsers()
 
 
 def pytest_configure(config):
-
     config.addinivalue_line(
         "markers",
         "skip_refcount_check: Don't run refcount checks",
     )
 
     config.addinivalue_line(
         "markers",
@@ -216,15 +215,15 @@
 
 
 @pytest.hookimpl(tryfirst=True)
 def pytest_runtest_setup(item):
     if item.config.option.run_in_pyodide:
         if not hasattr(item, "fixturenames"):
             return
-        if pytest.pyodide_runtimes and "runtime" in item.fixturenames:  # type: ignore[truthy-bool]
+        if pytest.pyodide_runtimes and "runtime" in item.fixturenames:
             pytest.skip(reason="pyodide specific test, can't run in pyodide")
         else:
             # Pass this test to pyodide runner
             # First: make sure that pyodide has the test folder copied over
             item_path = Path(item.path)
             copy_files = list(item_path.parent.rglob("*"))
             # If we have a pyodide build dist folder with wheels in, copy those over
@@ -249,17 +248,17 @@
             copy_files_to_emscripten_fs(
                 copy_files_with_destinations, selenium, install_wheels=True
             )
     else:
         if not hasattr(item, "fixturenames"):
             # Some items like DoctestItem have no fixture
             return
-        if not pytest.pyodide_runtimes and "runtime" in item.fixturenames:  # type: ignore[truthy-bool]
+        if not pytest.pyodide_runtimes and "runtime" in item.fixturenames:
             pytest.skip(reason="Non-host test")
-        elif not pytest.pyodide_run_host_test and "runtime" not in item.fixturenames:  # type: ignore[truthy-bool]
+        elif not pytest.pyodide_run_host_test and "runtime" not in item.fixturenames:
             pytest.skip("Host test")
 
 
 @pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_call(item):
     if item.config.option.run_in_pyodide:
```

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/hypothesis.py` & `pytest-pyodide-0.51.0/pytest_pyodide/hypothesis.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/node_test_driver.js` & `pytest-pyodide-0.51.0/pytest_pyodide/node_test_driver.js`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/pyodide.py` & `pytest-pyodide-0.51.0/pytest_pyodide/pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/run_tests_inside_pyodide.py` & `pytest-pyodide-0.51.0/pytest_pyodide/run_tests_inside_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/runner.py` & `pytest-pyodide-0.51.0/pytest_pyodide/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import json
 import textwrap
 from pathlib import Path
 
 import pexpect
 
+CHROME_FLAGS: list[str] = ["--js-flags=--expose-gc"]
+FIREFOX_FLAGS: list[str] = []
+NODE_FLAGS: list[str] = []
+
+
 TEST_SETUP_CODE = """
 Error.stackTraceLimit = Infinity;
 
 // Fix globalThis is messed up in firefox see facebook/react#16606.
 // Replace it with window.
 globalThis.globalThis = globalThis.window || globalThis;
 
@@ -401,47 +406,47 @@
         if retval[0] == 0:
             return retval[1]
         else:
             raise JavascriptException(retval[1], retval[2])
 
 
 class SeleniumFirefoxRunner(_SeleniumBaseRunner):
-
     browser = "firefox"
 
     def get_driver(self):
         from selenium.webdriver import Firefox
         from selenium.webdriver.firefox.options import Options
 
         options = Options()
         options.add_argument("--headless")
+        for flag in FIREFOX_FLAGS:
+            options.add_argument(flag)
 
         return Firefox(executable_path="geckodriver", options=options)
 
 
 class SeleniumChromeRunner(_SeleniumBaseRunner):
-
     browser = "chrome"
 
     def get_driver(self):
         from selenium.webdriver import Chrome
         from selenium.webdriver.chrome.options import Options
 
         options = Options()
         options.add_argument("--headless")
         options.add_argument("--no-sandbox")
-        options.add_argument("--js-flags=--expose-gc")
+        for flag in CHROME_FLAGS:
+            options.add_argument(flag)
         return Chrome(options=options)
 
     def collect_garbage(self):
         self.driver.execute_cdp_cmd("HeapProfiler.collectGarbage", {})
 
 
 class SeleniumSafariRunner(_SeleniumBaseRunner):
-
     browser = "safari"
     script_timeout = 30
 
     def get_driver(self):
         from selenium.webdriver import Safari
         from selenium.webdriver.safari.options import Options
 
@@ -470,22 +475,22 @@
         self.p.setecho(False)
         self.p.delaybeforesend = None
         # disable canonical input processing mode to allow sending longer lines
         # See: https://pexpect.readthedocs.io/en/stable/api/pexpect.html#pexpect.spawn.send
         self.p.sendline("stty -icanon")
 
         node_version = pexpect.spawn("node --version").read().decode("utf-8")
-        node_extra_args = ""
+        extra_args = NODE_FLAGS[:]
         # Node v14 require the --experimental-wasm-bigint which
         # produces errors on later versions
         if node_version.startswith("v14"):
-            node_extra_args = "--experimental-wasm-bigint"
+            extra_args.append("--experimental-wasm-bigint")
 
         self.p.sendline(
-            f"node --expose-gc {node_extra_args} {curdir}/node_test_driver.js {self.base_url} {self.dist_dir}",
+            f"node --expose-gc {' '.join(extra_args)} {curdir}/node_test_driver.js {self.base_url} {self.dist_dir}",
         )
 
         try:
             self.p.expect_exact("READY!!")
         except (pexpect.exceptions.EOF, pexpect.exceptions.TIMEOUT):
             raise JavascriptException("", self.p.before.decode()) from None
```

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide/utils.py` & `pytest-pyodide-0.51.0/pytest_pyodide/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide.egg-info/PKG-INFO` & `pytest-pyodide-0.51.0/pytest_pyodide.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pytest-pyodide
-Version: 0.50.0
+Version: 0.51.0
 Summary: "Pytest plugin for testing applications that use Pyodide"
 Home-page: https://github.com/pyodide/pytest-pyodide
 Author: Pyodide developers
 Project-URL: Bug Tracker, https://github.com/pyodide/pytest-pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Pytest
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
 
 # pytest-pyodide
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pytest-pyodide.svg)](https://pypi.org/project/pytest-pyodide/)
 ![GHA](https://github.com/pyodide/pytest-pyodide/actions/workflows/main.yml/badge.svg)
 [![codecov](https://codecov.io/gh/pyodide/pytest-pyodide/branch/main/graph/badge.svg?token=U7tWHpJj5c)](https://codecov.io/gh/pyodide/pytest-pyodide)
 
@@ -296,20 +297,13 @@
 ## Examples
 
 See [`examples`](./examples).
 
 
 ## Compatible Pyodide versions
 
-
-Following versions of pytest-pyodide and Pyodide are tested in CI. Other versions may work, however with no guarantee.
-
-| pytest-pyodide | Tested Pyodide versions |
-|----------------|-------------------------|
-| 0.23.*         | 0.21.0                  |
-| 0.50.0         | 0.21.0, 0.22.0          |
-
+See [`compatibility table`](./COMPATIBILITY.md).
 
 ## License
 
 pytest-pyodide uses the [Mozilla Public License Version
 2.0](https://choosealicense.com/licenses/mpl-2.0/).
```

### Comparing `pytest-pyodide-0.50.0/pytest_pyodide.egg-info/SOURCES.txt` & `pytest-pyodide-0.51.0/pytest_pyodide.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .flake8
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
+COMPATIBILITY.md
 README.md
 conftest.py
 pyproject.toml
 setup.cfg
 ./pytest_pyodide/__init__.py
 ./pytest_pyodide/_decorator_in_pyodide.py
 ./pytest_pyodide/copy_files_to_pyodide.py
@@ -15,14 +16,17 @@
 ./pytest_pyodide/hypothesis.py
 ./pytest_pyodide/node_test_driver.js
 ./pytest_pyodide/pyodide.py
 ./pytest_pyodide/run_tests_inside_pyodide.py
 ./pytest_pyodide/runner.py
 ./pytest_pyodide/server.py
 ./pytest_pyodide/utils.py
+./pytest_pyodide/_templates/__init__.py
+./pytest_pyodide/_templates/module_test.html
+./pytest_pyodide/_templates/test.html
 .github/FUNDING.yml
 .github/codecov.yml
 .github/workflows/build.yaml
 .github/workflows/filtermatrix.py
 .github/workflows/main.yaml
 .github/workflows/testall.yaml
 examples/test_install_package.py
@@ -42,14 +46,17 @@
 pytest_pyodide/utils.py
 pytest_pyodide.egg-info/PKG-INFO
 pytest_pyodide.egg-info/SOURCES.txt
 pytest_pyodide.egg-info/dependency_links.txt
 pytest_pyodide.egg-info/entry_points.txt
 pytest_pyodide.egg-info/requires.txt
 pytest_pyodide.egg-info/top_level.txt
+pytest_pyodide/_templates/__init__.py
+pytest_pyodide/_templates/module_test.html
+pytest_pyodide/_templates/test.html
 tests/test_copy_files.py
 tests/test_decorator.py
 tests/test_fixture.py
 tests/test_jsassert.py
 tests/test_marker.py
 tests/test_options.py
 tests/test_run_in_pyodide.py
```

### Comparing `pytest-pyodide-0.50.0/setup.cfg` & `pytest-pyodide-0.51.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -25,30 +25,35 @@
 	pytest
 	pytest-asyncio
 	hypothesis
 	selenium
 	playwright
 	pyodide-tblib # Forked to add https://github.com/ionelmc/python-tblib/pull/66
 
+[options.extras_require]
+test = 
+	pytest-cov
+	build
+	requests
+
 [options.package_data]
-pytest_pyodide = *.js
+pytest_pyodide = 
+	*.js
+pytest_pyodide._templates = 
+	*.html
 
 [options.entry_points]
 pytest11 = 
 	pytest_pyodide = pytest_pyodide.fixture
 	pytest_pyodide_hook = pytest_pyodide.hook
 
-[options.packages.find]
-where = .
-
 [tool:pytest]
 asyncio_mode = strict
 addopts = 
 	--tb=short
 	--doctest-modules
 	--cov=pytest_pyodide --cov-report xml
-testpaths = tests
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pytest-pyodide-0.50.0/tests/datafiles/in_pyodide_tests.py` & `pytest-pyodide-0.51.0/tests/datafiles/in_pyodide_tests.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl` & `pytest-pyodide-0.51.0/tests/datafiles/pyodide_http-0.2.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/tests/test_copy_files.py` & `pytest-pyodide-0.51.0/tests/test_copy_files.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/tests/test_decorator.py` & `pytest-pyodide-0.51.0/tests/test_decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -71,19 +71,19 @@
 
 
 def test_inner_function_js_exception(selenium):
     @run_in_pyodide
     def inner_function(selenium):
         from pyodide.code import run_js
 
-        run_js("throw 'some error'")
+        run_js("throw new Error('some error');")
 
     with pytest.raises(
         JsException,
-        match="Error: some error",
+        match="some error",
     ):
         inner_function(selenium)
 
 
 def test_not_unpickable_return_value(selenium):
     @run_in_pyodide
     async def inner_function(selenium):
@@ -216,15 +216,21 @@
 @given(obj=any_strategy)
 @settings(
     std_hypothesis_settings,
     max_examples=25,
 )
 @run_in_pyodide
 def test_hypothesis(selenium_standalone, obj):
-    from pyodide import to_js
+    try:
+        from pyodide.ffi import to_js
+    except ImportError:
+        try:
+            from pyodide import to_js
+        except ImportError:
+            raise Exception("Could not import to_js") from None
 
     to_js(obj)
 
 
 run_in_pyodide_inner = run_in_pyodide()
 run_in_pyodide_alias2 = pytest.mark.driver_timeout(40)(run_in_pyodide_inner)
```

### Comparing `pytest-pyodide-0.50.0/tests/test_jsassert.py` & `pytest-pyodide-0.51.0/tests/test_jsassert.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/tests/test_options.py` & `pytest-pyodide-0.51.0/tests/test_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
 
 
 def test_dist_dir(pytester):
-
     dist_dir = "dist"
 
     pytester.makepyfile(
         f"""
         import pytest
         def test_option(request):
             assert str(request.config.getoption("--dist-dir", "")) == {dist_dir!r}
@@ -28,15 +27,14 @@
     )
 
     result = pytester.runpytest("--runner", runner)
     result.assert_outcomes(passed=1)
 
 
 def test_invalid_runner(pytester):
-
     runner = "blah"
 
     pytester.makepyfile(
         f"""
         import pytest
         def test_option(request):
             assert request.config.getoption("--runner") == {runner!r}
@@ -56,15 +54,14 @@
         "firefox",
         "safari",
         "node",
         "firefox,chrome",
     ],
 )
 def test_runtime(pytester, _runtime):
-
     runtimes = _runtime.split(",")
 
     pytester.makepyfile(
         f"""
         import pytest
         def test_option():
             assert pytest.pyodide_runtimes == set({runtimes!r})
@@ -78,15 +75,14 @@
 @pytest.mark.parametrize(
     "_runtime",
     [
         "invalid",
     ],
 )
 def test_invalid_runtime(pytester, _runtime):
-
     runtimes = _runtime.split(",")
 
     pytester.makepyfile(
         f"""
         import pytest
         def test_option():
             assert pytest.pyodide_runtimes == set({runtimes!r})
```

### Comparing `pytest-pyodide-0.50.0/tests/test_run_in_pyodide.py` & `pytest-pyodide-0.51.0/tests/test_run_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `pytest-pyodide-0.50.0/tests/test_testing.py` & `pytest-pyodide-0.51.0/tests/test_testing.py`

 * *Files identical despite different names*

