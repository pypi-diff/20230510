# Comparing `tmp/pyikarus-0.3.0.dev202310000052.tar.gz` & `tmp/pyikarus-0.3.0.dev202310000053.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.0.dev202310000052.tar", last modified: Wed May 10 12:08:37 2023, max compression
+gzip compressed data, was "pyikarus-0.3.0.dev202310000053.tar", last modified: Wed May 10 12:10:54 2023, max compression
```

## Comparing `pyikarus-0.3.0.dev202310000052.tar` & `pyikarus-0.3.0.dev202310000053.tar`

### file list

```diff
@@ -1,25 +1,309 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:08:37.204333 pyikarus-0.3.0.dev202310000052/
--rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000052/LICENSE.md
--rw-r--r--   0 user      (1001) user      (1001)        0 2023-05-10 11:40:26.000000 pyikarus-0.3.0.dev202310000052/MANIFEST.in
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 12:08:37.202036 pyikarus-0.3.0.dev202310000052/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000052/README.md
--rwxrwxrwx   0 user      (1001) user      (1001)      305 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000052/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:08:36.891404 pyikarus-0.3.0.dev202310000052/python/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:08:37.010359 pyikarus-0.3.0.dev202310000052/python/pyikarus/
--rwxrwxrwx   0 user      (1001) user      (1001)      584 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus/__init__.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:08:37.131184 pyikarus-0.3.0.dev202310000052/python/pyikarus/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)     2310 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus/assembler/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1412 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus/dirichletValues.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:08:37.154006 pyikarus-0.3.0.dev202310000052/python/pyikarus/finite_elements/
--rwxrwxrwx   0 user      (1001) user      (1001)     3473 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus/finite_elements/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1796 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus/materials.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:08:37.179857 pyikarus-0.3.0.dev202310000052/python/pyikarus/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)     1463 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus/utils/__init__.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:08:37.107300 pyikarus-0.3.0.dev202310000052/python/pyikarus.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 12:08:36.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)      458 2023-05-10 12:08:36.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-10 12:08:36.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-10 12:08:36.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 user      (1001) user      (1001)        9 2023-05-10 12:08:36.000000 pyikarus-0.3.0.dev202310000052/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-10 12:08:37.204841 pyikarus-0.3.0.dev202310000052/setup.cfg
--rwxrwxrwx   0 user      (1001) user      (1001)     1381 2023-05-10 12:07:29.000000 pyikarus-0.3.0.dev202310000052/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:54.262342 pyikarus-0.3.0.dev202310000053/
+-rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.bettercodehub.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1300 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.clang-format
+-rwxrwxrwx   0 user      (1001) user      (1001)     1017 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.cmake-format
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:49.738479 pyikarus-0.3.0.dev202310000053/.github/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.216058 pyikarus-0.3.0.dev202310000053/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      615 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.357741 pyikarus-0.3.0.dev202310000053/.github/workflows/
+-rwxrwxrwx   0 user      (1001) user      (1001)      476 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/codespell.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1034 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/createDockerContainer.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     4900 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/createRelease.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1635 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/debian-coverage.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2108 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/debian.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/ghpages.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/reuseLint.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2854 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/runExamples.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1212 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.github/workflows/style.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      456 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/.gitignore
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.369760 pyikarus-0.3.0.dev202310000053/.reuse/
+-rwxrwxrwx   0 user      (1001) user      (1001)      661 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/.reuse/dep5
+-rwxrwxrwx   0 user      (1001) user      (1001)     3063 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/CHANGELOG.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1323 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5335 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/LICENSE.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.419032 pyikarus-0.3.0.dev202310000053/LICENSES/
+-rwxrwxrwx   0 user      (1001) user      (1001)    18375 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/LICENSES/CC-BY-SA-4.0.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     7048 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/LICENSES/CC0-1.0.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    42098 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/LICENSES/LGPL-3.0-or-later.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    16727 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 12:10:54.260454 pyikarus-0.3.0.dev202310000053/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/README.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.446355 pyikarus-0.3.0.dev202310000053/cmake/
+-rwxrwxrwx   0 user      (1001) user      (1001)      973 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/CPM.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.461555 pyikarus-0.3.0.dev202310000053/cmake/FormatTarget/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1270 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.559747 pyikarus-0.3.0.dev202310000053/cmake/modules/
+-rwxrwxrwx   0 user      (1001) user      (1001)      715 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/modules/AddAutoDiffFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      683 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/modules/AddEigenFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      740 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/modules/AddMatplotppFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      691 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/modules/AddSpdlogFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      226 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/modules/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      446 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/modules/IkarusMacros.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)     2040 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/cmake/tools.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      148 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/codecov.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/codespellignore
+-rwxrwxrwx   0 user      (1001) user      (1001)     1618 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/config.h.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.635442 pyikarus-0.3.0.dev202310000053/docs/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.650603 pyikarus-0.3.0.dev202310000053/docs/BuildLocally/
+-rwxrwxrwx   0 user      (1001) user      (1001)      439 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/BuildLocally/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      333 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.686478 pyikarus-0.3.0.dev202310000053/docs/__pycache__/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1136 2023-04-21 10:05:27.000000 pyikarus-0.3.0.dev202310000053/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     6961 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/literature.bib
+-rwxrwxrwx   0 user      (1001) user      (1001)      117 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/literature.bib.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     1245 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/mkdocs-macros.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      394 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/mkdocs.insiders.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     5042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/mkdocs.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:49.770829 pyikarus-0.3.0.dev202310000053/docs/overrides/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.704922 pyikarus-0.3.0.dev202310000053/docs/overrides/partials/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1732 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/overrides/partials/comments.html
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:50.772820 pyikarus-0.3.0.dev202310000053/docs/website/
+-rwxrwxrwx   0 user      (1001) user      (1001)       24 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/.meta.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.031258 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/
+-rwxrwxrwx   0 user      (1001) user      (1001)     4710 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/assembler.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     6387 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/controlRoutines.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2024 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/dirichletBCs.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3237 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/feRequirements.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     8527 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/finiteElements.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2745 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/grids.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/index.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4932 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/localBasis.md
+-rwxrwxrwx   0 user      (1001) user      (1001)    44233 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/localFunctions.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3978 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/manifolds.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2590 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/nonlinearOperator.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3086 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/observer.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5211 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.216749 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/
+-rwxrwxrwx   0 user      (1001) user      (1001)     6675 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/cantileverBeam.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7271 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/computePi.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5477 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/cooksMembrane.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7051 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/incompressibleRubberBlock.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2164 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/index.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7719 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/kirchhoffPlate.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5134 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/newtonRaphsonMethod.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     6149 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/nonLinearElasticity.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4090 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.300089 pyikarus-0.3.0.dev202310000053/docs/website/03_contribution/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/03_contribution/buildDocumentationLocally.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1002 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/03_contribution/codeStyle.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2415 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/03_contribution/howToEdit.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1762 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.333505 pyikarus-0.3.0.dev202310000053/docs/website/04_blog/
+-rwxrwxrwx   0 user      (1001) user      (1001)      274 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/04_blog/.authors.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/04_blog/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.357084 pyikarus-0.3.0.dev202310000053/docs/website/04_blog/posts/
+-rwxrwxrwx   0 user      (1001) user      (1001)     7731 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.376728 pyikarus-0.3.0.dev202310000053/docs/website/05_cppReferences/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2324 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.396306 pyikarus-0.3.0.dev202310000053/docs/website/99_Literature/
+-rwxrwxrwx   0 user      (1001) user      (1001)      169 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.464901 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.657254 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/
+-rwxrwxrwx   0 user      (1001) user      (1001)    52795 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    46250 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     2852 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    17924 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     9455 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     8101 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/logo_blue.svg
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/logo_blue.svg.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     8255 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/logo_white.svg
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/auxiliaryImages/logo_white.svg.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     4364 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/download.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/gallery.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1358 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.673167 pyikarus-0.3.0.dev202310000053/docs/website/javascripts/
+-rwxrwxrwx   0 user      (1001) user      (1001)      486 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.688998 pyikarus-0.3.0.dev202310000053/docs/website/stylesheets/
+-rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/docs/website/stylesheets/extra.css
+-rwxrwxrwx   0 user      (1001) user      (1001)      504 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/dune.module
+-rwxrwxrwx   0 user      (1001) user      (1001)      196 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/iwyu.imp
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.702743 pyikarus-0.3.0.dev202310000053/pyikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      748 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.744778 pyikarus-0.3.0.dev202310000053/pyikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      270 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    11016 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/assembler/simpleAssemblers.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    10681 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.786411 pyikarus-0.3.0.dev202310000053/pyikarus/controlRoutines/
+-rwxrwxrwx   0 user      (1001) user      (1001)      241 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/controlRoutines/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2583 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/controlRoutines/loadControl.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2980 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.878020 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      351 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      185 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:51.952879 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/feBases/
+-rwxrwxrwx   0 user      (1001) user      (1001)      284 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/feBases/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2653 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/feBases/autodiffFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2153 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/feBases/powerBasisFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1703 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/feBases/scalarFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1041 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/feRequirements.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     8419 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/feRequirements.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1340 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.054668 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/
+-rwxrwxrwx   0 user      (1001) user      (1001)      347 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    20315 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12771 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.241833 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/
+-rwxrwxrwx   0 user      (1001) user      (1001)      399 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5709 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/interface.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2720 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     4637 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/neohooke.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3811 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5736 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/svk.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      475 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/tags.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     8014 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1208 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/materials.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     7984 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12655 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.317849 pyikarus-0.3.0.dev202310000053/pyikarus/linearAlgebra/
+-rwxrwxrwx   0 user      (1001) user      (1001)      303 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/linearAlgebra/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     6452 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/linearAlgebra/dirichletValues.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     7793 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/linearAlgebra/nonLinearOperator.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12303 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.333602 pyikarus-0.3.0.dev202310000053/pyikarus/python/
+-rwxrwxrwx   0 user      (1001) user      (1001)      270 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.370685 pyikarus-0.3.0.dev202310000053/pyikarus/python/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      251 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3117 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.405698 pyikarus-0.3.0.dev202310000053/pyikarus/python/dirichletValues/
+-rwxrwxrwx   0 user      (1001) user      (1001)      259 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/dirichletValues/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     4118 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.462724 pyikarus-0.3.0.dev202310000053/pyikarus/python/finiteElements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      305 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/finiteElements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5528 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.506538 pyikarus-0.3.0.dev202310000053/pyikarus/python/finiteElements/materials/
+-rwxrwxrwx   0 user      (1001) user      (1001)      261 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/finiteElements/materials/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5113 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/finiteElements/materials/material.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5421 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.659660 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/
+-rwxrwxrwx   0 user      (1001) user      (1001)      787 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3820 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/linearElasticTest.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1839 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/nameTest.vtu
+-rwxrwxrwx   0 user      (1001) user      (1001)     4462 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/nonLinearElasticTest.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      866 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/setpath.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      862 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/setpath.py.in
+-rwxrwxrwx   0 user      (1001) user      (1001)      327 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/test1.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      586 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/test/test2.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.696504 pyikarus-0.3.0.dev202310000053/pyikarus/python/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      247 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1436 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.711404 pyikarus-0.3.0.dev202310000053/pyikarus/solver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      211 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.744304 pyikarus-0.3.0.dev202310000053/pyikarus/solver/linearSolver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      246 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/solver/linearSolver/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     8891 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:52.827152 pyikarus-0.3.0.dev202310000053/pyikarus/solver/nonLinearSolver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      274 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/solver/nonLinearSolver/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5419 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     8309 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    18586 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.154733 pyikarus-0.3.0.dev202310000053/pyikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      673 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1741 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/algorithms.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      878 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/autodiffHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     6930 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/concepts.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      503 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.234568 pyikarus-0.3.0.dev202310000053/pyikarus/utils/drawing/
+-rwxrwxrwx   0 user      (1001) user      (1001)      264 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/drawing/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1654 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/drawing/griddrawer.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      544 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/drawing/matplotHelper.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      703 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/drawing/matplotHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2484 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/duneUtilities.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2347 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/eigenDuneTransformations.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      682 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/eigenSparseAddon.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1367 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/findLineSegment.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/findLineSegment.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2171 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/functionSanityChecks.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6359 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/functionSanityChecks.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3154 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/init.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    15244 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/linearAlgebraHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1711 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/makeEnum.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.416108 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/
+-rwxrwxrwx   0 user      (1001) user      (1001)      452 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1558 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/controlLogger.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2307 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/controlVTKWriter.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      909 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/genericControlObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1059 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/gridDrawerObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1136 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/loadControlObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1985 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/nonLinearSolverLogger.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5499 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/observer.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      489 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/observer/observerMessages.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     4161 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/pathFollowingFunctions.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1131 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/polyfit.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      570 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/polyfit.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    10056 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/tensorUtils.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    15044 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus/utils/traits.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      432 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/pyikarus.pc.in
+-rwxrwxrwx   0 user      (1001) user      (1001)      305 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/pyproject.toml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.441729 pyikarus-0.3.0.dev202310000053/python/
+-rwxrwxrwx   0 user      (1001) user      (1001)      407 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.516744 pyikarus-0.3.0.dev202310000053/python/pyikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      523 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      584 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     5644 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/_pyikarus.cc
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.625118 pyikarus-0.3.0.dev202310000053/python/pyikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      167 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2310 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/assembler/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1412 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/dirichletValues.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.661532 pyikarus-0.3.0.dev202310000053/python/pyikarus/finite_elements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      173 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/finite_elements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3473 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/finite_elements/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1796 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/materials.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.697694 pyikarus-0.3.0.dev202310000053/python/pyikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      163 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1463 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus/utils/__init__.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.591640 pyikarus-0.3.0.dev202310000053/python/pyikarus.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 12:10:48.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)     9269 2023-05-10 12:10:49.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-10 12:10:48.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-10 12:10:48.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) user      (1001)        9 2023-05-10 12:10:48.000000 pyikarus-0.3.0.dev202310000053/python/pyikarus.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      638 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/python/setup.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.709539 pyikarus-0.3.0.dev202310000053/sandbox/
+-rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/sandbox/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.734633 pyikarus-0.3.0.dev202310000053/sandbox/src/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1222 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.749917 pyikarus-0.3.0.dev202310000053/sandbox/src/auxiliaryFiles/
+-rwxrwxrwx   0 user      (1001) user      (1001)   674469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/sandbox/src/auxiliaryFiles/circle.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      322 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/sandbox/src/sandbox.cpp
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-10 12:10:54.262851 pyikarus-0.3.0.dev202310000053/setup.cfg
+-rwxrwxrwx   0 user      (1001) user      (1001)     1381 2023-05-10 12:10:46.000000 pyikarus-0.3.0.dev202310000053/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:53.767027 pyikarus-0.3.0.dev202310000053/tests/
+-rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/tests/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:54.140728 pyikarus-0.3.0.dev202310000053/tests/src/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1397 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/tests/src/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3896 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/assemblerTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     9923 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/common.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2641 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/dependenciesTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6417 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/dirichletValueTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     3822 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/easTest.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1479 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/enhancedAssumedStrainsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      608 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/tests/src/factories.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1872 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/functionTraitsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     2225 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/linearElasticityTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     2382 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/manifoldsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     7971 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/materialTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6583 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/nonLinearElasticityTest.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/tests/src/nonLinearElasticityTestNeoHooke.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      729 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/tests/src/nonLinearElasticityTestSVK.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     9946 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/nonLinearOperatorTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6341 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/pathFollowingTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     1655 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/polyFitTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      699 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/pythonConversionTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     1296 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/testAutodiffHelper.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     5710 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/testFEElement.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 12:10:54.240581 pyikarus-0.3.0.dev202310000053/tests/src/testFiles/
+-rwxrwxrwx   0 user      (1001) user      (1001)     9028 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000053/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      395 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000053/tests/src/testFiles/unstructuredTest.geo
+-rwxrwxrwx   0 user      (1001) user      (1001)      497 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000053/tests/src/testFiles/unstructuredTest.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      546 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000053/tests/src/testFiles/unstructuredTest2.geo
+-rwxrwxrwx   0 user      (1001) user      (1001)    11431 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000053/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1114 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000053/tests/src/testHelpers.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    17601 2023-05-10 12:06:58.000000 pyikarus-0.3.0.dev202310000053/tests/src/trustRegionTest.cpp
```

### Comparing `pyikarus-0.3.0.dev202310000052/LICENSE.md` & `pyikarus-0.3.0.dev202310000053/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000052/PKG-INFO` & `pyikarus-0.3.0.dev202310000053/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000052
+Version: 0.3.0.dev202310000053
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000052 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000053 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000052/README.md` & `pyikarus-0.3.0.dev202310000053/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000052/python/pyikarus/__init__.py` & `pyikarus-0.3.0.dev202310000053/python/pyikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000052/python/pyikarus/assembler/__init__.py` & `pyikarus-0.3.0.dev202310000053/python/pyikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000052/python/pyikarus/dirichletValues.py` & `pyikarus-0.3.0.dev202310000053/python/pyikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000052/python/pyikarus/finite_elements/__init__.py` & `pyikarus-0.3.0.dev202310000053/python/pyikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000052/python/pyikarus/materials.py` & `pyikarus-0.3.0.dev202310000053/python/pyikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000052/python/pyikarus/utils/__init__.py` & `pyikarus-0.3.0.dev202310000053/python/pyikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000052/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.0.dev202310000053/python/pyikarus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000052
+Version: 0.3.0.dev202310000053
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000052 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000053 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000052/setup.py` & `pyikarus-0.3.0.dev202310000053/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 # You are logged in as $(whoami)
 # EOF
 # nano ~/.pypirc
 # python -m venv /dune/dune-common/build-cmake/dune-env/
 # source /dune/dune-common/build-cmake/dune-env/bin/activate
 # pip install pyikarus  --no-build-isolation
 
-pyikarusVersion = "0.3.0.dev202310000052" #+ datetime.today().time().strftime("%H%M%S")
+pyikarusVersion = "0.3.0.dev202310000053" #+ datetime.today().time().strftime("%H%M%S")
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = pyikarusVersion
 
 setup(**metadata)
```

