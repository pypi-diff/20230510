# Comparing `tmp/pyikarus-0.3.0.dev202310000056.tar.gz` & `tmp/pyikarus-0.3.0.dev202310000057.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.0.dev202310000056.tar", last modified: Wed May 10 13:20:05 2023, max compression
+gzip compressed data, was "pyikarus-0.3.0.dev202310000057.tar", last modified: Wed May 10 13:28:58 2023, max compression
```

## Comparing `pyikarus-0.3.0.dev202310000056.tar` & `pyikarus-0.3.0.dev202310000057.tar`

### file list

```diff
@@ -1,319 +1,319 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:05.237510 pyikarus-0.3.0.dev202310000056/
--rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.bettercodehub.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1300 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.clang-format
--rwxrwxrwx   0 user      (1001) user      (1001)     1017 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.cmake-format
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:19:59.789809 pyikarus-0.3.0.dev202310000056/.github/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.263944 pyikarus-0.3.0.dev202310000056/.github/ISSUE_TEMPLATE/
--rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/ISSUE_TEMPLATE/bug_report.md
--rwxrwxrwx   0 user      (1001) user      (1001)      615 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.421338 pyikarus-0.3.0.dev202310000056/.github/workflows/
--rwxrwxrwx   0 user      (1001) user      (1001)      476 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/codespell.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1034 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/createDockerContainer.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     4900 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/createRelease.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1635 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/debian-coverage.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2108 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/debian.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/ghpages.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/reuseLint.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     2854 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/runExamples.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     1212 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.github/workflows/style.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      455 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/.gitignore
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.435734 pyikarus-0.3.0.dev202310000056/.reuse/
--rwxrwxrwx   0 user      (1001) user      (1001)      661 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/.reuse/dep5
--rwxrwxrwx   0 user      (1001) user      (1001)     3063 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/CHANGELOG.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1319 2023-05-10 12:56:29.000000 pyikarus-0.3.0.dev202310000056/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5335 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/CODE_OF_CONDUCT.md
--rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/LICENSE.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.487925 pyikarus-0.3.0.dev202310000056/LICENSES/
--rwxrwxrwx   0 user      (1001) user      (1001)    18375 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/LICENSES/CC-BY-SA-4.0.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     7048 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/LICENSES/CC0-1.0.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    42098 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/LICENSES/LGPL-3.0-or-later.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    16727 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/LICENSES/MPL-2.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 13:20:05.234761 pyikarus-0.3.0.dev202310000056/PKG-INFO
--rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/README.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.514087 pyikarus-0.3.0.dev202310000056/cmake/
--rwxrwxrwx   0 user      (1001) user      (1001)      973 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/CPM.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.530250 pyikarus-0.3.0.dev202310000056/cmake/FormatTarget/
--rwxrwxrwx   0 user      (1001) user      (1001)     1270 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.626167 pyikarus-0.3.0.dev202310000056/cmake/modules/
--rwxrwxrwx   0 user      (1001) user      (1001)      715 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/modules/AddAutoDiffFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      683 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/modules/AddEigenFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      740 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/modules/AddMatplotppFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      691 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/modules/AddSpdlogFlags.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      226 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/modules/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      446 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/modules/IkarusMacros.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)     2040 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/cmake/tools.cmake
--rwxrwxrwx   0 user      (1001) user      (1001)      148 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/codecov.yml
--rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/codespellignore
--rwxrwxrwx   0 user      (1001) user      (1001)     1588 2023-05-10 12:14:52.000000 pyikarus-0.3.0.dev202310000056/config.h.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.709465 pyikarus-0.3.0.dev202310000056/docs/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.725093 pyikarus-0.3.0.dev202310000056/docs/BuildLocally/
--rwxrwxrwx   0 user      (1001) user      (1001)      439 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/BuildLocally/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      333 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.759522 pyikarus-0.3.0.dev202310000056/docs/__pycache__/
--rwxrwxrwx   0 user      (1001) user      (1001)     1136 2023-04-21 10:05:27.000000 pyikarus-0.3.0.dev202310000056/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rwxrwxrwx   0 user      (1001) user      (1001)     6961 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/literature.bib
--rwxrwxrwx   0 user      (1001) user      (1001)      117 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/literature.bib.license
--rwxrwxrwx   0 user      (1001) user      (1001)     1245 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/mkdocs-macros.py
--rwxrwxrwx   0 user      (1001) user      (1001)      394 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/mkdocs.insiders.yml
--rwxrwxrwx   0 user      (1001) user      (1001)     5042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/mkdocs.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:19:59.820590 pyikarus-0.3.0.dev202310000056/docs/overrides/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.779168 pyikarus-0.3.0.dev202310000056/docs/overrides/partials/
--rwxrwxrwx   0 user      (1001) user      (1001)     1732 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/overrides/partials/comments.html
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:00.848058 pyikarus-0.3.0.dev202310000056/docs/website/
--rwxrwxrwx   0 user      (1001) user      (1001)       24 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/.meta.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:01.158086 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/
--rwxrwxrwx   0 user      (1001) user      (1001)     4710 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/assembler.md
--rwxrwxrwx   0 user      (1001) user      (1001)     6387 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/controlRoutines.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2024 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/dirichletBCs.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3237 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/feRequirements.md
--rwxrwxrwx   0 user      (1001) user      (1001)     8527 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/finiteElements.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2745 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/grids.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/index.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4932 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/localBasis.md
--rwxrwxrwx   0 user      (1001) user      (1001)    44233 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/localFunctions.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3978 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/manifolds.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2590 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/nonlinearOperator.md
--rwxrwxrwx   0 user      (1001) user      (1001)     3086 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/observer.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5211 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:01.396411 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/
--rwxrwxrwx   0 user      (1001) user      (1001)     6675 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/cantileverBeam.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7271 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/computePi.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5477 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/cooksMembrane.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7051 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/incompressibleRubberBlock.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2164 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/index.md
--rwxrwxrwx   0 user      (1001) user      (1001)     7719 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/kirchhoffPlate.md
--rwxrwxrwx   0 user      (1001) user      (1001)     5134 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/newtonRaphsonMethod.md
--rwxrwxrwx   0 user      (1001) user      (1001)     6149 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/nonLinearElasticity.md
--rwxrwxrwx   0 user      (1001) user      (1001)     4090 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:01.481330 pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/
--rwxrwxrwx   0 user      (1001) user      (1001)     2439 2023-05-10 12:50:55.000000 pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/buildDocumentationLocally.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1002 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/codeStyle.md
--rwxrwxrwx   0 user      (1001) user      (1001)     2415 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/howToEdit.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1762 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:01.526525 pyikarus-0.3.0.dev202310000056/docs/website/04_blog/
--rwxrwxrwx   0 user      (1001) user      (1001)      274 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/04_blog/.authors.yml
--rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/04_blog/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:01.551218 pyikarus-0.3.0.dev202310000056/docs/website/04_blog/posts/
--rwxrwxrwx   0 user      (1001) user      (1001)     7731 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:01.574464 pyikarus-0.3.0.dev202310000056/docs/website/05_cppReferences/
--rwxrwxrwx   0 user      (1001) user      (1001)     2324 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:01.598307 pyikarus-0.3.0.dev202310000056/docs/website/99_Literature/
--rwxrwxrwx   0 user      (1001) user      (1001)      169 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:01.704036 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.004013 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/
--rwxrwxrwx   0 user      (1001) user      (1001)    52795 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    46250 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     2852 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    17924 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     9455 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.298465 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/
--rwxrwxrwx   0 user      (1001) user      (1001)    35234 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    62184 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     2281 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    40033 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)    25505 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rwxrwxrwx   0 user      (1001) user      (1001)     8101 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/logo_blue.svg
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/logo_blue.svg.license
--rwxrwxrwx   0 user      (1001) user      (1001)     8255 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/logo_white.svg
--rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/logo_white.svg.license
--rwxrwxrwx   0 user      (1001) user      (1001)     4364 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/download.md
--rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/gallery.md
--rwxrwxrwx   0 user      (1001) user      (1001)     1358 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.321740 pyikarus-0.3.0.dev202310000056/docs/website/javascripts/
--rwxrwxrwx   0 user      (1001) user      (1001)      486 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.343741 pyikarus-0.3.0.dev202310000056/docs/website/stylesheets/
--rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/docs/website/stylesheets/extra.css
--rwxrwxrwx   0 user      (1001) user      (1001)      502 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/dune.module
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.357741 pyikarus-0.3.0.dev202310000056/ikarus/
--rwxrwxrwx   0 user      (1001) user      (1001)      748 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.414337 pyikarus-0.3.0.dev202310000056/ikarus/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      268 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    11012 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/assembler/simpleAssemblers.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    10681 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.459634 pyikarus-0.3.0.dev202310000056/ikarus/controlRoutines/
--rwxrwxrwx   0 user      (1001) user      (1001)      239 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/controlRoutines/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2575 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/controlRoutines/loadControl.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2970 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.557514 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/
--rwxrwxrwx   0 user      (1001) user      (1001)      349 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      185 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.629045 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feBases/
--rwxrwxrwx   0 user      (1001) user      (1001)      282 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feBases/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2649 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feBases/autodiffFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2151 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feBases/powerBasisFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1701 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feBases/scalarFE.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1041 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feRequirements.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     8419 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feRequirements.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1338 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.719674 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/
--rwxrwxrwx   0 user      (1001) user      (1001)      345 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)    20311 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12753 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:02.932220 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/
--rwxrwxrwx   0 user      (1001) user      (1001)      397 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5699 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/interface.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2718 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     4635 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     3809 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5734 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/svk.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      473 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/tags.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     8010 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1196 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     7966 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12655 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.008796 pyikarus-0.3.0.dev202310000056/ikarus/linearAlgebra/
--rwxrwxrwx   0 user      (1001) user      (1001)      301 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/linearAlgebra/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     6448 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/linearAlgebra/dirichletValues.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     7791 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/linearAlgebra/nonLinearOperator.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    12303 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.027604 pyikarus-0.3.0.dev202310000056/ikarus/python/
--rwxrwxrwx   0 user      (1001) user      (1001)      270 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.072976 pyikarus-0.3.0.dev202310000056/ikarus/python/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      249 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3115 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.120112 pyikarus-0.3.0.dev202310000056/ikarus/python/dirichletValues/
--rwxrwxrwx   0 user      (1001) user      (1001)      257 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/dirichletValues/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     4116 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.196041 pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/
--rwxrwxrwx   0 user      (1001) user      (1001)      303 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5526 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.257381 pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/materials/
--rwxrwxrwx   0 user      (1001) user      (1001)      259 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/materials/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5107 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/materials/material.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5419 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.420028 pyikarus-0.3.0.dev202310000056/ikarus/python/test/
--rwxrwxrwx   0 user      (1001) user      (1001)      787 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/test/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3808 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/test/linearElasticTest.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1839 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/test/nameTest.vtu
--rwxrwxrwx   0 user      (1001) user      (1001)     4444 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/test/nonLinearElasticTest.py
--rwxrwxrwx   0 user      (1001) user      (1001)      862 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/test/setpath.py.in
--rwxrwxrwx   0 user      (1001) user      (1001)      321 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/test/test1.py
--rwxrwxrwx   0 user      (1001) user      (1001)      582 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/test/test2.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.464792 pyikarus-0.3.0.dev202310000056/ikarus/python/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      245 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1434 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.483489 pyikarus-0.3.0.dev202310000056/ikarus/solver/
--rwxrwxrwx   0 user      (1001) user      (1001)      211 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.521929 pyikarus-0.3.0.dev202310000056/ikarus/solver/linearSolver/
--rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/solver/linearSolver/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     8891 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.613691 pyikarus-0.3.0.dev202310000056/ikarus/solver/nonLinearSolver/
--rwxrwxrwx   0 user      (1001) user      (1001)      272 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     5407 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     8297 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    18574 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:03.973157 pyikarus-0.3.0.dev202310000056/ikarus/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      671 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1741 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/algorithms.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      878 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/autodiffHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     6930 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/concepts.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      503 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.058270 pyikarus-0.3.0.dev202310000056/ikarus/utils/drawing/
--rwxrwxrwx   0 user      (1001) user      (1001)      262 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/drawing/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1654 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/drawing/griddrawer.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      544 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/drawing/matplotHelper.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      703 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/drawing/matplotHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2484 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/duneUtilities.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2347 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/eigenDuneTransformations.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      682 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/eigenSparseAddon.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1367 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/findLineSegment.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/findLineSegment.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2171 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/functionSanityChecks.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6359 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/functionSanityChecks.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     3152 2023-05-10 12:14:52.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/init.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    15244 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/linearAlgebraHelper.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1711 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.246321 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/
--rwxrwxrwx   0 user      (1001) user      (1001)      450 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1554 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/controlLogger.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2307 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/controlVTKWriter.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      905 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/genericControlObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1053 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/gridDrawerObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1132 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/loadControlObserver.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1985 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/nonLinearSolverLogger.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     5497 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/observer.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      489 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/observerMessages.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     4159 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/pathFollowingFunctions.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1131 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/polyfit.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      570 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/polyfit.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    10054 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/tensorUtils.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    15044 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus/utils/traits.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      432 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/ikarus.pc.in
--rwxrwxrwx   0 user      (1001) user      (1001)      196 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/iwyu.imp
--rwxrwxrwx   0 user      (1001) user      (1001)      305 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.280320 pyikarus-0.3.0.dev202310000056/python/
--rwxrwxrwx   0 user      (1001) user      (1001)      403 2023-05-10 12:21:57.000000 pyikarus-0.3.0.dev202310000056/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.367309 pyikarus-0.3.0.dev202310000056/python/ikarus/
--rwxrwxrwx   0 user      (1001) user      (1001)      511 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      578 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     5636 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.409778 pyikarus-0.3.0.dev202310000056/python/ikarus/assembler/
--rwxrwxrwx   0 user      (1001) user      (1001)      167 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/assembler/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     2300 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/assembler/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1408 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.454500 pyikarus-0.3.0.dev202310000056/python/ikarus/finite_elements/
--rwxrwxrwx   0 user      (1001) user      (1001)      173 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/finite_elements/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3465 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/finite_elements/__init__.py
--rwxrwxrwx   0 user      (1001) user      (1001)     1792 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/materials.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.499417 pyikarus-0.3.0.dev202310000056/python/ikarus/utils/
--rwxrwxrwx   0 user      (1001) user      (1001)      163 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/utils/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     1461 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.586462 pyikarus-0.3.0.dev202310000056/python/pyikarus.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 13:19:57.000000 pyikarus-0.3.0.dev202310000056/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)     9785 2023-05-10 13:19:59.000000 pyikarus-0.3.0.dev202310000056/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-10 13:19:57.000000 pyikarus-0.3.0.dev202310000056/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-10 13:19:57.000000 pyikarus-0.3.0.dev202310000056/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 user      (1001) user      (1001)        7 2023-05-10 13:19:57.000000 pyikarus-0.3.0.dev202310000056/python/pyikarus.egg-info/top_level.txt
--rwxrwxrwx   0 user      (1001) user      (1001)      636 2023-05-10 12:27:37.000000 pyikarus-0.3.0.dev202310000056/python/setup.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.599707 pyikarus-0.3.0.dev202310000056/sandbox/
--rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/sandbox/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.632122 pyikarus-0.3.0.dev202310000056/sandbox/src/
--rwxrwxrwx   0 user      (1001) user      (1001)     1220 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.653640 pyikarus-0.3.0.dev202310000056/sandbox/src/auxiliaryFiles/
--rwxrwxrwx   0 user      (1001) user      (1001)   674469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/sandbox/src/auxiliaryFiles/circle.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      320 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/sandbox/src/sandbox.cpp
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-10 13:20:05.238017 pyikarus-0.3.0.dev202310000056/setup.cfg
--rwxrwxrwx   0 user      (1001) user      (1001)     1683 2023-05-10 13:19:55.000000 pyikarus-0.3.0.dev202310000056/setup.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:04.678555 pyikarus-0.3.0.dev202310000056/tests/
--rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/tests/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:05.097408 pyikarus-0.3.0.dev202310000056/tests/src/
--rwxrwxrwx   0 user      (1001) user      (1001)     1397 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/tests/src/CMakeLists.txt
--rwxrwxrwx   0 user      (1001) user      (1001)     3888 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/assemblerTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     9913 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/common.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     2639 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/dependenciesTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6409 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/dirichletValueTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     3820 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/easTest.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1473 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/enhancedAssumedStrainsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      608 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/tests/src/factories.hh
--rwxrwxrwx   0 user      (1001) user      (1001)     1870 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/functionTraitsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     2221 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/linearElasticityTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     2378 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/manifoldsTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     7961 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/materialTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6561 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/nonLinearElasticityTest.hh
--rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      729 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/tests/src/nonLinearElasticityTestSVK.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     9936 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/nonLinearOperatorTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     6327 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/pathFollowingTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     1651 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/polyFitTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)      695 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/pythonConversionTest.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     1292 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/testAutodiffHelper.cpp
--rwxrwxrwx   0 user      (1001) user      (1001)     5702 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/testFEElement.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:20:05.214963 pyikarus-0.3.0.dev202310000056/tests/src/testFiles/
--rwxrwxrwx   0 user      (1001) user      (1001)     9028 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000056/tests/src/testFiles/unstructuredQuadscoarse.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      395 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000056/tests/src/testFiles/unstructuredTest.geo
--rwxrwxrwx   0 user      (1001) user      (1001)      497 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000056/tests/src/testFiles/unstructuredTest.msh
--rwxrwxrwx   0 user      (1001) user      (1001)      546 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000056/tests/src/testFiles/unstructuredTest2.geo
--rwxrwxrwx   0 user      (1001) user      (1001)    11431 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000056/tests/src/testFiles/unstructuredTrianglesfine.msh
--rwxrwxrwx   0 user      (1001) user      (1001)     1114 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000056/tests/src/testHelpers.hh
--rwxrwxrwx   0 user      (1001) user      (1001)    17595 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000056/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:58.524821 pyikarus-0.3.0.dev202310000057/
+-rwxrwxrwx   0 user      (1001) user      (1001)      312 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.bettercodehub.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1300 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.clang-format
+-rwxrwxrwx   0 user      (1001) user      (1001)     1017 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.cmake-format
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.098308 pyikarus-0.3.0.dev202310000057/.github/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.586663 pyikarus-0.3.0.dev202310000057/.github/ISSUE_TEMPLATE/
+-rwxrwxrwx   0 user      (1001) user      (1001)      460 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/ISSUE_TEMPLATE/bug_report.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      615 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.749716 pyikarus-0.3.0.dev202310000057/.github/workflows/
+-rwxrwxrwx   0 user      (1001) user      (1001)      476 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/codespell.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1034 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/createDockerContainer.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     4900 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/createRelease.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1635 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/debian-coverage.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2108 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/debian.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/ghpages.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/reuseLint.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     2854 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/runExamples.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     1212 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.github/workflows/style.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      455 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/.gitignore
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.764062 pyikarus-0.3.0.dev202310000057/.reuse/
+-rwxrwxrwx   0 user      (1001) user      (1001)      661 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/.reuse/dep5
+-rwxrwxrwx   0 user      (1001) user      (1001)     3063 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/CHANGELOG.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1319 2023-05-10 12:56:29.000000 pyikarus-0.3.0.dev202310000057/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5335 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/CODE_OF_CONDUCT.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/LICENSE.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.819335 pyikarus-0.3.0.dev202310000057/LICENSES/
+-rwxrwxrwx   0 user      (1001) user      (1001)    18375 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/LICENSES/CC-BY-SA-4.0.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     7048 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/LICENSES/CC0-1.0.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    42098 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/LICENSES/LGPL-3.0-or-later.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    16727 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 13:28:58.522564 pyikarus-0.3.0.dev202310000057/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/README.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.843707 pyikarus-0.3.0.dev202310000057/cmake/
+-rwxrwxrwx   0 user      (1001) user      (1001)      973 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/CPM.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.859458 pyikarus-0.3.0.dev202310000057/cmake/FormatTarget/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1270 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.969444 pyikarus-0.3.0.dev202310000057/cmake/modules/
+-rwxrwxrwx   0 user      (1001) user      (1001)      715 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/modules/AddAutoDiffFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      683 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/modules/AddEigenFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      740 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/modules/AddMatplotppFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      691 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/modules/AddSpdlogFlags.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      226 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/modules/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      446 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/modules/IkarusMacros.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)     2040 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/cmake/tools.cmake
+-rwxrwxrwx   0 user      (1001) user      (1001)      148 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/codecov.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)      121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/codespellignore
+-rwxrwxrwx   0 user      (1001) user      (1001)     1588 2023-05-10 12:14:52.000000 pyikarus-0.3.0.dev202310000057/config.h.cmake
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.060113 pyikarus-0.3.0.dev202310000057/docs/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.078734 pyikarus-0.3.0.dev202310000057/docs/BuildLocally/
+-rwxrwxrwx   0 user      (1001) user      (1001)      439 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/BuildLocally/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      333 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.118614 pyikarus-0.3.0.dev202310000057/docs/__pycache__/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1136 2023-04-21 10:05:27.000000 pyikarus-0.3.0.dev202310000057/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     6961 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/literature.bib
+-rwxrwxrwx   0 user      (1001) user      (1001)      117 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/literature.bib.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     1245 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/mkdocs-macros.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      394 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/mkdocs.insiders.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)     5042 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/mkdocs.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:52.132694 pyikarus-0.3.0.dev202310000057/docs/overrides/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.140258 pyikarus-0.3.0.dev202310000057/docs/overrides/partials/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1732 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/overrides/partials/comments.html
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.216323 pyikarus-0.3.0.dev202310000057/docs/website/
+-rwxrwxrwx   0 user      (1001) user      (1001)       24 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/.meta.yml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.512160 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/
+-rwxrwxrwx   0 user      (1001) user      (1001)     4710 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/assembler.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     6387 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/controlRoutines.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2024 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/dirichletBCs.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3237 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/feRequirements.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     8527 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/finiteElements.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2745 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/grids.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4121 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/index.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4932 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/localBasis.md
+-rwxrwxrwx   0 user      (1001) user      (1001)    44233 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/localFunctions.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3978 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/manifolds.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2590 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/nonlinearOperator.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     3086 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/observer.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5211 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.730689 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/
+-rwxrwxrwx   0 user      (1001) user      (1001)     6675 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/cantileverBeam.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7271 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/computePi.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5477 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/cooksMembrane.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7051 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/incompressibleRubberBlock.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2164 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/index.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     7719 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/kirchhoffPlate.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     5134 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/newtonRaphsonMethod.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     6149 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/nonLinearElasticity.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     4090 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.830930 pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2439 2023-05-10 12:50:55.000000 pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/buildDocumentationLocally.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1002 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/codeStyle.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     2415 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/howToEdit.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1762 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.882418 pyikarus-0.3.0.dev202310000057/docs/website/04_blog/
+-rwxrwxrwx   0 user      (1001) user      (1001)      274 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/04_blog/.authors.yml
+-rwxrwxrwx   0 user      (1001) user      (1001)        7 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/04_blog/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.912689 pyikarus-0.3.0.dev202310000057/docs/website/04_blog/posts/
+-rwxrwxrwx   0 user      (1001) user      (1001)     7731 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.939538 pyikarus-0.3.0.dev202310000057/docs/website/05_cppReferences/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2324 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:53.961153 pyikarus-0.3.0.dev202310000057/docs/website/99_Literature/
+-rwxrwxrwx   0 user      (1001) user      (1001)      169 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:54.075642 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:54.495562 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/
+-rwxrwxrwx   0 user      (1001) user      (1001)    52795 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    46250 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     2852 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    17924 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     9455 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:54.996495 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/
+-rwxrwxrwx   0 user      (1001) user      (1001)    35234 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    62184 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     2281 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    40033 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)    25505 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     8101 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/logo_blue.svg
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/logo_blue.svg.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     8255 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/logo_white.svg
+-rwxrwxrwx   0 user      (1001) user      (1001)      119 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/logo_white.svg.license
+-rwxrwxrwx   0 user      (1001) user      (1001)     4364 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/download.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/gallery.md
+-rwxrwxrwx   0 user      (1001) user      (1001)     1358 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/index.md
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:55.022129 pyikarus-0.3.0.dev202310000057/docs/website/javascripts/
+-rwxrwxrwx   0 user      (1001) user      (1001)      486 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:55.044143 pyikarus-0.3.0.dev202310000057/docs/website/stylesheets/
+-rwxrwxrwx   0 user      (1001) user      (1001)      302 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/docs/website/stylesheets/extra.css
+-rwxrwxrwx   0 user      (1001) user      (1001)      502 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/dune.module
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:55.059151 pyikarus-0.3.0.dev202310000057/ikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      748 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:55.303405 pyikarus-0.3.0.dev202310000057/ikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      268 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    11012 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/assembler/simpleAssemblers.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    10681 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:55.535370 pyikarus-0.3.0.dev202310000057/ikarus/controlRoutines/
+-rwxrwxrwx   0 user      (1001) user      (1001)      239 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/controlRoutines/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2575 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/controlRoutines/loadControl.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2970 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:55.712675 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      349 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      185 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:55.830099 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feBases/
+-rwxrwxrwx   0 user      (1001) user      (1001)      282 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feBases/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2649 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feBases/autodiffFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2151 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1701 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feBases/scalarFE.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1041 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feRequirements.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     8419 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feRequirements.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1338 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:55.971646 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/
+-rwxrwxrwx   0 user      (1001) user      (1001)      345 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)    20311 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12753 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.235727 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/
+-rwxrwxrwx   0 user      (1001) user      (1001)      397 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5699 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/interface.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2718 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     4635 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3809 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5734 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/svk.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      473 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/tags.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     8010 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1196 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     7966 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12655 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.326371 pyikarus-0.3.0.dev202310000057/ikarus/linearAlgebra/
+-rwxrwxrwx   0 user      (1001) user      (1001)      301 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/linearAlgebra/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     6448 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/linearAlgebra/dirichletValues.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     7791 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/linearAlgebra/nonLinearOperator.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    12303 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.346178 pyikarus-0.3.0.dev202310000057/ikarus/python/
+-rwxrwxrwx   0 user      (1001) user      (1001)      270 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.393834 pyikarus-0.3.0.dev202310000057/ikarus/python/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      249 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3115 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.442771 pyikarus-0.3.0.dev202310000057/ikarus/python/dirichletValues/
+-rwxrwxrwx   0 user      (1001) user      (1001)      257 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/dirichletValues/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     4116 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.515737 pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      303 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5526 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.578688 pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/materials/
+-rwxrwxrwx   0 user      (1001) user      (1001)      259 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5107 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/materials/material.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5419 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.748958 pyikarus-0.3.0.dev202310000057/ikarus/python/test/
+-rwxrwxrwx   0 user      (1001) user      (1001)      787 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/test/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3808 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/test/linearElasticTest.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1839 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/test/nameTest.vtu
+-rwxrwxrwx   0 user      (1001) user      (1001)     4444 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/test/nonLinearElasticTest.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      862 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/test/setpath.py.in
+-rwxrwxrwx   0 user      (1001) user      (1001)      321 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/test/test1.py
+-rwxrwxrwx   0 user      (1001) user      (1001)      582 2023-05-10 13:17:17.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/test/test2.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.825841 pyikarus-0.3.0.dev202310000057/ikarus/python/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      245 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1434 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.848089 pyikarus-0.3.0.dev202310000057/ikarus/solver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      211 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.896886 pyikarus-0.3.0.dev202310000057/ikarus/solver/linearSolver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      244 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/solver/linearSolver/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     8891 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:56.982602 pyikarus-0.3.0.dev202310000057/ikarus/solver/nonLinearSolver/
+-rwxrwxrwx   0 user      (1001) user      (1001)      272 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     5407 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     8297 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    18574 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.310745 pyikarus-0.3.0.dev202310000057/ikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      671 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1741 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/algorithms.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      878 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/autodiffHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     6930 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/concepts.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      503 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.399010 pyikarus-0.3.0.dev202310000057/ikarus/utils/drawing/
+-rwxrwxrwx   0 user      (1001) user      (1001)      262 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/drawing/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1654 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/drawing/griddrawer.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      544 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/drawing/matplotHelper.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      703 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/drawing/matplotHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2484 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/duneUtilities.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2347 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/eigenDuneTransformations.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      682 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/eigenSparseAddon.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1367 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/findLineSegment.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/findLineSegment.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2171 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/functionSanityChecks.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6359 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/functionSanityChecks.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     3152 2023-05-10 12:14:52.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/init.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    15244 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/linearAlgebraHelper.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1711 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.621291 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/
+-rwxrwxrwx   0 user      (1001) user      (1001)      450 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1554 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/controlLogger.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2307 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/controlVTKWriter.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      905 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/genericControlObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1053 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/gridDrawerObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1132 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/loadControlObserver.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1985 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     5497 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/observer.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      489 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/observerMessages.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     4159 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/pathFollowingFunctions.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1131 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/polyfit.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      570 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/polyfit.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    10054 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/tensorUtils.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    15044 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus/utils/traits.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      432 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/ikarus.pc.in
+-rwxrwxrwx   0 user      (1001) user      (1001)      196 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/iwyu.imp
+-rwxrwxrwx   0 user      (1001) user      (1001)      305 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/pyproject.toml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.652508 pyikarus-0.3.0.dev202310000057/python/
+-rwxrwxrwx   0 user      (1001) user      (1001)      403 2023-05-10 12:21:57.000000 pyikarus-0.3.0.dev202310000057/python/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.746125 pyikarus-0.3.0.dev202310000057/python/ikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      654 2023-05-10 13:25:20.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      578 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     5636 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.788512 pyikarus-0.3.0.dev202310000057/python/ikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)      167 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/assembler/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     2300 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/assembler/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1408 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.831123 pyikarus-0.3.0.dev202310000057/python/ikarus/finite_elements/
+-rwxrwxrwx   0 user      (1001) user      (1001)      173 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/finite_elements/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3465 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/finite_elements/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1792 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/materials.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.874572 pyikarus-0.3.0.dev202310000057/python/ikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)      163 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/utils/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     1461 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.964672 pyikarus-0.3.0.dev202310000057/python/pyikarus.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 13:28:50.000000 pyikarus-0.3.0.dev202310000057/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)     9785 2023-05-10 13:28:52.000000 pyikarus-0.3.0.dev202310000057/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-10 13:28:50.000000 pyikarus-0.3.0.dev202310000057/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-10 13:28:50.000000 pyikarus-0.3.0.dev202310000057/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) user      (1001)        7 2023-05-10 13:28:50.000000 pyikarus-0.3.0.dev202310000057/python/pyikarus.egg-info/top_level.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)      636 2023-05-10 12:27:37.000000 pyikarus-0.3.0.dev202310000057/python/setup.py.in
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:57.976529 pyikarus-0.3.0.dev202310000057/sandbox/
+-rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/sandbox/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:58.002333 pyikarus-0.3.0.dev202310000057/sandbox/src/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1220 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:58.018607 pyikarus-0.3.0.dev202310000057/sandbox/src/auxiliaryFiles/
+-rwxrwxrwx   0 user      (1001) user      (1001)   674469 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/sandbox/src/auxiliaryFiles/circle.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      320 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/sandbox/src/sandbox.cpp
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-10 13:28:58.525861 pyikarus-0.3.0.dev202310000057/setup.cfg
+-rwxrwxrwx   0 user      (1001) user      (1001)     1683 2023-05-10 13:25:27.000000 pyikarus-0.3.0.dev202310000057/setup.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:58.038274 pyikarus-0.3.0.dev202310000057/tests/
+-rwxrwxrwx   0 user      (1001) user      (1001)      150 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/tests/CMakeLists.txt
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:58.397042 pyikarus-0.3.0.dev202310000057/tests/src/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1397 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/tests/src/CMakeLists.txt
+-rwxrwxrwx   0 user      (1001) user      (1001)     3888 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/assemblerTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     9913 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/common.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     2639 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/dependenciesTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6409 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/dirichletValueTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     3820 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/easTest.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1473 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/enhancedAssumedStrainsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      608 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/tests/src/factories.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1870 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/functionTraitsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     2221 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/linearElasticityTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     2378 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/manifoldsTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     7961 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/materialTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6561 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/nonLinearElasticityTest.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)      724 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/tests/src/nonLinearElasticityTestNeoHooke.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      729 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/tests/src/nonLinearElasticityTestSVK.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     9936 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/nonLinearOperatorTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     6327 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/pathFollowingTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     1651 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/polyFitTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)      695 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/pythonConversionTest.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     1292 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/testAutodiffHelper.cpp
+-rwxrwxrwx   0 user      (1001) user      (1001)     5702 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/testFEElement.hh
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 13:28:58.503172 pyikarus-0.3.0.dev202310000057/tests/src/testFiles/
+-rwxrwxrwx   0 user      (1001) user      (1001)     9028 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000057/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      395 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000057/tests/src/testFiles/unstructuredTest.geo
+-rwxrwxrwx   0 user      (1001) user      (1001)      497 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000057/tests/src/testFiles/unstructuredTest.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)      546 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000057/tests/src/testFiles/unstructuredTest2.geo
+-rwxrwxrwx   0 user      (1001) user      (1001)    11431 2023-02-17 11:23:00.000000 pyikarus-0.3.0.dev202310000057/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rwxrwxrwx   0 user      (1001) user      (1001)     1114 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000057/tests/src/testHelpers.hh
+-rwxrwxrwx   0 user      (1001) user      (1001)    17595 2023-05-10 12:11:48.000000 pyikarus-0.3.0.dev202310000057/tests/src/trustRegionTest.cpp
```

### Comparing `pyikarus-0.3.0.dev202310000056/.clang-format` & `pyikarus-0.3.0.dev202310000057/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.cmake-format` & `pyikarus-0.3.0.dev202310000057/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.0.dev202310000057/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.0.dev202310000057/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.github/workflows/createRelease.yml` & `pyikarus-0.3.0.dev202310000057/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.0.dev202310000057/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.github/workflows/debian.yml` & `pyikarus-0.3.0.dev202310000057/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.github/workflows/ghpages.yml` & `pyikarus-0.3.0.dev202310000057/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.github/workflows/runExamples.yml` & `pyikarus-0.3.0.dev202310000057/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.github/workflows/style.yml` & `pyikarus-0.3.0.dev202310000057/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/.reuse/dep5` & `pyikarus-0.3.0.dev202310000057/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/CHANGELOG.md` & `pyikarus-0.3.0.dev202310000057/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000057/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/CODE_OF_CONDUCT.md` & `pyikarus-0.3.0.dev202310000057/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/LICENSE.md` & `pyikarus-0.3.0.dev202310000057/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.0.dev202310000057/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.0.dev202310000057/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.0.dev202310000057/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.0.dev202310000057/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/PKG-INFO` & `pyikarus-0.3.0.dev202310000057/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000056
+Version: 0.3.0.dev202310000057
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
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000056 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000057 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000056/README.md` & `pyikarus-0.3.0.dev202310000057/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/cmake/CPM.cmake` & `pyikarus-0.3.0.dev202310000057/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000057/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.0.dev202310000057/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.0.dev202310000057/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.0.dev202310000057/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.0.dev202310000057/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/cmake/tools.cmake` & `pyikarus-0.3.0.dev202310000057/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/config.h.cmake` & `pyikarus-0.3.0.dev202310000057/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.0.dev202310000057/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/literature.bib` & `pyikarus-0.3.0.dev202310000057/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/mkdocs-macros.py` & `pyikarus-0.3.0.dev202310000057/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/mkdocs.yml` & `pyikarus-0.3.0.dev202310000057/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/overrides/partials/comments.html` & `pyikarus-0.3.0.dev202310000057/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/assembler.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/grids.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/index.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/observer.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/01_framework/solvers.md` & `pyikarus-0.3.0.dev202310000057/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/computePi.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/index.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/nonLinearElasticity.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.0.dev202310000057/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.0.dev202310000057/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.0.dev202310000057/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.0.dev202310000057/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.0.dev202310000057/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/download.md` & `pyikarus-0.3.0.dev202310000057/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/docs/website/index.md` & `pyikarus-0.3.0.dev202310000057/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000057/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.0.dev202310000057/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feRequirements.cpp` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feRequirements.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/test/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000057/ikarus/python/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.0.dev202310000057/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/test/nameTest.vtu` & `pyikarus-0.3.0.dev202310000057/ikarus/python/test/nameTest.vtu`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.0.dev202310000057/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.0.dev202310000057/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/test/test2.py` & `pyikarus-0.3.0.dev202310000057/ikarus/python/test/test2.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/algorithms.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/concepts.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/init.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/polyfit.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/ikarus/utils/traits.hh` & `pyikarus-0.3.0.dev202310000057/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/ikarus/__init__.py` & `pyikarus-0.3.0.dev202310000057/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/ikarus/_ikarus.cc` & `pyikarus-0.3.0.dev202310000057/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.0.dev202310000057/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/ikarus/dirichletValues.py` & `pyikarus-0.3.0.dev202310000057/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.0.dev202310000057/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/ikarus/materials.py` & `pyikarus-0.3.0.dev202310000057/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/ikarus/utils/__init__.py` & `pyikarus-0.3.0.dev202310000057/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.0.dev202310000057/python/pyikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000056
+Version: 0.3.0.dev202310000057
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
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000056 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000057 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000056/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.0.dev202310000057/python/pyikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/python/setup.py.in` & `pyikarus-0.3.0.dev202310000057/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000057/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.0.dev202310000057/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/setup.py` & `pyikarus-0.3.0.dev202310000057/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # You are logged in as $(whoami)
 # EOF
 # nano ~/.pypirc
 # python -m venv /dune/dune-common/build-cmake/dune-env/
 # source /dune/dune-common/build-cmake/dune-env/bin/activate
 # pip install ikarus  --no-build-isolation
 
-ikarusVersion = "0.3.0.dev202310000056" #+ datetime.today().time().strftime("%H%M%S")
+ikarusVersion = "0.3.0.dev202310000057" #+ datetime.today().time().strftime("%H%M%S")
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor sicne ikarus pypi package already exists
 metadata["name"] = "pyikarus"
```

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/CMakeLists.txt` & `pyikarus-0.3.0.dev202310000057/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/assemblerTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/assemblerTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/common.hh` & `pyikarus-0.3.0.dev202310000057/tests/src/common.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/dependenciesTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/dependenciesTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/dirichletValueTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/dirichletValueTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/easTest.hh` & `pyikarus-0.3.0.dev202310000057/tests/src/easTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/enhancedAssumedStrainsTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/enhancedAssumedStrainsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/factories.hh` & `pyikarus-0.3.0.dev202310000057/tests/src/factories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/functionTraitsTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/functionTraitsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/linearElasticityTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/linearElasticityTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/manifoldsTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/manifoldsTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/materialTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/materialTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/nonLinearElasticityTest.hh` & `pyikarus-0.3.0.dev202310000057/tests/src/nonLinearElasticityTest.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/nonLinearElasticityTestNeoHooke.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/nonLinearElasticityTestNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/nonLinearElasticityTestSVK.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/nonLinearElasticityTestSVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/nonLinearOperatorTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/nonLinearOperatorTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/pathFollowingTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/pathFollowingTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/polyFitTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/polyFitTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/pythonConversionTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/pythonConversionTest.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/testFEElement.hh` & `pyikarus-0.3.0.dev202310000057/tests/src/testFEElement.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.0.dev202310000057/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.0.dev202310000057/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.0.dev202310000057/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/testHelpers.hh` & `pyikarus-0.3.0.dev202310000057/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000056/tests/src/trustRegionTest.cpp` & `pyikarus-0.3.0.dev202310000057/tests/src/trustRegionTest.cpp`

 * *Files identical despite different names*

