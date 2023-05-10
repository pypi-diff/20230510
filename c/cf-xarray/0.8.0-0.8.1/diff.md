# Comparing `tmp/cf_xarray-0.8.0.tar.gz` & `tmp/cf_xarray-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cf_xarray-0.8.0.tar", last modified: Thu Feb  9 05:18:46 2023, max compression
+gzip compressed data, was "cf_xarray-0.8.1.tar", last modified: Wed May 10 03:07:03 2023, max compression
```

## Comparing `cf_xarray-0.8.0.tar` & `cf_xarray-0.8.1.tar`

### file list

```diff
@@ -1,101 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.497506 cf_xarray-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.477506 cf_xarray-0.8.0/.binder/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.deepsource.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.477506 cf_xarray-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.477506 cf_xarray-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.github/workflows/parse_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.github/workflows/testpypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.github/workflows/upstream-dev-ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/.tributors
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-02-09 05:18:46.497506 cf_xarray-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.481506 cf_xarray-0.8.0/cf_xarray/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-09 05:18:45.000000 cf_xarray-0.8.0/cf_xarray/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    96133 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/criteria.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.481506 cf_xarray-0.8.0/cf_xarray/data/
--rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/data/cf-standard-name-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/options.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.485506 cf_xarray-0.8.0/cf_xarray/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/scripts/make_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/scripts/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/sgrid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.489506 cf_xarray-0.8.0/cf_xarray/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61429 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/tests/test_accessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/tests/test_coding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/cf_xarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.481506 cf_xarray-0.8.0/cf_xarray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-02-09 05:18:46.000000 cf_xarray-0.8.0/cf_xarray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-02-09 05:18:46.000000 cf_xarray-0.8.0/cf_xarray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 05:18:46.000000 cf_xarray-0.8.0/cf_xarray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-09 05:18:46.000000 cf_xarray-0.8.0/cf_xarray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-09 05:18:46.000000 cf_xarray-0.8.0/cf_xarray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.489506 cf_xarray-0.8.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/ci/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/ci/environment-no-optional-deps.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/ci/upstream-dev-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.497506 cf_xarray-0.8.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/2D_bounds_averaged.png
--rw-r--r--   0 runner    (1001) docker     (123)    62190 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/2D_bounds_error.png
--rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/2D_bounds_nonunique.png
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.497506 cf_xarray-0.8.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/_static/dataset-diagram-logo.tex
--rw-r--r--   0 runner    (1001) docker     (123)    48563 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/_static/full-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    71840 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)   130855 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/_static/rich-repr-example.png
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/bounds.md
--rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/cartopy_rotated_pole.png
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/coding.md
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/coord_axes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/custom-criteria.md
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/dsg.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 05:18:46.497506 cf_xarray-0.8.0/doc/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/flags.md
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/geometry.md
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/grid_mappings.md
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/howtouse.md
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/parametricz.md
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/plotting.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/provenance.md
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/selecting.md
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/sgrid_ugrid.md
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/units.md
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/doc/whats-new.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-02-09 05:18:13.000000 cf_xarray-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-09 05:18:46.497506 cf_xarray-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.259348 cf_xarray-0.8.1/.binder/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.deepsource.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.259348 cf_xarray-0.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.259348 cf_xarray-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/parse_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/testpypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.github/workflows/upstream-dev-ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/.tributors
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.267348 cf_xarray-0.8.1/cf_xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:07:02.000000 cf_xarray-0.8.1/cf_xarray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96676 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.267348 cf_xarray-0.8.1/cf_xarray/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/scripts/make_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/scripts/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/sgrid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.271348 cf_xarray-0.8.1/cf_xarray/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61220 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_coding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/cf_xarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.267348 cf_xarray-0.8.1/cf_xarray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 03:07:03.000000 cf_xarray-0.8.1/cf_xarray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.271348 cf_xarray-0.8.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/ci/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/ci/environment-no-optional-deps.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/ci/upstream-dev-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.275348 cf_xarray-0.8.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    46836 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/2D_bounds_averaged.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62190 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/2D_bounds_error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53236 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/2D_bounds_nonunique.png
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/dataset-diagram-logo.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    48563 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/full-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33479 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71840 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   130855 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/rich-repr-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/bounds.md
+-rw-r--r--   0 runner    (1001) docker     (123)    33785 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/cartopy_rotated_pole.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/coding.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/coord_axes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/custom-criteria.md
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/dsg.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/doc/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    23322 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/flags.md
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/geometry.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/grid_mappings.md
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/howtouse.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/parametricz.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/provenance.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/selecting.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/sgrid_ugrid.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/units.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/doc/whats-new.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-10 03:06:27.000000 cf_xarray-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:07:03.279348 cf_xarray-0.8.1/setup.cfg
```

### Comparing `cf_xarray-0.8.0/.github/workflows/ci.yaml` & `cf_xarray-0.8.1/.github/workflows/ci.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
       - name: Install cf_xarray
         run: |
           python -m pip install --no-deps -e .
       - name: Run Tests
         run: |
           pytest -n auto --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS,PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -87,15 +87,15 @@
       - name: Install cf_xarray
         run: |
           python -m pip install --no-deps -e .
       - name: Run Tests
         run: |
           pytest -n auto --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: RUNNER_OS,PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
 
@@ -151,14 +151,14 @@
       - name: Install mypy
         run: |
           python -m pip install 'mypy'
       - name: Run mypy
         run: |
           python -m mypy --install-types --non-interactive --cobertura-xml-report mypy_report cf_xarray/
       - name: Upload mypy coverage to Codecov
-        uses: codecov/codecov-action@v3.1.1
+        uses: codecov/codecov-action@v3.1.3
         with:
           file: mypy_report/cobertura.xml
           flags: mypy
           env_vars: PYTHON_VERSION
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `cf_xarray-0.8.0/.github/workflows/parse_logs.py` & `cf_xarray-0.8.1/.github/workflows/parse_logs.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/.github/workflows/pypi.yaml` & `cf_xarray-0.8.1/.github/workflows/pypi.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -68,28 +68,34 @@
         run: |
           python -m pip install --upgrade pip
           python -m pip install dist/cf_xarray*.whl
           python -m cf_xarray.scripts.print_versions
 
       - name: Publish package to TestPyPI
         if: github.event_name == 'push'
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           password: ${{ secrets.TESTPYPI_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
           verbose: true
 
 
   upload-to-pypi:
     needs: test-built-dist
     if: github.event_name == 'release'
     runs-on: ubuntu-latest
+
+    environment:
+      name: pypi
+      url: https://pypi.org/p/cf-xarray
+    permissions:
+      id-token: write
+
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
-          password: ${{ secrets.PYPI_PASSWORD }}
           verbose: true
```

### Comparing `cf_xarray-0.8.0/.github/workflows/testpypi-release.yaml` & `cf_xarray-0.8.1/.github/workflows/testpypi-release.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/.github/workflows/upstream-dev-ci.yaml` & `cf_xarray-0.8.1/.github/workflows/upstream-dev-ci.yaml`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/.gitignore` & `cf_xarray-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/.pre-commit-config.yaml` & `cf_xarray-0.8.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 ci:
     autoupdate_schedule: quarterly
 
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     # Ruff version.
-    rev: 'v0.0.237'
+    rev: 'v0.0.260'
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/rstcheck/rstcheck
-    rev: v6.1.1
+    rev: v6.1.2
     hooks:
         - id: rstcheck
           additional_dependencies: [sphinx, tomli]
           args: ['--config', 'pyproject.toml']
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
     - id: mdformat
       additional_dependencies:
         - mdformat-black
         - mdformat-myst
 
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.6.1
+    rev: 1.7.0
     hooks:
         - id: nbqa-black
         - id: nbqa-ruff
         - id: nbqa
           entry: nbqa mdformat
           name: nbqa-mdformat
           alias: nbqa-mdformat
@@ -57,10 +57,10 @@
 
   - repo: https://github.com/citation-file-format/cff-converter-python
     rev: "44e8fc9"
     hooks:
     - id: validate-cff
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: main
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
```

### Comparing `cf_xarray-0.8.0/.tributors` & `cf_xarray-0.8.1/.tributors`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/CITATION.cff` & `cf_xarray-0.8.1/CITATION.cff`

 * *Files 2% similar despite different names*

```diff
@@ -78,24 +78,24 @@
     affiliation: DKRZ (German Climate Computing Centre)
   - family-names: Vo
     given-names: Tom
     orcid: 'https://orcid.org/0000-0002-2461-0191'
     affiliation: Lawrence Livermore National Laboratory
 identifiers:
   - type: doi
-    value: 10.5281/zenodo.7538737
+    value: 10.5281/zenodo.4749735
     description: Zenodo DOI
 repository-code: 'https://github.com/xarray-contrib/cf-xarray'
 url: 'https://cf-xarray.readthedocs.io'
 abstract: >-
   cf_xarray provides an accessor (DataArray.cf or
   Dataset.cf) that allows you to interpret Climate and
   Forecast metadata convention attributes present on xarray
   objects.
 keywords:
   - cf-conventions
   - xarray
   - metadata
 license: Apache-2.0
 commit: 1b373a21b558423da8f22c3ec79f58737871719b
-version: 0.7.7
-date-released: '2023-01-14'
+version: 0.8.0
+date-released: '2023-02-08'
```

### Comparing `cf_xarray-0.8.0/LICENSE` & `cf_xarray-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/PKG-INFO` & `cf_xarray-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf_xarray
-Version: 0.8.0
+Version: 0.8.1
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.0/README.rst` & `cf_xarray-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/accessor.py` & `cf_xarray-0.8.1/cf_xarray/accessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
                 "`default` must be provided when `key` is not not a valid DataArray name (of hashable type)."
             )
         return list(always_iterable(default))
 
     default = [] if default is None else list(always_iterable(default))
 
     def _apply_single_mapper(mapper):
-
         try:
             results = mapper(obj, key)
         except (KeyError, ValueError) as e:
             if error or "I expected only one." in repr(e):
                 raise e
             else:
                 results = []
@@ -226,29 +225,30 @@
     try:
         from regex import match as regex_match
     except ImportError:
         from re import match as regex_match  # type: ignore
 
     if isinstance(obj, DataArray):
         obj = obj._to_temp_dataset()
+    variables = obj._variables
 
     if criteria is None:
         if not OPTIONS["custom_criteria"]:
             return []
         criteria = OPTIONS["custom_criteria"]
 
     if criteria is not None:
         criteria_iter = always_iterable(criteria, allowed=(tuple, list, set))
 
     criteria_map = ChainMap(*criteria_iter)
     results: set = set()
     if key in criteria_map:
         for criterion, patterns in criteria_map[key].items():
-            for var in obj.variables:
-                if regex_match(patterns, obj[var].attrs.get(criterion, "")):
+            for var in variables:
+                if regex_match(patterns, variables[var].attrs.get(criterion, "")):
                     results.update((var,))
                 # also check name specifically since not in attributes
                 elif (
                     criterion == "name"
                     and isinstance(var, str)
                     and regex_match(patterns, var)
                 ):
@@ -286,42 +286,45 @@
 
     valid_keys = _COORD_NAMES + _AXIS_NAMES
     if key not in valid_keys:
         raise KeyError(
             f"cf_xarray did not understand key {key!r}. Expected one of {valid_keys!r}"
         )
 
+    crds = obj.coords
+    crd_names = set(crds)
     search_in = set()
     attrs_or_encoding = ChainMap(obj.attrs, obj.encoding)
     coordinates = attrs_or_encoding.get("coordinates", None)
     # Handles case where the coordinates attribute is None
     # This is used to tell xarray to not write a coordinates attribute
     if coordinates:
         search_in.update(coordinates.split(" "))
     if not search_in:
-        search_in = set(obj.coords)
+        search_in = crd_names
 
     # maybe only do this for key in _AXIS_NAMES?
-    search_in.update(obj.indexes)
+    if obj._indexes:
+        search_in.update(obj._indexes)
 
-    search_in = search_in & set(obj.coords)
+    search_in = search_in & crd_names
     results: set = set()
     for coord in search_in:
-        var = obj.coords[coord]
+        var = crds[coord]
         if key in coordinate_criteria:
             for criterion, expected in coordinate_criteria[key].items():
                 if var.attrs.get(criterion, None) in expected:
                     results.update((coord,))
                 if criterion == "units":
                     # deal with pint-backed objects
                     units = getattr(var.data, "units", None)
                     if units in expected:
                         results.update((coord,))
 
-    if key in _AXIS_NAMES and "grid_topology" in obj.cf.cf_roles:
+    if key in ["X", "Y", "Z"] and "grid_topology" in obj.cf.cf_roles:
         sgrid_axes = sgrid.parse_axes(obj)
         results.update((search_in | set(obj.dims)) & sgrid_axes[key])
 
     return list(results)
 
 
 def _get_measure(obj: DataArray | Dataset, key: str) -> list[str]:
@@ -341,17 +344,16 @@
     List[str], Variable name(s) in parent xarray object that matches axis or coordinate `key`
     """
 
     if isinstance(obj, DataArray):
         obj = obj._to_temp_dataset()
 
     results = set()
-    for var in obj.variables:
-        da = obj[var]
-        attrs_or_encoding = ChainMap(da.attrs, da.encoding)
+    for var in obj._variables.values():
+        attrs_or_encoding = ChainMap(var.attrs, var.encoding)
         if "cell_measures" in attrs_or_encoding:
             attr = attrs_or_encoding["cell_measures"]
             try:
                 measures = parse_cell_methods_attr(attr)
             except ValueError as e:
                 raise ValueError(
                     f"{var} has malformed cell_measures attribute {attr}."
@@ -377,17 +379,21 @@
         key to check for.
 
     Returns
     -------
     List[str], Variable name(s) in parent xarray object that are bounds of `key`
     """
 
+    if isinstance(obj, DataArray):
+        obj = obj._to_temp_dataset()
+    variables = obj._variables
+
     results = set()
     for var in apply_mapper(_get_all, obj, key, error=False, default=[key]):
-        attrs_or_encoding = ChainMap(obj[var].attrs, obj[var].encoding)
+        attrs_or_encoding = ChainMap(variables[var].attrs, variables[var].encoding)
         if "bounds" in attrs_or_encoding:
             results |= {attrs_or_encoding["bounds"]}
 
     return list(results)
 
 
 def _get_grid_mapping_name(obj: DataArray | Dataset, key: str) -> list[str]:
@@ -406,25 +412,25 @@
     -------
     List[str], Variable name(s) in parent xarray object that matches grid_mapping_name `key`
     """
 
     if isinstance(obj, DataArray):
         obj = obj._to_temp_dataset()
 
+    variables = obj._variables
     results = set()
-    for var in obj.variables:
-        da = obj[var]
-        attrs_or_encoding = ChainMap(da.attrs, da.encoding)
+    for var in variables.values():
+        attrs_or_encoding = ChainMap(var.attrs, var.encoding)
         if "grid_mapping" in attrs_or_encoding:
             grid_mapping_var_name = attrs_or_encoding["grid_mapping"]
-            if grid_mapping_var_name not in obj.variables:
+            if grid_mapping_var_name not in variables:
                 raise ValueError(
                     f"{var} defines non-existing grid_mapping variable {grid_mapping_var_name}."
                 )
-            if key == obj[grid_mapping_var_name].attrs["grid_mapping_name"]:
+            if key == variables[grid_mapping_var_name].attrs["grid_mapping_name"]:
                 results.update([grid_mapping_var_name])
     return list(results)
 
 
 def _get_with_standard_name(
     obj: DataArray | Dataset, name: Hashable | Iterable[Hashable]
 ) -> list[Hashable]:
@@ -470,15 +476,15 @@
 
 
 def _get_indexes(obj: DataArray | Dataset, key: Hashable) -> list[Hashable]:
     """
     One or more of ('X', 'Y', 'Z', 'T', 'longitude', 'latitude', 'vertical', 'time',
     'area', 'volume'), or arbitrary measures, or standard names present in .indexes
     """
-    return [k for k in _get_all(obj, key) if k in obj.indexes]
+    return [k for k in _get_all(obj, key) if k in obj._indexes]
 
 
 def _get_coords(obj: DataArray | Dataset, key: Hashable) -> list[Hashable]:
     """
     One or more of ('X', 'Y', 'Z', 'T', 'longitude', 'latitude', 'vertical', 'time',
     'area', 'volume'), or arbitrary measures, or standard names present in .coords
     """
@@ -1207,15 +1213,14 @@
         reduce_dims: Hashable | Iterable[Hashable] | None = None,
         skipna: bool = True,
         p0: dict[str, Any] | None = None,
         bounds: dict[str, Any] | None = None,
         param_names: Sequence[str] | None = None,
         kwargs: dict[str, Any] | None = None,
     ):
-
         if coords is not None:
             if isinstance(coords, (Hashable, DataArray)):
                 coords_iter: Iterable[Hashable | DataArray] = [coords]
             else:
                 coords_iter = coords
             coords = [
                 apply_mapper(
@@ -2014,15 +2019,15 @@
             Override existing attributes.
         skip : str, iterable, optional
             Attribute(s) to skip: ``{"units", "grib", "amip", "description"}``.
         verbose : bool
             Print added attributes to screen.
         source : optional
             Path of `cf-standard-name-table.xml` or file object containing XML data.
-            If ``None``, use the default version associated with ``cf-xarray``.
+            If ``None``, use the latest CF standard name table (requires ``pooch``).
 
         Returns
         -------
         DataArray or Dataset with attributes added.
 
         Notes
         -----
@@ -2042,29 +2047,27 @@
         # Parse table
         info, table, aliases = parse_cf_standard_name_table(source)
 
         # Loop over standard names
         ds = self._maybe_to_dataset().copy(deep=False)
         attrs_to_print: dict = {}
         for std_name, var_names in ds.cf.standard_names.items():
-
             # Loop over variable names
             for var_name in var_names:
                 old_attrs = ds[var_name].attrs
                 std_name = aliases.get(std_name, std_name)
                 new_attrs = table.get(std_name, {})
 
                 # Loop over attributes
                 for key, value in new_attrs.items():
                     if (
                         value
                         and key not in skip_
                         and (override or key not in old_attrs)
                     ):
-
                         # Don't add units to time variables (e.g., datetime64, ...)
                         if key == "units" and _is_datetime_like(ds[var_name]):
                             continue
 
                         # Add attribute
                         ds[var_name].attrs[key] = value
 
@@ -2247,15 +2250,15 @@
             Name of variable whose bounds are desired
 
         Returns
         -------
         DataArray
         """
 
-        results = self.bounds.get(key, [])
+        results = self[[key]].cf.bounds.get(key, [])
         if not results:
             raise KeyError(f"No results found for {key!r}.")
 
         return self._obj[results[0] if len(results) == 1 else results]
 
     def get_bounds_dim_name(self, key: Hashable) -> Hashable:
         """
@@ -2266,20 +2269,26 @@
         key : str
             Name of variable whose bounds dimension name is desired.
 
         Returns
         -------
         str
         """
-        crd = self[key]
-        bounds = self.get_bounds(key)
+        (crd_name,) = apply_mapper(_get_all, self._obj, key, error=False, default=[key])
+        variables = self._obj._variables
+        crd = variables[crd_name]
+        crd_attrs = crd._attrs
+        if crd_attrs is None or "bounds" not in crd_attrs:
+            raise KeyError(f"No bounds variable found for {key!r}")
+
+        bounds = variables[crd_attrs["bounds"].strip()]
         bounds_dims = set(bounds.dims) - set(crd.dims)
         assert len(bounds_dims) == 1
         bounds_dim = bounds_dims.pop()
-        assert self._obj.sizes[bounds_dim] in [2, 4]
+        assert bounds.sizes[bounds_dim] in [2, 4]
         return bounds_dim
 
     def add_bounds(
         self,
         keys: str | Iterable[str],
         *,
         dim: str | Iterable[str] | None = None,
```

### Comparing `cf_xarray-0.8.0/cf_xarray/coding.py` & `cf_xarray-0.8.1/cf_xarray/coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/criteria.py` & `cf_xarray-0.8.1/cf_xarray/criteria.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,22 +90,30 @@
             "height_above_geopotential_datum",
             "height_above_reference_ellipsoid",
             "height_above_mean_sea_level",
         ),
         "positive": ("up", "down"),
     },
     "X": {
-        "standard_name": ("projection_x_coordinate",),
+        "standard_name": (
+            "projection_x_coordinate",
+            "grid_longitude",
+            "projection_x_angular_coordinate",
+        ),
         "_CoordinateAxisType": ("GeoX",),
         "axis": ("X",),
         "cartesian_axis": ("X",),
         "grads_dim": ("x",),
     },
     "Y": {
-        "standard_name": ("projection_y_coordinate",),
+        "standard_name": (
+            "projection_y_coordinate",
+            "grid_latitude",
+            "projection_y_angular_coordinate",
+        ),
         "_CoordinateAxisType": ("GeoY",),
         "axis": ("Y",),
         "cartesian_axis": ("Y",),
         "grads_dim": ("y",),
     },
     "T": {
         "standard_name": ("time",),
@@ -130,13 +138,13 @@
 #: regular expressions for guess_coord_axis
 regex = {
     "time": re.compile("\\bt\\b|(time|min|hour|day|week|month|year)[0-9]*"),
     "Z": re.compile(
         "(z|nav_lev|gdep|lv_|[o]*lev|bottom_top|sigma|h(ei)?ght|altitude|depth|"
         "isobaric|pres|isotherm)[a-z_]*[0-9]*"
     ),
-    "Y": re.compile("y|j|nlat|nj"),
+    "Y": re.compile("y|j|nlat|rlat|nj"),
     "latitude": re.compile("y?(nav_lat|lat|gphi)[a-z0-9]*"),
-    "X": re.compile("x|i|nlon|ni"),
+    "X": re.compile("x|i|nlon|rlon|ni"),
     "longitude": re.compile("x?(nav_lon|lon|glam)[a-z0-9]*"),
 }
 regex["T"] = regex["time"]
```

### Comparing `cf_xarray-0.8.0/cf_xarray/datasets.py` & `cf_xarray-0.8.1/cf_xarray/datasets.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/formatting.py` & `cf_xarray-0.8.1/cf_xarray/formatting.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     attr: str,
     dims=None,
     valid_keys=None,
     valid_values=None,
     default_keys=None,
     rich: bool = False,
 ):
-
     from .accessor import sort_maybe_hashable
 
     if dims is None:
         dims = []
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         if isinstance(attr, str):
```

### Comparing `cf_xarray-0.8.0/cf_xarray/geometry.py` & `cf_xarray-0.8.1/cf_xarray/geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/helpers.py` & `cf_xarray-0.8.1/cf_xarray/helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/options.py` & `cf_xarray-0.8.1/cf_xarray/options.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/scripts/make_doc.py` & `cf_xarray-0.8.1/cf_xarray/scripts/make_doc.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/sgrid.py` & `cf_xarray-0.8.1/cf_xarray/sgrid.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/tests/__init__.py` & `cf_xarray-0.8.1/cf_xarray/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,9 +63,10 @@
     return version.LooseVersion(vstring)
 
 
 has_cftime, requires_cftime = _importorskip("cftime")
 has_scipy, requires_scipy = _importorskip("scipy")
 has_shapely, requires_shapely = _importorskip("shapely")
 has_pint, requires_pint = _importorskip("pint")
+has_pooch, requires_pooch = _importorskip("pooch")
 _, requires_rich = _importorskip("rich")
 has_regex, requires_regex = _importorskip("regex")
```

### Comparing `cf_xarray-0.8.0/cf_xarray/tests/test_accessor.py` & `cf_xarray-0.8.1/cf_xarray/tests/test_accessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import itertools
 import pickle
 import warnings
 from textwrap import dedent
-from urllib.request import urlopen
 
 import matplotlib as mpl
 import numpy as np
 import pandas as pd
 import pytest
 import xarray as xr
 from matplotlib import pyplot as plt
@@ -37,14 +36,15 @@
     sgrid_roms,
     vert,
 )
 from . import (
     raise_if_dask_computes,
     requires_cftime,
     requires_pint,
+    requires_pooch,
     requires_regex,
     requires_rich,
     requires_scipy,
 )
 
 mpl.use("Agg")
 
@@ -57,15 +57,14 @@
 def assert_dicts_identical(dict1, dict2):
     assert dict1.keys() == dict2.keys()
     for k in dict1:
         assert_identical(dict1[k], dict2[k])
 
 
 def test_repr() -> None:
-
     assert "air_temperature: [(1, 2, 3)]" in ds_with_tuple.cf.__repr__()
 
     # Dataset.
     # Stars: axes, coords, and std names
     actual = airds.cf.__repr__()
     expected = """\
     Coordinates:
@@ -450,15 +449,14 @@
         ("groupby", {"group": "time"}, {"group": "T"}),
         ("groupby", {"group": "time.month"}, {"group": "T.month"}),
         ("groupby_bins", {"group": "lat", "bins": 5}, {"group": "latitude", "bins": 5}),
         ("coarsen", {"lon": 2, "lat": 5}, {"X": 2, "Y": 5}),
     ),
 )
 def test_wrapped_classes(obj, attr, xrkwargs, cfkwargs):
-
     if attr in ("rolling", "coarsen"):
         # TODO: xarray bug, rolling and coarsen don't accept ellipsis
         args = ()
     else:
         args = (...,)
 
     with raise_if_dask_computes():
@@ -518,24 +516,22 @@
 
     expected = multiple.transpose("y2", "y1", "x1", "x2")
     actual = multiple.cf.transpose("Y", "X")
     assert_identical(actual, expected)
 
 
 def test_preserve_unused_keys() -> None:
-
     ds = airds.copy(deep=False)
     ds.time.attrs.clear()
     actual = ds.cf.sel(X=260, Y=40, time=airds.time[:2], method="nearest")
     expected = ds.sel(lon=260, lat=40, time=airds.time[:2], method="nearest")
     assert_identical(actual, expected)
 
 
 def test_kwargs_expand_key_to_multiple_keys() -> None:
-
     actual = multiple.cf.isel(X=5, Y=3)
     expected = multiple.isel(x1=5, y1=3, x2=5, y2=3)
     assert_identical(actual, expected)
 
     actual = multiple.cf.mean("X")
     expected = multiple.mean(["x1", "x2"])
     assert_identical(actual, expected)
@@ -567,30 +563,28 @@
     with raise_if_dask_computes():
         expected = obj.sum("time")
         actual = obj.cf.sum("T")
     assert_identical(expected, actual)
 
 
 def test_dataarray_getitem() -> None:
-
     air = airds.air.copy(deep=False)
     air.name = None
 
     assert_identical(air.cf["longitude"], air["lon"])
     with pytest.raises(KeyError):
         air.cf[["longitude"]]
     with pytest.raises(KeyError):
         air.cf[["longitude", "latitude"]]
 
     air["cell_area"].attrs["standard_name"] = "area_grid_cell"
     assert_identical(air.cf["area_grid_cell"], air.cell_area.reset_coords(drop=True))
 
 
 def test_dataarray_plot() -> None:
-
     obj = airds.air.copy(deep=False)
 
     rv = obj.isel(time=1).transpose("lon", "lat").cf.plot()
     assert isinstance(rv, mpl.collections.QuadMesh)
     assert all(v > 180 for v in rv.axes.get_xlim())
     assert all(v < 200 for v in rv.axes.get_ylim())
     plt.close()
@@ -1138,16 +1132,16 @@
         "isobaric",
         "pressure",
         "isotherm",
         "gdep",
         "nav_lev",
     ]
 )
-_X_NAMES = _make_names(["x", "nlon", "i", "ni"])
-_Y_NAMES = _make_names(["y", "nlat", "j", "nj"])
+_X_NAMES = _make_names(["x", "nlon", "i", "ni", "rlon"])
+_Y_NAMES = _make_names(["y", "nlat", "j", "nj", "rlat"])
 _Z_NAMES = _VERTICAL_NAMES + ["olevel", "level", "zlevel"]
 _LATITUDE_NAMES = _make_names(["lat", "latitude", "gphi", "nav_lat"])
 _LONGITUDE_NAMES = _make_names(["lon", "longitude", "glam", "nav_lon"])
 
 
 @pytest.mark.parametrize(
     "kind, names",
@@ -1371,15 +1365,14 @@
 
     assert cf_xarray.accessor._get_with_standard_name(da, None) == []
 
 
 @pytest.mark.parametrize("obj", objects)
 @pytest.mark.parametrize("attr", ["drop_vars", "set_coords"])
 def test_drop_vars_and_set_coords(obj, attr):
-
     # DataArray object has no attribute set_coords
     if not isinstance(obj, Dataset) and attr == "set_coords":
         return
 
     # Get attribute
     expected = getattr(obj, attr)
     actual = getattr(obj.cf, attr)
@@ -1394,15 +1387,14 @@
     if isinstance(obj, Dataset) and "air" in obj.data_vars:
         assert_identical(expected("air"), actual("air_temperature"))
         assert_identical(expected(obj.variables), actual(obj.cf.keys()))
 
 
 @pytest.mark.parametrize("obj", objects)
 def test_drop_sel_and_reset_coords(obj):
-
     # Axis
     assert_identical(obj.drop_sel(lat=75), obj.cf.drop_sel(Y=75))
     # Coordinate
     assert_identical(obj.drop_sel(lat=75), obj.cf.drop_sel(latitude=75))
 
     # Cell measure
     assert_identical(obj.reset_coords("cell_area"), obj.cf.reset_coords("area"))
@@ -1411,27 +1403,25 @@
         assert_identical(
             obj.reset_coords("air"), obj.cf.reset_coords("air_temperature")
         )
 
 
 @pytest.mark.parametrize("ds", datasets)
 def test_drop_dims(ds):
-
     # Add data_var and coord to test _get_dims
     ds["lon_var"] = ds["lon"]
     ds = ds.assign_coords(lon_coord=ds["lon"])
 
     # Axis and coordinate
     for cf_name in ["X", "longitude"]:
         assert_identical(ds.drop_dims("lon"), ds.cf.drop_dims(cf_name))
 
 
 @pytest.mark.parametrize("obj", objects)
 def test_rename(obj):
-
     cf_dict = {
         "air_temperature" if isinstance(obj, Dataset) else "longitude": "renamed"
     }
     xr_dict = {
         "air"
         if isinstance(obj, Dataset) and "air" in obj.data_vars
         else "lon": "renamed"
@@ -1446,15 +1436,14 @@
     cf_dict = {"air_temperature": "renamed"}
     xr_dict = {(1, 2, 3): "renamed"}
     assert_identical(obj.rename(xr_dict), obj.cf.rename(cf_dict))
 
 
 @pytest.mark.parametrize("ds", datasets)
 def test_differentiate(ds):
-
     # Add data_var and coord to test _get_coords
     ds["lon_var"] = ds["lon"]
     ds = ds.assign_coords(lon_coord=ds["lon"])
 
     # Coordinate
     assert_identical(ds.differentiate("lon"), ds.cf.differentiate("lon"))
 
@@ -1705,23 +1694,17 @@
     vocab = {"temp": {"name": "tem|(?i)temp"}}
     ds = xr.Dataset()
     ds["Tempblah"] = [0, 1, 2]
     with cf_xarray.set_options(custom_criteria=vocab):
         assert_identical(ds.cf["temp"], ds["Tempblah"])
 
 
+@requires_pooch
 def test_cf_standard_name_table_version() -> None:
-
-    url = (
-        "https://raw.githubusercontent.com/cf-convention/cf-convention.github.io/"
-        "master/Data/cf-standard-names/current/src/cf-standard-name-table.xml"
-    )
-    expected_info, _, _ = parse_cf_standard_name_table(urlopen(url))
-    actual_info, _, _ = parse_cf_standard_name_table()
-    assert expected_info == actual_info
+    parse_cf_standard_name_table()
 
 
 def test_add_canonical_attributes_0_dim() -> None:
     """test if works for variables with 0 dimension"""
     xr.DataArray(
         0, attrs={"standard_name": "sea_water_potential_temperature"}
     ).cf.add_canonical_attributes()
@@ -1744,15 +1727,14 @@
     assert "units" not in new_attrs and "description" in new_attrs
 
 
 @pytest.mark.parametrize("override", [True, False])
 @pytest.mark.parametrize("skip", ["units", None])
 @pytest.mark.parametrize("verbose", [True, False])
 def test_add_canonical_attributes(override, skip, verbose, capsys):
-
     ds = airds
     original = ds.copy(deep=True)
     cf_ds = ds.cf.add_canonical_attributes(
         override=override, skip=skip, verbose=verbose
     )
 
     # Catch print
@@ -1830,15 +1812,14 @@
         basin_.cf.isin(["pacific_ocean"])
 
     with pytest.raises(ValueError):
         basin_.cf == "pacific_ocean"
 
 
 def test_missing_variables() -> None:
-
     # Bounds
     ds = mollwds.copy(deep=False)
     ds = ds.drop_vars("lon_bounds")
     assert ds.cf.bounds == {"lat": ["lat_bounds"], "latitude": ["lat_bounds"]}
 
     with pytest.raises(KeyError, match=r"No results found for 'longitude'."):
         ds.cf.get_bounds("longitude")
@@ -1874,20 +1855,22 @@
     dsg.foo.cf.plot(x="trajectory_id")
 
 
 def test_grid_topology() -> None:
     ds = xr.Dataset(
         data_vars={},
         coords={
+            "time": ("time", [1, 2, 3], {"standard_name": "time"}),
             "mesh": (tuple(), 1, {"cf_role": "mesh_topology"}),
             "grid": (tuple(), 1, {"cf_role": "grid_topology"}),
         },
     )
     assert_identical(ds.cf["grid_topology"], ds.grid.reset_coords(drop=True))
     assert_identical(ds.cf["mesh_topology"], ds.mesh.reset_coords(drop=True))
+    assert "T" in ds.cf.axes
 
 
 @requires_scipy
 def test_curvefit() -> None:
     from cf_xarray.datasets import airds
 
     def line(time, slope):
```

### Comparing `cf_xarray-0.8.0/cf_xarray/tests/test_coding.py` & `cf_xarray-0.8.1/cf_xarray/tests/test_coding.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/tests/test_geometry.py` & `cf_xarray-0.8.1/cf_xarray/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/tests/test_helpers.py` & `cf_xarray-0.8.1/cf_xarray/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/tests/test_scripts.py` & `cf_xarray-0.8.1/cf_xarray/tests/test_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from tempfile import TemporaryDirectory
 
 from cf_xarray.scripts import make_doc
 
 
 def test_make_doc():
-
     names = [
         "axes_criteria",
         "coords_criteria",
         "all_criteria",
         "all_regex",
     ]
     tables_to_check = [f"_build/csv/{name}.csv" for name in names]
```

### Comparing `cf_xarray-0.8.0/cf_xarray/tests/test_units.py` & `cf_xarray-0.8.1/cf_xarray/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/units.py` & `cf_xarray-0.8.1/cf_xarray/units.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/cf_xarray/utils.py` & `cf_xarray-0.8.1/cf_xarray/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from collections import defaultdict
 from typing import Any, Dict, Iterable
 from xml.etree import ElementTree
 
 import numpy as np
 from xarray import DataArray
 
@@ -79,16 +78,20 @@
     return [obj] if not isinstance(obj, allowed) else obj
 
 
 def parse_cf_standard_name_table(source=None):
     """"""
 
     if not source:
-        source = os.path.join(
-            os.path.dirname(__file__), "data", "cf-standard-name-table.xml"
+        import pooch
+
+        source = pooch.retrieve(
+            "https://raw.githubusercontent.com/cf-convention/cf-convention.github.io/"
+            "master/Data/cf-standard-names/current/src/cf-standard-name-table.xml",
+            known_hash=None,
         )
     root = ElementTree.parse(source).getroot()
 
     # Build dictionaries
     info = {}
     table: dict = {}
     aliases = {}
```

### Comparing `cf_xarray-0.8.0/cf_xarray.egg-info/PKG-INFO` & `cf_xarray-0.8.1/cf_xarray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cf-xarray
-Version: 0.8.0
+Version: 0.8.1
 Summary: A convenience wrapper for using CF attributes on xarray objects
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cf_xarray-0.8.0/cf_xarray.egg-info/SOURCES.txt` & `cf_xarray-0.8.1/cf_xarray.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 cf_xarray/units.py
 cf_xarray/utils.py
 cf_xarray.egg-info/PKG-INFO
 cf_xarray.egg-info/SOURCES.txt
 cf_xarray.egg-info/dependency_links.txt
 cf_xarray.egg-info/requires.txt
 cf_xarray.egg-info/top_level.txt
-cf_xarray/data/cf-standard-name-table.xml
 cf_xarray/scripts/make_doc.py
 cf_xarray/scripts/print_versions.py
 cf_xarray/tests/__init__.py
 cf_xarray/tests/test_accessor.py
 cf_xarray/tests/test_coding.py
 cf_xarray/tests/test_geometry.py
 cf_xarray/tests/test_helpers.py
```

### Comparing `cf_xarray-0.8.0/doc/2D_bounds_averaged.png` & `cf_xarray-0.8.1/doc/2D_bounds_averaged.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/2D_bounds_error.png` & `cf_xarray-0.8.1/doc/2D_bounds_error.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/2D_bounds_nonunique.png` & `cf_xarray-0.8.1/doc/2D_bounds_nonunique.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/Makefile` & `cf_xarray-0.8.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/_static/dataset-diagram-logo.tex` & `cf_xarray-0.8.1/doc/_static/dataset-diagram-logo.tex`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/_static/full-logo.png` & `cf_xarray-0.8.1/doc/_static/full-logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/_static/logo.png` & `cf_xarray-0.8.1/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/_static/logo.svg` & `cf_xarray-0.8.1/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/_static/rich-repr-example.png` & `cf_xarray-0.8.1/doc/_static/rich-repr-example.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/api.rst` & `cf_xarray-0.8.1/doc/api.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/bounds.md` & `cf_xarray-0.8.1/doc/bounds.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/cartopy_rotated_pole.png` & `cf_xarray-0.8.1/doc/cartopy_rotated_pole.png`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/coding.md` & `cf_xarray-0.8.1/doc/coding.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/conf.py` & `cf_xarray-0.8.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/contributing.rst` & `cf_xarray-0.8.1/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/coord_axes.md` & `cf_xarray-0.8.1/doc/coord_axes.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/custom-criteria.md` & `cf_xarray-0.8.1/doc/custom-criteria.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/dsg.md` & `cf_xarray-0.8.1/doc/dsg.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/examples/introduction.ipynb` & `cf_xarray-0.8.1/doc/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/flags.md` & `cf_xarray-0.8.1/doc/flags.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/grid_mappings.md` & `cf_xarray-0.8.1/doc/grid_mappings.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/howtouse.md` & `cf_xarray-0.8.1/doc/howtouse.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/index.rst` & `cf_xarray-0.8.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/make.bat` & `cf_xarray-0.8.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/parametricz.md` & `cf_xarray-0.8.1/doc/parametricz.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/plotting.md` & `cf_xarray-0.8.1/doc/plotting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/provenance.md` & `cf_xarray-0.8.1/doc/provenance.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/quickstart.md` & `cf_xarray-0.8.1/doc/quickstart.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/roadmap.rst` & `cf_xarray-0.8.1/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/selecting.md` & `cf_xarray-0.8.1/doc/selecting.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/sgrid_ugrid.md` & `cf_xarray-0.8.1/doc/sgrid_ugrid.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/units.md` & `cf_xarray-0.8.1/doc/units.md`

 * *Files identical despite different names*

### Comparing `cf_xarray-0.8.0/doc/whats-new.rst` & `cf_xarray-0.8.1/doc/whats-new.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 .. currentmodule:: xarray
 
 What's New
 ----------
 
+v0.8.1 (May 9, 2023)
+====================
+- Stop bundling the standard name table and use ``pooch`` (new optional dependency) to download when needed.
+  By `Deepak Cherian`_.
+- Major performance improvements.  By `Deepak Cherian`_.
+- Fix bug where code was looking for ``T`` axis in SGRID info.
+  By `Kristen Thyng`_.
+- Support ``X``, ``Y`` for rotated pole grids.  By `Lars Buntemeyer`_.
+
+
 v0.8.0 (Feb 8, 2023)
 ====================
 
 - Support interpreting `SGRID Conventions <https://sgrid.github.io/sgrid/>`_ to identify
   X, Y, Z axes. By `Deepak Cherian`_.
 - Add a `rich <https://rich.readthedocs.io>`_ repr. (:pr:`409`).
   Use ``rich.print(ds.cf)`` or ``%load_ext rich`` in a Jupyter session to
```

### Comparing `cf_xarray-0.8.0/pyproject.toml` & `cf_xarray-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 dependencies = [
     "xarray",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
-all = ["matplotlib", "pint", "shapely", "regex", "rich"]
+all = ["matplotlib", "pint", "shapely", "regex", "rich", "pooch"]
 
 [project.urls]
 homepage = "https://cf-xarray.readthedocs.io"
 documentation = "https://cf-xarray.readthedocs.io"
 repository = "https://github.com/xarray-contrib/cf-xarray.git"
 changelog = "https://cf-xarray.readthedocs.io/en/latest/whats-new.html"
 
@@ -37,15 +37,15 @@
     "setuptools>=45",
     "wheel",
     "setuptools_scm[toml]>=6.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-packages = ["cf_xarray", "cf_xarray.data", "cf_xarray.scripts"]
+packages = ["cf_xarray", "cf_xarray.scripts"]
 
 [tool.setuptools.exclude-package-data]
 cf_xarray = ["tests/*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "cf_xarray.__version__"}
 
@@ -125,13 +125,14 @@
 show_error_codes = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module=[
     "cftime",
     "pandas",
+    "pooch",
     "matplotlib",
     "pytest",
     "shapely.geometry",
     "xarray.core.pycompat",
 ]
 ignore_missing_imports = true
```

