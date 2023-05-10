# Comparing `tmp/pydantic-kedro-0.2.0.tar.gz` & `tmp/pydantic-kedro-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-kedro-0.2.0.tar", last modified: Wed May 10 11:08:02 2023, max compression
+gzip compressed data, was "pydantic-kedro-0.3.0.tar", last modified: Wed May 10 21:11:03 2023, max compression
```

## Comparing `pydantic-kedro-0.2.0.tar` & `pydantic-kedro-0.3.0.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.311260 pydantic-kedro-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-10 11:08:02.311260 pydantic-kedro-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/docs/arbitrary_types.md
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/docs/implementation_details.md
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 11:08:02.311260 pydantic-kedro-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.303260 pydantic-kedro-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/pydantic_kedro/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/pydantic_kedro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:07:09.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 11:08:02.000000 pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/catalogs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.303260 pydantic-kedro-0.2.0/src/test/catalogs/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/catalogs/conf/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/conf/base/catalog.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/catalogs/conf/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/conf/local/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/conf/local/credentials.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:08:02.307260 pydantic-kedro-0.2.0/src/test/catalogs/data/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/data/tst1.json
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/catalogs/test_basic_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_ds_extended.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_ds_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_ds_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 11:06:56.000000 pydantic-kedro-0.2.0/src/test/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/arbitrary_types.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/implementation_details.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/docs/standalone_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.228605 pydantic-kedro-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/src/pydantic_kedro/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/pydantic_kedro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 21:10:05.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 21:11:03.000000 pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/catalogs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.232605 pydantic-kedro-0.3.0/src/test/catalogs/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/catalogs/conf/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/conf/base/catalog.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/catalogs/conf/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/conf/local/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/conf/local/credentials.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 21:11:03.236605 pydantic-kedro-0.3.0/src/test/catalogs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/data/tst1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/catalogs/test_basic_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_docs_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_ds_extended.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_ds_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_ds_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-10 21:09:51.000000 pydantic-kedro-0.3.0/src/test/test_utils.py
```

### Comparing `pydantic-kedro-0.2.0/.github/dependabot.yml` & `pydantic-kedro-0.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/.github/workflows/python-publish.yml` & `pydantic-kedro-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/.github/workflows/python-testing.yml` & `pydantic-kedro-0.3.0/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/.pre-commit-config.yaml` & `pydantic-kedro-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/LICENSE` & `pydantic-kedro-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/PKG-INFO` & `pydantic-kedro-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.2.0
+Version: 0.3.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -41,20 +41,35 @@
 # `pydantic-kedro`
 
 Advanced serialization for [Pydantic](https://docs.pydantic.dev/) models
 via [Kedro](https://kedro.readthedocs.io/en/stable/index.html) and
 [fsspec](https://filesystem-spec.readthedocs.io/en/latest/).
 
 This package implements custom Kedro "datasets" for both "pure" and "arbitrary"
-Pydantic models.
+Pydantic models. You can also use it stand-alone, using Kedro just for
+serializing other object types.
 
-Please see the [docs](https://pydantic-kedro.rtfd.io) for a tutorial and
-more examples.
+Please see the [documentation](https://pydantic-kedro.rtfd.io) for a tutorial
+and more examples.
 
-## Minimal Example
+## Usage with Kedro
+
+You can use the [PydanticAutoDataSet][pydantic_kedro.PydanticAutoDataSet]
+or any other dataset from `pydantic-kedro` within your
+[Kedro catalog](https://docs.kedro.org/en/stable/get_started/kedro_concepts.html#data-catalog)
+to save your Pydantic models:
+
+```yaml
+# conf/base/catalog.yml
+my_pydantic_model:
+ type: pydantic_kedro.PydanticAutoDataSet
+ filepath: folder/my_model
+```
+
+## Direct Dataset Usage
 
 This example works for "pure", JSON-safe Pydantic models via
 `PydanticJsonDataSet`:
 
 ```python
 from pydantic import BaseModel
 from pydantic_kedro import PydanticJsonDataSet
@@ -73,7 +88,30 @@
 ds = PydanticJsonDataSet("memory://temporary-file.json")
 ds.save(obj)
 
 # We can re-load it from the same file
 read_obj = ds.load()
 assert read_obj.x == 1
 ```
+
+## Standalone Usage
+
+You can also use `pydantic-kedro` as a generic saving and loading engine for
+Pydantic models:
+
+```python
+from tempfile import TemporaryDirectory
+
+from pydantic import BaseModel
+from pydantic_kedro import load_model, save_model
+
+class MyModel(BaseModel):
+    """My custom model."""
+
+    name: str
+
+# We can use any fsspec URL, so we'll make a temporary folder
+with TemporaryDirectory() as tmpdir:
+    save_model(MyModel(name="foo"), f"{tmpdir}/my_model")
+    obj = load_model(f"{tmpdir}/my_model")
+    assert obj.name == "foo"
+```
```

### Comparing `pydantic-kedro-0.2.0/docs/arbitrary_types.md` & `pydantic-kedro-0.3.0/docs/arbitrary_types.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/docs/implementation_details.md` & `pydantic-kedro-0.3.0/docs/implementation_details.md`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/docs/index.md` & `pydantic-kedro-0.3.0/docs/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 via [Kedro](https://kedro.readthedocs.io/en/stable/index.html) and
 [fsspec](https://filesystem-spec.readthedocs.io/en/latest/).
 
 This package implements custom Kedro DataSet types for not only "pure" (JSON-serializable)
 Pydantic models, but also models with [`arbitrary_types_allowed`](https://docs.pydantic.dev/usage/types/#arbitrary-types-allowed).
 
 Keep reading for a basic tutorial,
-or check out the [API Reference](reference/index.md) for auto-generated docs.
+or check out the [API Reference](reference.md) for auto-generated docs.
 
 ## Pre-requisites
 
 To simplify the documentation, we will refer to JSON-serializable Pydantic models
 as "pure" models, while all others will be "arbitrary" models.
 
 We also assume you are familiar with [Kedro's Data Catalog](https://docs.kedro.org/en/stable/data/data_catalog.html)
@@ -53,14 +53,20 @@
 # etc.
 ```
 
 If you are using Kedro for the pipelines or data catalog, that should be enough.
 
 If you want to use these datasets stand-alone, keep on reading.
 
+## Standalone Usage
+
+The functions [save_model][pydantic_kedro.save_model] and
+[load_model][pydantic_kedro.load_model] can be used directly.
+See [the relevant docs](standalone_usage.md) for more info.
+
 ## "Pure" Pydantic Models
 
 If you have a JSON-safe Pydantic model, you can use a
 [PydanticJsonDataSet][pydantic_kedro.PydanticJsonDataSet]
 or [PydanticYamlDataSet][pydantic_kedro.PydanticYamlDataSet]
 to save your model to any `fsspec`-supported location:
```

### Comparing `pydantic-kedro-0.2.0/mkdocs.yml` & `pydantic-kedro-0.3.0/mkdocs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 # See https://www.mkdocs.org/user-guide/configuration/#use_directory_urls
 site_url: ""
 use_directory_urls: false
 
 nav:
   - Overview: index.md
   - Arbitrary Types: arbitrary_types.md
-  - API Reference: reference/index.md
+  - Standalone Usage: standalone_usage.md
+  - API Reference: reference.md
   - Implementation Details: implementation_details.md
 
 theme:
   name: "material"
   palette:
     - media: "(prefers-color-scheme: light)"
       scheme: default
```

### Comparing `pydantic-kedro-0.2.0/pyproject.toml` & `pydantic-kedro-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/auto.py` & `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/auto.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/folder.py` & `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/folder.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/json.py` & `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/yaml.py` & `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/yaml.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/pydantic_kedro/datasets/zip.py` & `pydantic-kedro-0.3.0/src/pydantic_kedro/datasets/zip.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/pydantic_kedro/models.py` & `pydantic-kedro-0.3.0/src/pydantic_kedro/models.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/PKG-INFO` & `pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-kedro
-Version: 0.2.0
+Version: 0.3.0
 Summary: Kedro
 License: MIT License
         
         Copyright (c) 2023 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -41,20 +41,35 @@
 # `pydantic-kedro`
 
 Advanced serialization for [Pydantic](https://docs.pydantic.dev/) models
 via [Kedro](https://kedro.readthedocs.io/en/stable/index.html) and
 [fsspec](https://filesystem-spec.readthedocs.io/en/latest/).
 
 This package implements custom Kedro "datasets" for both "pure" and "arbitrary"
-Pydantic models.
+Pydantic models. You can also use it stand-alone, using Kedro just for
+serializing other object types.
 
-Please see the [docs](https://pydantic-kedro.rtfd.io) for a tutorial and
-more examples.
+Please see the [documentation](https://pydantic-kedro.rtfd.io) for a tutorial
+and more examples.
 
-## Minimal Example
+## Usage with Kedro
+
+You can use the [PydanticAutoDataSet][pydantic_kedro.PydanticAutoDataSet]
+or any other dataset from `pydantic-kedro` within your
+[Kedro catalog](https://docs.kedro.org/en/stable/get_started/kedro_concepts.html#data-catalog)
+to save your Pydantic models:
+
+```yaml
+# conf/base/catalog.yml
+my_pydantic_model:
+ type: pydantic_kedro.PydanticAutoDataSet
+ filepath: folder/my_model
+```
+
+## Direct Dataset Usage
 
 This example works for "pure", JSON-safe Pydantic models via
 `PydanticJsonDataSet`:
 
 ```python
 from pydantic import BaseModel
 from pydantic_kedro import PydanticJsonDataSet
@@ -73,7 +88,30 @@
 ds = PydanticJsonDataSet("memory://temporary-file.json")
 ds.save(obj)
 
 # We can re-load it from the same file
 read_obj = ds.load()
 assert read_obj.x == 1
 ```
+
+## Standalone Usage
+
+You can also use `pydantic-kedro` as a generic saving and loading engine for
+Pydantic models:
+
+```python
+from tempfile import TemporaryDirectory
+
+from pydantic import BaseModel
+from pydantic_kedro import load_model, save_model
+
+class MyModel(BaseModel):
+    """My custom model."""
+
+    name: str
+
+# We can use any fsspec URL, so we'll make a temporary folder
+with TemporaryDirectory() as tmpdir:
+    save_model(MyModel(name="foo"), f"{tmpdir}/my_model")
+    obj = load_model(f"{tmpdir}/my_model")
+    assert obj.name == "foo"
+```
```

### Comparing `pydantic-kedro-0.2.0/src/pydantic_kedro.egg-info/SOURCES.txt` & `pydantic-kedro-0.3.0/src/pydantic_kedro.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,34 +10,38 @@
 setup.py
 .github/dependabot.yml
 .github/workflows/python-publish.yml
 .github/workflows/python-testing.yml
 docs/arbitrary_types.md
 docs/implementation_details.md
 docs/index.md
-docs/reference/index.md
+docs/reference.md
+docs/standalone_usage.md
 src/pydantic_kedro/__init__.py
 src/pydantic_kedro/models.py
 src/pydantic_kedro/py.typed
+src/pydantic_kedro/utils.py
 src/pydantic_kedro/version.py
 src/pydantic_kedro.egg-info/PKG-INFO
 src/pydantic_kedro.egg-info/SOURCES.txt
 src/pydantic_kedro.egg-info/dependency_links.txt
 src/pydantic_kedro.egg-info/not-zip-safe
 src/pydantic_kedro.egg-info/requires.txt
 src/pydantic_kedro.egg-info/top_level.txt
 src/pydantic_kedro/datasets/__init__.py
 src/pydantic_kedro/datasets/auto.py
 src/pydantic_kedro/datasets/folder.py
 src/pydantic_kedro/datasets/json.py
 src/pydantic_kedro/datasets/yaml.py
 src/pydantic_kedro/datasets/zip.py
 src/test/test_auto.py
+src/test/test_docs_standalone.py
 src/test/test_ds_extended.py
 src/test/test_ds_pandas.py
 src/test/test_ds_simple.py
 src/test/test_import.py
+src/test/test_utils.py
 src/test/catalogs/test_basic_catalog.py
 src/test/catalogs/conf/base/catalog.yml
 src/test/catalogs/conf/local/.gitkeep
 src/test/catalogs/conf/local/credentials.yml
 src/test/catalogs/data/tst1.json
```

### Comparing `pydantic-kedro-0.2.0/src/test/catalogs/test_basic_catalog.py` & `pydantic-kedro-0.3.0/src/test/catalogs/test_basic_catalog.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/test/test_auto.py` & `pydantic-kedro-0.3.0/src/test/test_auto.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/test/test_ds_extended.py` & `pydantic-kedro-0.3.0/src/test/test_ds_extended.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/test/test_ds_pandas.py` & `pydantic-kedro-0.3.0/src/test/test_ds_pandas.py`

 * *Files identical despite different names*

### Comparing `pydantic-kedro-0.2.0/src/test/test_ds_simple.py` & `pydantic-kedro-0.3.0/src/test/test_ds_simple.py`

 * *Files identical despite different names*

