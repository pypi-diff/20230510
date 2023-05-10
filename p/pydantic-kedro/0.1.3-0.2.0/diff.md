# Comparing `tmp/pydantic-kedro-0.1.3.tar.gz` & `tmp/pydantic-kedro-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-kedro-0.1.3.tar", last modified: Wed Apr 26 18:00:38 2023, max compression
+gzip compressed data, was "pydantic-kedro-0.2.0.tar", last modified: Wed May 10 11:08:02 2023, max compression
```

## Comparing `pydantic-kedro-0.1.3.tar` & `pydantic-kedro-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.596019 pydantic-kedro-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.584019 pydantic-kedro-0.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.584019 pydantic-kedro-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.584019 pydantic-kedro-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/docs/arbitrary_types.md
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.584019 pydantic-kedro-0.1.3/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:00:38.596019 pydantic-kedro-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.580019 pydantic-kedro-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.588019 pydantic-kedro-0.1.3/src/pydantic_kedro/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/pydantic_kedro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.588019 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:59:47.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 18:00:38.000000 pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.580019 pydantic-kedro-0.1.3/src/test/catalogs/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/catalogs/conf/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/conf/base/catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/catalogs/conf/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/conf/local/credentials.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:00:38.592019 pydantic-kedro-0.1.3/src/test/catalogs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/data/tst1.json
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/catalogs/test_basic_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/test_ds_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/test_ds_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/test_ds_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-26 17:59:30.000000 pydantic-kedro-0.1.3/src/test/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.311260 pydantic-kedro-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-10 11:08:02.311260 pydantic-kedro-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/docs/arbitrary_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:08:02.311260 pydantic-kedro-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.303260 pydantic-kedro-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/pydantic_kedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:07:09.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.303260 pydantic-kedro-0.2.0/src/test/catalogs/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/catalogs/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/conf/base/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/catalogs/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/conf/local/credentials.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/catalogs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/data/tst1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/test_basic_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_ds_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_ds_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_ds_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_import.py
```

### Comparing `pydantic-kedro-0.1.3/.github/dependabot.yml` & `pydantic-kedro-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/.github/workflows/python-publish.yml` & `pydantic-kedro-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/.github/workflows/python-testing.yml` & `pydantic-kedro-0.2.0/.github/workflows/python-testing.yml`

 * *Files 8% similar despite different names*

```diff
@@ -38,9 +38,9 @@
       - name: Test with pytest
         run: |
           pytest
       - name: Test with mypy
         run: |
           mypy
       - name: Check Markdown (Optional)
-        uses: DavidAnson/markdownlint-cli2-action@v9
+        uses: DavidAnson/markdownlint-cli2-action@v10
         continue-on-error: true
```

### Comparing `pydantic-kedro-0.1.3/.pre-commit-config.yaml` & `pydantic-kedro-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/LICENSE` & `pydantic-kedro-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/PKG-INFO` & `pydantic-kedro-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.1.3
+Version: 0.2.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.1.3/README.md` & `pydantic-kedro-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/docs/arbitrary_types.md` & `pydantic-kedro-0.2.0/docs/arbitrary_types.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/docs/implementation_details.md` & `pydantic-kedro-0.2.0/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/mkdocs.yml` & `pydantic-kedro-0.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/pyproject.toml` & `pydantic-kedro-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,18 @@
 ]
 urls = { github = "https://github.com/NowanIlfideme/pydantic-kedro" }
 
 [project.optional-dependencies]
 dev = [
     "setuptools>=61.0.0",
     "setuptools-scm[toml]>=6.2",
-    "pre-commit==3.2.2",
+    "pre-commit==3.3.1",
     "black==23.3.0",
     "isort==5.12.0",
-    "ruff==0.0.263",
+    "ruff==0.0.265",
     "mypy==1.2.0",
     "pytest==7.3.1",
     # required for testing
     "kedro[pandas]",
 ]
 docs = [
     "mkdocs",
```

### Comparing `pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/folder.py` & `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
     if module_i is None:
         raise TypeError(f"Could not find module for {obj!r}")
     r_name: str = getattr(obj, "__qualname__", obj.__name__)  # type: ignore
     return f"{module_i.__name__}.{r_name}"
 
 
 class PydanticFolderDataSet(AbstractDataSet[BaseModel, BaseModel]):
-    """A Pydantic model with folder-based load/save.
+    """Dataset for saving/loading Pydantic models, based on saving sub-datasets in a folder.
 
     This allows fields with arbitrary types.
 
     Example:
     -------
     ```python
     class MyModel(BaseModel):
@@ -162,14 +162,19 @@
 
         Args:
         ----
         filepath : The location of the folder.
         """
         self._filepath = filepath
 
+    @property
+    def filepath(self) -> str:
+        """File path name."""
+        return str(self._filepath)
+
     def _save(self, data: BaseModel) -> None:
         """Save Pydantic model to the filepath."""
         fs: AbstractFileSystem = fsspec.open(self._filepath).fs  # type: ignore
         if isinstance(fs, LocalFileSystem):
             self._save_local(data, self._filepath)
         else:
             from tempfile import TemporaryDirectory
@@ -309,8 +314,8 @@
 
         # Create and write metadata
         meta = FolderFormatMetadata(model_class=model_class_str, model_info=model_info, catalog=catalog)
         with fsspec.open(f"{filepath}/meta.json", mode="w") as f:
             f.write(meta.json())  # type: ignore
 
     def _describe(self) -> Dict[str, Any]:
-        return dict(filepath=self._filepath)
+        return dict(filepath=self.filepath)
```

### Comparing `pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/json.py` & `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/json.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pydantic import BaseModel, create_model, parse_obj_as
 from pydantic.utils import import_string
 
 KLS_MARK_STR = "class"
 
 
 class PydanticJsonDataSet(AbstractDataSet[BaseModel, BaseModel]):
-    """A Pydantic model with JSON-based load/save.
+    """Dataset for saving/loading Pydantic models, based on JSON.
 
     Please note that the Pydantic model must be JSON-serializable.
     That means the fields are "pure" Pydantic fields,
     or you have added `json_encoders` to the model config.
 
     Example:
     -------
@@ -41,14 +41,19 @@
         """
         # parse the path and protocol (e.g. file, http, s3, etc.)
         protocol, path = get_protocol_and_path(filepath)
         self._protocol = protocol
         self._filepath = PurePosixPath(path)
         self._fs: AbstractFileSystem = fsspec.filesystem(self._protocol)
 
+    @property
+    def filepath(self) -> str:
+        """File path name."""
+        return str(self._filepath)
+
     def _load(self) -> BaseModel:
         """Load Pydantic model from the filepath.
 
         Returns
         -------
         Pydantic model.
         """
@@ -85,8 +90,8 @@
         # Open file and write to it
         save_path = get_filepath_str(self._filepath, self._protocol)
         with self._fs.open(save_path, mode="w") as f:
             f.write(tmp_obj.json())
 
     def _describe(self) -> Dict[str, Any]:
         """Return a dict that describes the attributes of the dataset."""
-        return dict(filepath=self._filepath, protocol=self._protocol)
+        return dict(filepath=self.filepath, protocol=self._protocol)
```

### Comparing `pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/yaml.py` & `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 class _YamlPreLoader(BaseModel):
     """YAML pre-loader model."""
 
     kls_mark_str: str = Field(alias=KLS_MARK_STR)  # type: ignore
 
 
 class PydanticYamlDataSet(AbstractDataSet[BaseModel, BaseModel]):
-    """A Pydantic model with YAML-based load/save.
+    """Dataset for saving/loading Pydantic models, based on YAML.
 
     Please note that the Pydantic model must be JSON-serializable.
     That means the fields are "pure" Pydantic fields,
     or you have added `json_encoders` to the model config.
 
     Example:
     -------
@@ -41,20 +41,26 @@
     def __init__(self, filepath: str) -> None:
         """Create a new instance of PydanticYamlDataSet to load/save Pydantic models for given filepath.
 
         Args:
         ----
         filepath : The location of the YAML file.
         """
+        # TODO: Update to just save the path and open it with `fsspec` directly
         # parse the path and protocol (e.g. file, http, s3, etc.)
         protocol, path = get_protocol_and_path(filepath)
         self._protocol = protocol
         self._filepath = PurePosixPath(path)
         self._fs: AbstractFileSystem = fsspec.filesystem(self._protocol)
 
+    @property
+    def filepath(self) -> str:
+        """File path name."""
+        return str(self._filepath)
+
     def _load(self) -> BaseModel:
         """Load Pydantic model from the filepath.
 
         Returns
         -------
         Pydantic model.
         """
@@ -88,8 +94,8 @@
         # Open file and write to it
         save_path = get_filepath_str(self._filepath, self._protocol)
         with self._fs.open(save_path, mode="w") as f:
             to_yaml_file(f, tmp_obj)
 
     def _describe(self) -> Dict[str, Any]:
         """Return a dict that describes the attributes of the dataset."""
-        return dict(filepath=self._filepath, protocol=self._protocol)
+        return dict(filepath=self.filepath, protocol=self._protocol)
```

### Comparing `pydantic-kedro-0.1.3/src/pydantic_kedro/datasets/zip.py` & `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/zip.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from kedro.io.core import AbstractDataSet
 from pydantic import BaseModel
 
 from .folder import PydanticFolderDataSet
 
 
 class PydanticZipDataSet(AbstractDataSet[BaseModel, BaseModel]):
-    """A Pydantic model with Zip-file-based load/save.
+    """Dataset for saving/loading Pydantic models, based on saving sub-datasets in a ZIP file.
 
     This allows fields with arbitrary types.
 
     Example:
     -------
     ```python
     class MyModel(BaseModel):
@@ -31,15 +31,20 @@
     def __init__(self, filepath: str) -> None:
         """Create a new instance of PydanticZipDataSet to load/save Pydantic models for given filepath.
 
         Args:
         ----
         filepath : The location of the Zip file.
         """
-        self._filepath = filepath
+        self._filepath = filepath  # NOTE: This is not checked when created.
+
+    @property
+    def filepath(self) -> str:
+        """File path name."""
+        return str(self._filepath)
 
     def _load(self) -> BaseModel:
         """Load Pydantic model from the filepath.
 
         Returns
         -------
         Pydantic model.
@@ -72,8 +77,8 @@
                 zip_fs = ZipFileSystem(fo=zip_file, mode="w")  # type: ignore
                 m_zip = zip_fs.get_mapper()
                 for k, v in m_local.items():
                     m_zip[k] = v
                 zip_fs.close()
 
     def _describe(self) -> Dict[str, Any]:
-        return dict(filepath=self._filepath)
+        return dict(filepath=self.filepath)
```

### Comparing `pydantic-kedro-0.1.3/src/pydantic_kedro/models.py` & `pydantic-kedro-0.2.0/src/pydantic_kedro/models.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/PKG-INFO` & `pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.1.3
+Version: 0.2.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pydantic-kedro-0.1.3/src/pydantic_kedro.egg-info/SOURCES.txt` & `pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,18 +22,20 @@
 src/pydantic_kedro.egg-info/PKG-INFO
 src/pydantic_kedro.egg-info/SOURCES.txt
 src/pydantic_kedro.egg-info/dependency_links.txt
 src/pydantic_kedro.egg-info/not-zip-safe
 src/pydantic_kedro.egg-info/requires.txt
 src/pydantic_kedro.egg-info/top_level.txt
 src/pydantic_kedro/datasets/__init__.py
+src/pydantic_kedro/datasets/auto.py
 src/pydantic_kedro/datasets/folder.py
 src/pydantic_kedro/datasets/json.py
 src/pydantic_kedro/datasets/yaml.py
 src/pydantic_kedro/datasets/zip.py
+src/test/test_auto.py
 src/test/test_ds_extended.py
 src/test/test_ds_pandas.py
 src/test/test_ds_simple.py
 src/test/test_import.py
 src/test/catalogs/test_basic_catalog.py
 src/test/catalogs/conf/base/catalog.yml
 src/test/catalogs/conf/local/.gitkeep
```

### Comparing `pydantic-kedro-0.1.3/src/test/catalogs/test_basic_catalog.py` & `pydantic-kedro-0.2.0/src/test/catalogs/test_basic_catalog.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.1.3/src/test/test_ds_extended.py` & `pydantic-kedro-0.2.0/src/test/test_ds_extended.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """Test extended models, but without external libraries."""
 from typing import Any, Dict, Union
 
 import pytest
 from kedro.extras.datasets.text import TextDataSet
 
-from pydantic_kedro import ArbModel, PydanticFolderDataSet, PydanticZipDataSet
+from pydantic_kedro import (
+    ArbModel,
+    PydanticAutoDataSet,
+    PydanticFolderDataSet,
+    PydanticZipDataSet,
+)
 
-Kls = Union[PydanticFolderDataSet, PydanticZipDataSet]
+Kls = Union[PydanticAutoDataSet, PydanticFolderDataSet, PydanticZipDataSet]
 
 
 class Singleton:
     """Class that is always equal to itself (for ease of testing)."""
 
     def __eq__(self, __o: object) -> bool:
         """Check for equality of the singleton."""
@@ -58,15 +63,15 @@
     ms: MyStr = MyStr("foobar")
     dct: Dict[str, Any] = {}
 
 
 @pytest.mark.parametrize(
     "mdl", [UserExtendedModel(), UserExtendedModel(dct={"a": Singleton(), "b": MyStr("bee")})]
 )
-@pytest.mark.parametrize("kls", [PydanticFolderDataSet, PydanticZipDataSet])
+@pytest.mark.parametrize("kls", [PydanticAutoDataSet, PydanticFolderDataSet, PydanticZipDataSet])
 def test_pandas_flat_model(mdl: UserExtendedModel, kls: Kls, tmpdir):
     """Test roundtripping of the flat Pandas model, using default Pickle dataset."""
     paths = [f"{tmpdir}/model_on_disk", f"memory://{tmpdir}/model_in_memory"]
     for path in paths:
         ds: Kls = kls(path)  # type: ignore
         ds.save(mdl)
         m2 = ds.load()
```

### Comparing `pydantic-kedro-0.1.3/src/test/test_ds_pandas.py` & `pydantic-kedro-0.2.0/src/test/test_ds_pandas.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,20 @@
 
 from typing import Any, Dict, Union
 
 import pandas as pd
 import pytest
 from kedro.extras.datasets.pandas import ParquetDataSet
 
-from pydantic_kedro import ArbModel, PydanticFolderDataSet, PydanticZipDataSet
+from pydantic_kedro import (
+    ArbModel,
+    PydanticAutoDataSet,
+    PydanticFolderDataSet,
+    PydanticZipDataSet,
+)
 
 Kls = Union[PydanticFolderDataSet, PydanticZipDataSet]
 
 dfx = pd.DataFrame([[1, 2, 3]], columns=["a", "b", "c"])
 
 
 class _PdModel(ArbModel):
@@ -45,29 +50,29 @@
     df_map: dict[int, pd.DataFrame] = {1: dfx}
     df_list: list[pd.DataFrame] = [dfx]
     nested: Inner = Inner()
     onion: Union[pd.DataFrame, Dict[str, Any]] = dfx
     any_model: Any = None
 
 
-@pytest.mark.parametrize("kls", [PydanticFolderDataSet, PydanticZipDataSet])
+@pytest.mark.parametrize("kls", [PydanticAutoDataSet, PydanticFolderDataSet, PydanticZipDataSet])
 def test_pandas_flat_model(kls: Kls, tmpdir):
     """Test roundtripping of the flat Pandas model, using default Pickle dataset."""
     mdl = FlatPandasModel(df=dfx, val=1)
     paths = [f"{tmpdir}/model_on_disk", f"memory://{tmpdir}/model_in_memory"]
     for path in paths:
         ds: Kls = kls(path)  # type: ignore
         with pytest.warns(match="No dataset defined for.*"):
             ds.save(mdl)
         m2 = ds.load()
         assert isinstance(m2, FlatPandasModel)
         assert m2.df.equals(mdl.df)
 
 
-@pytest.mark.parametrize("kls", [PydanticFolderDataSet, PydanticZipDataSet])
+@pytest.mark.parametrize("kls", [PydanticAutoDataSet, PydanticFolderDataSet, PydanticZipDataSet])
 def test_pandas_nested_model(kls: Kls, tmpdir):
     """Test roundtripping of the nested Pandas model, using Parquet dataset."""
     mdl = NestedPandasModel()
     paths = [f"{tmpdir}/model_on_disk", f"memory://{tmpdir}/model_in_memory"]
     for path in paths:
         ds: Kls = kls(path)  # type: ignore
         ds.save(mdl)
```

