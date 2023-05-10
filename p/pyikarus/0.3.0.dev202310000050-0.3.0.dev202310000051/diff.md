# Comparing `tmp/pyikarus-0.3.0.dev202310000050.tar.gz` & `tmp/pyikarus-0.3.0.dev202310000051.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.0.dev202310000050.tar", last modified: Wed Mar 15 14:12:09 2023, max compression
+gzip compressed data, was "pyikarus-0.3.0.dev202310000051.tar", last modified: Wed May 10 11:47:48 2023, max compression
```

## Comparing `pyikarus-0.3.0.dev202310000050.tar` & `pyikarus-0.3.0.dev202310000051.tar`

### file list

```diff
@@ -1,309 +1,25 @@
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.392975 pyikarus-0.3.0.dev202310000050/
--rw-r--r--   0 user      (1001) user      (1001)      312 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/.bettercodehub.yml
--rw-r--r--   0 user      (1001) user      (1001)     1300 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/.clang-format
--rw-r--r--   0 user      (1001) user      (1001)     1017 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/.cmake-format
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.204975 pyikarus-0.3.0.dev202310000050/.github/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.236975 pyikarus-0.3.0.dev202310000050/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 user      (1001) user      (1001)      460 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 user      (1001) user      (1001)      615 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.240975 pyikarus-0.3.0.dev202310000050/.github/workflows/
--rw-r--r--   0 user      (1001) user      (1001)      476 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/codespell.yml
--rw-r--r--   0 user      (1001) user      (1001)     1034 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 user      (1001) user      (1001)     4900 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/createRelease.yml
--rw-r--r--   0 user      (1001) user      (1001)     1635 2023-03-14 18:58:04.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/debian-coverage.yml
--rw-r--r--   0 user      (1001) user      (1001)     2108 2023-03-14 18:58:04.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/debian.yml
--rw-r--r--   0 user      (1001) user      (1001)     2042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/ghpages.yml
--rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/reuseLint.yml
--rw-r--r--   0 user      (1001) user      (1001)     2854 2023-03-14 18:58:11.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/runExamples.yml
--rw-r--r--   0 user      (1001) user      (1001)     1212 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/.github/workflows/style.yml
--rw-r--r--   0 user      (1001) user      (1001)      456 2023-03-14 18:58:14.000000 pyikarus-0.3.0.dev202310000050/.gitignore
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.240975 pyikarus-0.3.0.dev202310000050/.reuse/
--rw-r--r--   0 user      (1001) user      (1001)      661 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/.reuse/dep5
--rw-r--r--   0 user      (1001) user      (1001)     3063 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/CHANGELOG.md
--rw-r--r--   0 user      (1001) user      (1001)     1323 2023-03-14 18:57:18.000000 pyikarus-0.3.0.dev202310000050/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5335 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/CODE_OF_CONDUCT.md
--rw-r--r--   0 user      (1001) user      (1001)      759 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/LICENSE.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.244975 pyikarus-0.3.0.dev202310000050/LICENSES/
--rw-r--r--   0 user      (1001) user      (1001)    18375 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     7048 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/LICENSES/CC0-1.0.txt
--rw-r--r--   0 user      (1001) user      (1001)    42098 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 user      (1001) user      (1001)    16727 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/LICENSES/MPL-2.0.txt
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-03-15 14:12:09.392975 pyikarus-0.3.0.dev202310000050/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)     3229 2023-03-06 10:17:28.000000 pyikarus-0.3.0.dev202310000050/README.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.248975 pyikarus-0.3.0.dev202310000050/cmake/
--rw-r--r--   0 user      (1001) user      (1001)      973 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/cmake/CPM.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.248975 pyikarus-0.3.0.dev202310000050/cmake/FormatTarget/
--rw-r--r--   0 user      (1001) user      (1001)     1270 2023-03-10 08:15:25.000000 pyikarus-0.3.0.dev202310000050/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.252975 pyikarus-0.3.0.dev202310000050/cmake/modules/
--rw-r--r--   0 user      (1001) user      (1001)      715 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      683 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      740 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      691 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 user      (1001) user      (1001)      226 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/cmake/modules/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      446 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 user      (1001) user      (1001)     2040 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/cmake/tools.cmake
--rw-r--r--   0 user      (1001) user      (1001)      148 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/codecov.yml
--rw-r--r--   0 user      (1001) user      (1001)      121 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/codespellignore
--rw-r--r--   0 user      (1001) user      (1001)     1618 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/config.h.cmake
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.256975 pyikarus-0.3.0.dev202310000050/docs/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.256975 pyikarus-0.3.0.dev202310000050/docs/BuildLocally/
--rw-r--r--   0 user      (1001) user      (1001)      439 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      333 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.256975 pyikarus-0.3.0.dev202310000050/docs/__pycache__/
--rw-r--r--   0 user      (1001) user      (1001)     1136 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 user      (1001) user      (1001)     6961 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/literature.bib
--rw-r--r--   0 user      (1001) user      (1001)      117 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/literature.bib.license
--rw-r--r--   0 user      (1001) user      (1001)     1245 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/mkdocs-macros.py
--rw-r--r--   0 user      (1001) user      (1001)      394 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/mkdocs.insiders.yml
--rw-r--r--   0 user      (1001) user      (1001)     5042 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/mkdocs.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.208975 pyikarus-0.3.0.dev202310000050/docs/overrides/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.256975 pyikarus-0.3.0.dev202310000050/docs/overrides/partials/
--rw-r--r--   0 user      (1001) user      (1001)     1732 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/overrides/partials/comments.html
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.260975 pyikarus-0.3.0.dev202310000050/docs/website/
--rw-r--r--   0 user      (1001) user      (1001)       24 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/.meta.yml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.268975 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/
--rw-r--r--   0 user      (1001) user      (1001)     4710 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/assembler.md
--rw-r--r--   0 user      (1001) user      (1001)     6387 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 user      (1001) user      (1001)     2024 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 user      (1001) user      (1001)     3237 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 user      (1001) user      (1001)     8527 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 user      (1001) user      (1001)     2745 2023-03-14 18:55:34.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/grids.md
--rw-r--r--   0 user      (1001) user      (1001)     4121 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/index.md
--rw-r--r--   0 user      (1001) user      (1001)     4932 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/localBasis.md
--rw-r--r--   0 user      (1001) user      (1001)    44233 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 user      (1001) user      (1001)     3978 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/manifolds.md
--rw-r--r--   0 user      (1001) user      (1001)     2590 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 user      (1001) user      (1001)     3086 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/observer.md
--rw-r--r--   0 user      (1001) user      (1001)     5211 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.272975 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/
--rw-r--r--   0 user      (1001) user      (1001)     6675 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 user      (1001) user      (1001)     7271 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/computePi.md
--rw-r--r--   0 user      (1001) user      (1001)     5477 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 user      (1001) user      (1001)     7051 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 user      (1001) user      (1001)     2164 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/index.md
--rw-r--r--   0 user      (1001) user      (1001)     7719 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 user      (1001) user      (1001)     5134 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 user      (1001) user      (1001)     6149 2023-03-14 19:23:17.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 user      (1001) user      (1001)     4090 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.276975 pyikarus-0.3.0.dev202310000050/docs/website/03_contribution/
--rw-r--r--   0 user      (1001) user      (1001)     2469 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 user      (1001) user      (1001)     1002 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 user      (1001) user      (1001)     2415 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 user      (1001) user      (1001)     1762 2023-03-14 19:23:17.000000 pyikarus-0.3.0.dev202310000050/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.276975 pyikarus-0.3.0.dev202310000050/docs/website/04_blog/
--rw-r--r--   0 user      (1001) user      (1001)      274 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/04_blog/.authors.yml
--rw-r--r--   0 user      (1001) user      (1001)        7 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/04_blog/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.276975 pyikarus-0.3.0.dev202310000050/docs/website/04_blog/posts/
--rw-r--r--   0 user      (1001) user      (1001)     7731 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.280975 pyikarus-0.3.0.dev202310000050/docs/website/05_cppReferences/
--rw-r--r--   0 user      (1001) user      (1001)     2324 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.280975 pyikarus-0.3.0.dev202310000050/docs/website/99_Literature/
--rw-r--r--   0 user      (1001) user      (1001)      169 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.280975 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.292975 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 user      (1001) user      (1001)    52795 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 user      (1001) user      (1001)    46250 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 user      (1001) user      (1001)     2852 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 user      (1001) user      (1001)    17924 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 user      (1001) user      (1001)     9455 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
--rw-r--r--   0 user      (1001) user      (1001)     8101 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/logo_blue.svg
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/logo_blue.svg.license
--rw-r--r--   0 user      (1001) user      (1001)     8255 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/logo_white.svg
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/auxiliaryImages/logo_white.svg.license
--rw-r--r--   0 user      (1001) user      (1001)     4364 2023-02-20 07:47:52.000000 pyikarus-0.3.0.dev202310000050/docs/website/download.md
--rw-r--r--   0 user      (1001) user      (1001)      244 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/gallery.md
--rw-r--r--   0 user      (1001) user      (1001)     1358 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/index.md
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.292975 pyikarus-0.3.0.dev202310000050/docs/website/javascripts/
--rw-r--r--   0 user      (1001) user      (1001)      486 2023-03-14 16:50:02.000000 pyikarus-0.3.0.dev202310000050/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.292975 pyikarus-0.3.0.dev202310000050/docs/website/stylesheets/
--rw-r--r--   0 user      (1001) user      (1001)      302 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/docs/website/stylesheets/extra.css
--rw-r--r--   0 user      (1001) user      (1001)      504 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/dune.module
--rw-r--r--   0 user      (1001) user      (1001)      196 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/iwyu.imp
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.292975 pyikarus-0.3.0.dev202310000050/pyikarus/
--rw-r--r--   0 user      (1001) user      (1001)      748 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.296975 pyikarus-0.3.0.dev202310000050/pyikarus/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      270 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)    11016 2023-03-15 11:45:03.000000 pyikarus-0.3.0.dev202310000050/pyikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 user      (1001) user      (1001)    10681 2023-03-15 11:35:34.000000 pyikarus-0.3.0.dev202310000050/pyikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.296975 pyikarus-0.3.0.dev202310000050/pyikarus/controlRoutines/
--rw-r--r--   0 user      (1001) user      (1001)      241 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2583 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 user      (1001) user      (1001)     2980 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.300975 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/
--rw-r--r--   0 user      (1001) user      (1001)      351 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      185 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.304975 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/feBases/
--rw-r--r--   0 user      (1001) user      (1001)      284 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2653 2023-03-15 12:43:47.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     2153 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     1703 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 user      (1001) user      (1001)     1041 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/feRequirements.cpp
--rw-r--r--   0 user      (1001) user      (1001)     8419 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 user      (1001) user      (1001)     1340 2023-03-14 18:57:22.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.304975 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/
--rw-r--r--   0 user      (1001) user      (1001)      347 2023-03-14 19:23:17.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)    20315 2023-03-14 19:01:04.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 user      (1001) user      (1001)    12771 2023-03-15 08:36:26.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.312975 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 user      (1001) user      (1001)      399 2023-03-15 14:11:56.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5709 2023-03-14 19:00:59.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 user      (1001) user      (1001)     2720 2023-03-14 19:01:00.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 user      (1001) user      (1001)     4637 2023-03-14 19:01:01.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 user      (1001) user      (1001)     3811 2023-03-14 19:01:02.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 user      (1001) user      (1001)     5736 2023-03-14 19:01:02.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 user      (1001) user      (1001)      475 2023-03-14 19:01:03.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 user      (1001) user      (1001)     8014 2023-03-15 09:46:02.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 user      (1001) user      (1001)     1208 2023-03-15 13:55:55.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 user      (1001) user      (1001)     8187 2023-03-15 12:29:30.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 user      (1001) user      (1001)    12655 2023-03-14 18:57:22.000000 pyikarus-0.3.0.dev202310000050/pyikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.316975 pyikarus-0.3.0.dev202310000050/pyikarus/linearAlgebra/
--rw-r--r--   0 user      (1001) user      (1001)      303 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     6452 2023-03-14 18:57:22.000000 pyikarus-0.3.0.dev202310000050/pyikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 user      (1001) user      (1001)     7793 2023-03-14 19:39:52.000000 pyikarus-0.3.0.dev202310000050/pyikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 user      (1001) user      (1001)    12303 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.316975 pyikarus-0.3.0.dev202310000050/pyikarus/python/
--rw-r--r--   0 user      (1001) user      (1001)      270 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.316975 pyikarus-0.3.0.dev202310000050/pyikarus/python/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      251 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3117 2023-03-15 12:59:54.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.316975 pyikarus-0.3.0.dev202310000050/pyikarus/python/dirichletValues/
--rw-r--r--   0 user      (1001) user      (1001)      259 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     4118 2023-03-14 18:58:14.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.320975 pyikarus-0.3.0.dev202310000050/pyikarus/python/finiteElements/
--rw-r--r--   0 user      (1001) user      (1001)      305 2023-03-15 11:27:53.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5528 2023-03-14 19:11:55.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.320975 pyikarus-0.3.0.dev202310000050/pyikarus/python/finiteElements/materials/
--rw-r--r--   0 user      (1001) user      (1001)      261 2023-03-15 11:28:22.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5113 2023-03-15 11:15:22.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 user      (1001) user      (1001)     5421 2023-03-14 21:00:01.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.328975 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/
--rw-r--r--   0 user      (1001) user      (1001)      787 2023-03-15 11:25:59.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3820 2023-03-15 11:24:29.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/linearElasticTest.py
--rw-r--r--   0 user      (1001) user      (1001)     1839 2023-03-15 12:03:48.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/nameTest.vtu
--rw-r--r--   0 user      (1001) user      (1001)     4462 2023-03-15 13:37:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 user      (1001) user      (1001)      866 2023-03-14 18:58:32.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/setpath.py
--rw-r--r--   0 user      (1001) user      (1001)      862 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/setpath.py.in
--rw-r--r--   0 user      (1001) user      (1001)      327 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/test1.py
--rw-r--r--   0 user      (1001) user      (1001)      586 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/test/test2.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.328975 pyikarus-0.3.0.dev202310000050/pyikarus/python/utils/
--rw-r--r--   0 user      (1001) user      (1001)      247 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1436 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.332975 pyikarus-0.3.0.dev202310000050/pyikarus/solver/
--rw-r--r--   0 user      (1001) user      (1001)      211 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.332975 pyikarus-0.3.0.dev202310000050/pyikarus/solver/linearSolver/
--rw-r--r--   0 user      (1001) user      (1001)      246 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     8891 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.336975 pyikarus-0.3.0.dev202310000050/pyikarus/solver/nonLinearSolver/
--rw-r--r--   0 user      (1001) user      (1001)      274 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     5419 2023-03-14 19:43:25.000000 pyikarus-0.3.0.dev202310000050/pyikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 user      (1001) user      (1001)     8309 2023-03-14 19:01:23.000000 pyikarus-0.3.0.dev202310000050/pyikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 user      (1001) user      (1001)    18586 2023-03-14 19:01:27.000000 pyikarus-0.3.0.dev202310000050/pyikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.348975 pyikarus-0.3.0.dev202310000050/pyikarus/utils/
--rw-r--r--   0 user      (1001) user      (1001)      673 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1741 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/algorithms.hh
--rw-r--r--   0 user      (1001) user      (1001)      878 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/autodiffHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     6930 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/concepts.hh
--rw-r--r--   0 user      (1001) user      (1001)      503 2023-03-15 08:36:26.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.352975 pyikarus-0.3.0.dev202310000050/pyikarus/utils/drawing/
--rw-r--r--   0 user      (1001) user      (1001)      264 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1654 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 user      (1001) user      (1001)      544 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 user      (1001) user      (1001)      703 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     2484 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/duneUtilities.hh
--rw-r--r--   0 user      (1001) user      (1001)     2347 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 user      (1001) user      (1001)      682 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 user      (1001) user      (1001)     1367 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/findLineSegment.cpp
--rw-r--r--   0 user      (1001) user      (1001)      724 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/findLineSegment.hh
--rw-r--r--   0 user      (1001) user      (1001)     2171 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6359 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 user      (1001) user      (1001)     3154 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/init.hh
--rw-r--r--   0 user      (1001) user      (1001)    15244 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 user      (1001) user      (1001)     1711 2023-03-14 19:23:32.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/makeEnum.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.360975 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/
--rw-r--r--   0 user      (1001) user      (1001)      452 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1558 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 user      (1001) user      (1001)     2307 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 user      (1001) user      (1001)      909 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1059 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1136 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 user      (1001) user      (1001)     1985 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 user      (1001) user      (1001)     5499 2023-03-14 19:01:30.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/observer.hh
--rw-r--r--   0 user      (1001) user      (1001)      489 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 user      (1001) user      (1001)     4161 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 user      (1001) user      (1001)     1131 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/polyfit.cpp
--rw-r--r--   0 user      (1001) user      (1001)      570 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/polyfit.hh
--rw-r--r--   0 user      (1001) user      (1001)    10056 2023-03-14 19:24:12.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/tensorUtils.hh
--rw-r--r--   0 user      (1001) user      (1001)    15044 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus/utils/traits.hh
--rw-r--r--   0 user      (1001) user      (1001)      432 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/pyikarus.pc.in
--rw-r--r--   0 user      (1001) user      (1001)      305 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/pyproject.toml
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.364975 pyikarus-0.3.0.dev202310000050/python/
--rw-r--r--   0 user      (1001) user      (1001)      407 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/python/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.368975 pyikarus-0.3.0.dev202310000050/python/pyikarus/
--rw-r--r--   0 user      (1001) user      (1001)      523 2023-03-14 19:52:32.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)      584 2023-03-14 19:52:02.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     5644 2023-03-15 08:23:38.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/_pyikarus.cc
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.368975 pyikarus-0.3.0.dev202310000050/python/pyikarus/assembler/
--rw-r--r--   0 user      (1001) user      (1001)      167 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/assembler/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     2310 2023-03-15 14:00:57.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/assembler/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     1412 2023-03-14 19:48:37.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/dirichletValues.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.372975 pyikarus-0.3.0.dev202310000050/python/pyikarus/finite_elements/
--rw-r--r--   0 user      (1001) user      (1001)      173 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/finite_elements/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3473 2023-03-15 09:49:53.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/finite_elements/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)     1796 2023-03-15 08:57:06.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/materials.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.372975 pyikarus-0.3.0.dev202310000050/python/pyikarus/utils/
--rw-r--r--   0 user      (1001) user      (1001)      163 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/utils/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     1463 2023-03-14 18:58:14.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus/utils/__init__.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.368975 pyikarus-0.3.0.dev202310000050/python/pyikarus.egg-info/
--rw-r--r--   0 user      (1001) user      (1001)     3638 2023-03-15 14:12:09.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)     9269 2023-03-15 14:12:09.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1001) user      (1001)        1 2023-03-15 14:12:09.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1001) user      (1001)      119 2023-03-15 14:12:09.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 user      (1001) user      (1001)        9 2023-03-15 14:12:09.000000 pyikarus-0.3.0.dev202310000050/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 user      (1001) user      (1001)      638 2023-03-14 18:57:07.000000 pyikarus-0.3.0.dev202310000050/python/setup.py.in
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.372975 pyikarus-0.3.0.dev202310000050/sandbox/
--rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/sandbox/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.372975 pyikarus-0.3.0.dev202310000050/sandbox/src/
--rw-r--r--   0 user      (1001) user      (1001)     1222 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.372975 pyikarus-0.3.0.dev202310000050/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 user      (1001) user      (1001)   674469 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 user      (1001) user      (1001)      322 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/sandbox/src/sandbox.cpp
--rw-r--r--   0 user      (1001) user      (1001)       38 2023-03-15 14:12:09.392975 pyikarus-0.3.0.dev202310000050/setup.cfg
--rw-r--r--   0 user      (1001) user      (1001)     1381 2023-03-15 14:11:56.000000 pyikarus-0.3.0.dev202310000050/setup.py
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.376975 pyikarus-0.3.0.dev202310000050/tests/
--rw-r--r--   0 user      (1001) user      (1001)      150 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/tests/CMakeLists.txt
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.388975 pyikarus-0.3.0.dev202310000050/tests/src/
--rw-r--r--   0 user      (1001) user      (1001)     1397 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/CMakeLists.txt
--rw-r--r--   0 user      (1001) user      (1001)     3896 2023-03-14 19:23:17.000000 pyikarus-0.3.0.dev202310000050/tests/src/assemblerTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     9923 2023-03-14 18:57:22.000000 pyikarus-0.3.0.dev202310000050/tests/src/common.hh
--rw-r--r--   0 user      (1001) user      (1001)     2641 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/dependenciesTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6417 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/dirichletValueTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     3822 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/easTest.hh
--rw-r--r--   0 user      (1001) user      (1001)     1479 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/enhancedAssumedStrainsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)      608 2023-03-14 16:50:02.000000 pyikarus-0.3.0.dev202310000050/tests/src/factories.hh
--rw-r--r--   0 user      (1001) user      (1001)     1872 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/functionTraitsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     2225 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/linearElasticityTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     2382 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/manifoldsTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     7971 2023-03-14 19:01:34.000000 pyikarus-0.3.0.dev202310000050/tests/src/materialTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6583 2023-03-14 19:23:17.000000 pyikarus-0.3.0.dev202310000050/tests/src/nonLinearElasticityTest.hh
--rw-r--r--   0 user      (1001) user      (1001)      724 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rw-r--r--   0 user      (1001) user      (1001)      729 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/nonLinearElasticityTestSVK.cpp
--rw-r--r--   0 user      (1001) user      (1001)     9946 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/nonLinearOperatorTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     6341 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/pathFollowingTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     1655 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/polyFitTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)      699 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/pythonConversionTest.cpp
--rw-r--r--   0 user      (1001) user      (1001)     1296 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 user      (1001) user      (1001)     5710 2023-03-14 18:57:22.000000 pyikarus-0.3.0.dev202310000050/tests/src/testFEElement.hh
-drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-03-15 14:12:09.392975 pyikarus-0.3.0.dev202310000050/tests/src/testFiles/
--rw-r--r--   0 user      (1001) user      (1001)     9028 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 user      (1001) user      (1001)      395 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 user      (1001) user      (1001)      497 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 user      (1001) user      (1001)      546 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 user      (1001) user      (1001)    11431 2023-02-10 14:16:43.000000 pyikarus-0.3.0.dev202310000050/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 user      (1001) user      (1001)     1114 2023-03-14 16:50:02.000000 pyikarus-0.3.0.dev202310000050/tests/src/testHelpers.hh
--rw-r--r--   0 user      (1001) user      (1001)    17601 2023-03-14 18:55:35.000000 pyikarus-0.3.0.dev202310000050/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 11:47:48.035440 pyikarus-0.3.0.dev202310000051/
+-rwxrwxrwx   0 user      (1001) user      (1001)      759 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000051/LICENSE.md
+-rw-r--r--   0 user      (1001) user      (1001)        0 2023-05-10 11:40:26.000000 pyikarus-0.3.0.dev202310000051/MANIFEST.in
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 11:47:48.033435 pyikarus-0.3.0.dev202310000051/PKG-INFO
+-rwxrwxrwx   0 user      (1001) user      (1001)     3229 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000051/README.md
+-rwxrwxrwx   0 user      (1001) user      (1001)      305 2023-05-10 11:24:23.000000 pyikarus-0.3.0.dev202310000051/pyproject.toml
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 11:47:47.793167 pyikarus-0.3.0.dev202310000051/python/
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 11:47:47.882421 pyikarus-0.3.0.dev202310000051/python/ikarus/
+-rwxrwxrwx   0 user      (1001) user      (1001)      578 2023-05-10 11:30:04.000000 pyikarus-0.3.0.dev202310000051/python/ikarus/__init__.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 11:47:47.902424 pyikarus-0.3.0.dev202310000051/python/ikarus/assembler/
+-rwxrwxrwx   0 user      (1001) user      (1001)     2300 2023-05-10 11:30:04.000000 pyikarus-0.3.0.dev202310000051/python/ikarus/assembler/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1408 2023-05-10 11:30:04.000000 pyikarus-0.3.0.dev202310000051/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 11:47:47.922618 pyikarus-0.3.0.dev202310000051/python/ikarus/finite_elements/
+-rwxrwxrwx   0 user      (1001) user      (1001)     3465 2023-05-10 11:30:04.000000 pyikarus-0.3.0.dev202310000051/python/ikarus/finite_elements/__init__.py
+-rwxrwxrwx   0 user      (1001) user      (1001)     1792 2023-05-10 11:30:04.000000 pyikarus-0.3.0.dev202310000051/python/ikarus/materials.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 11:47:47.943270 pyikarus-0.3.0.dev202310000051/python/ikarus/utils/
+-rwxrwxrwx   0 user      (1001) user      (1001)     1461 2023-05-10 11:30:04.000000 pyikarus-0.3.0.dev202310000051/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 user      (1001) user      (1001)        0 2023-05-10 11:47:48.018194 pyikarus-0.3.0.dev202310000051/python/pyikarus.egg-info/
+-rw-r--r--   0 user      (1001) user      (1001)     3638 2023-05-10 11:47:47.000000 pyikarus-0.3.0.dev202310000051/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)      446 2023-05-10 11:47:47.000000 pyikarus-0.3.0.dev202310000051/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1001) user      (1001)        1 2023-05-10 11:47:47.000000 pyikarus-0.3.0.dev202310000051/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1001) user      (1001)      119 2023-05-10 11:47:47.000000 pyikarus-0.3.0.dev202310000051/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 user      (1001) user      (1001)        7 2023-05-10 11:47:47.000000 pyikarus-0.3.0.dev202310000051/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 user      (1001) user      (1001)       38 2023-05-10 11:47:48.036592 pyikarus-0.3.0.dev202310000051/setup.cfg
+-rwxrwxrwx   0 user      (1001) user      (1001)     1477 2023-05-10 11:47:38.000000 pyikarus-0.3.0.dev202310000051/setup.py
```

### Comparing `pyikarus-0.3.0.dev202310000050/LICENSE.md` & `pyikarus-0.3.0.dev202310000051/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000050/PKG-INFO` & `pyikarus-0.3.0.dev202310000051/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000050
+Version: 0.3.0.dev202310000051
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
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000050 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000051 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000050/README.md` & `pyikarus-0.3.0.dev202310000051/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.0.dev202310000050/python/pyikarus/__init__.py` & `pyikarus-0.3.0.dev202310000051/python/ikarus/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 # SPDX-License-Identifier: LGPL-3.0-or-later
 try:
     from dune.packagemetadata import registerExternalModule
     import pathlib
 
-    # register pyikarus to be recognized by dune-py (code generation module)
+    # register ikarus to be recognized by dune-py (code generation module)
     # as a module of the dune universe
     registerExternalModule(
-        moduleName="pyikarus",
+        moduleName="ikarus",
         modulePath=str(pathlib.Path(__file__).parent.resolve()),
     )
 
 except ImportError:
     pass
 
-from ._pyikarus import *
+from ._ikarus import *
 from .dirichletValues import dirichletValues
 from .materials import *
```

### Comparing `pyikarus-0.3.0.dev202310000050/python/pyikarus/assembler/__init__.py` & `pyikarus-0.3.0.dev202310000051/python/ikarus/assembler/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 
 def sparseFlatAssembler(fes, dirichletValues) :
     generator = MySimpleGenerator("SparseFlatAssembler", "Ikarus::Python")
     element_type = f"Ikarus::SparseFlatAssembler<std::vector<{fes[0].cppTypeName}>,{dirichletValues.cppTypeName}>"
 
     includes = []
-    includes += ["pyikarus/assembler/simpleAssemblers.hh"]
+    includes += ["ikarus/assembler/simpleAssemblers.hh"]
     includes += fes[0]._includes # include header of finite element
-    includes += ["pyikarus/python/assembler/flatAssembler.hh"]
+    includes += ["ikarus/python/assembler/flatAssembler.hh"]
     moduleName = "SparseFlatAssembler_" + hashIt(element_type)
     module = generator.load(
         includes=includes,
         typeName=element_type,
         moduleName=moduleName
     )
     return module.SparseFlatAssembler(fes,dirichletValues)
@@ -41,17 +41,17 @@
 
 def denseFlatAssembler(fes, dirichletValues) :
     # dune.generator.addToFlags(pre="-DCMAKE_PREFIX_PATH=/dune/dune-fufem ")
     generator = MySimpleGenerator("DenseFlatAssembler", "Ikarus::Python")
     element_type = f"Ikarus::DenseFlatAssembler<std::vector<{fes[0].cppTypeName}>,{dirichletValues.cppTypeName}>"
 
     includes = []
-    includes += ["pyikarus/assembler/simpleAssemblers.hh"]
-    includes += ["pyikarus/finiteElements/mechanics/linearElastic.hh"]
-    includes += ["pyikarus/python/assembler/flatAssembler.hh"]
+    includes += ["ikarus/assembler/simpleAssemblers.hh"]
+    includes += ["ikarus/finiteElements/mechanics/linearElastic.hh"]
+    includes += ["ikarus/python/assembler/flatAssembler.hh"]
     moduleName = "SparseFlatAssembler_" + hashIt(element_type)
     module = generator.load(
         includes=includes,
         typeName=element_type,
         moduleName=moduleName
     )
     return module.DenseFlatAssembler(fes,dirichletValues)
```

### Comparing `pyikarus-0.3.0.dev202310000050/python/pyikarus/dirichletValues.py` & `pyikarus-0.3.0.dev202310000051/python/ikarus/dirichletValues.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 
 def dirichletValues(basis) :
     generator = MySimpleGenerator("DirichletValues", "Ikarus::Python")
     element_type = f"Ikarus::DirichletValues<{basis.cppTypeName},Eigen::VectorX<bool>>"
 
     includes = []
-    includes += ["pyikarus/assembler/simpleAssemblers.hh"]
-    includes += ["pyikarus/python/dirichletValues/dirichletValues.hh"]
+    includes += ["ikarus/assembler/simpleAssemblers.hh"]
+    includes += ["ikarus/python/dirichletValues/dirichletValues.hh"]
     moduleName = "SparseFlatAssembler_" + hashIt(element_type)
     module = generator.load(
         includes=includes,
         typeName=element_type,
         moduleName=moduleName
     )
     return module.DirichletValues(basis)
```

### Comparing `pyikarus-0.3.0.dev202310000050/python/pyikarus/finite_elements/__init__.py` & `pyikarus-0.3.0.dev202310000051/python/ikarus/finite_elements/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     if not ((bp is None and neumannBoundaryLoad is None) or (bp is not None and neumannBoundaryLoad is not None)):
         raise TypeError("If you provide a boundary patch you should also provide a boundary load!")
 
     generator = MySimpleGenerator("LinearElastic", "Ikarus::Python")
     element_type = f"Ikarus::LinearElastic<{basis.cppTypeName},Ikarus::FErequirements<Eigen::Ref<Eigen::VectorXd>>,true>"
 
     includes = []
-    includes += ["pyikarus/finiteElements/mechanics/linearElastic.hh"]
-    includes += ["pyikarus/python/finiteElements/linearElastic.hh"]
+    includes += ["ikarus/finiteElements/mechanics/linearElastic.hh"]
+    includes += ["ikarus/python/finiteElements/linearElastic.hh"]
     moduleName = "linearElastic_" + hashIt(element_type)
     module = generator.load(
         includes=includes,
         typeName=element_type,
         moduleName=moduleName
     )
     # https://pybind11.readthedocs.io/en/stable/advanced/functions.html#allow-prohibiting-none-arguments
@@ -51,16 +51,16 @@
     if not ((bp is None and neumannBoundaryLoad is None) or (bp is not None and neumannBoundaryLoad is not None)):
         raise TypeError("If you provide a boundary patch you should also provide a boundary load!")
 
     generator = MySimpleGenerator("NonLinearElastic", "Ikarus::Python")
     element_type = f"Ikarus::NonLinearElastic<{basis.cppTypeName},  {material.cppTypeName} ,Ikarus::FErequirements<Eigen::Ref<Eigen::VectorXd>>,true>"
 
     includes = []
-    includes += ["pyikarus/finiteElements/mechanics/nonLinearElastic.hh"]
-    includes += ["pyikarus/python/finiteElements/nonLinearElastic.hh"]
+    includes += ["ikarus/finiteElements/mechanics/nonLinearElastic.hh"]
+    includes += ["ikarus/python/finiteElements/nonLinearElastic.hh"]
     moduleName = "nonLinearElastic_" + hashIt(element_type)
     module = generator.load(
         includes=includes,
         typeName=element_type,
         moduleName=moduleName
     )
     # https://pybind11.readthedocs.io/en/stable/advanced/functions.html#allow-prohibiting-none-arguments
```

### Comparing `pyikarus-0.3.0.dev202310000050/python/pyikarus/materials.py` & `pyikarus-0.3.0.dev202310000051/python/ikarus/materials.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 
 def materialConstructorDecorator(func):
     def wrapper(emodul,nu):
         generator = MySimpleGenerator(func.__name__, "Ikarus::Python")
         element_type = f"Ikarus::"+func.__name__+"<double>"
 
         includes = []
-        includes += ["pyikarus/finiteElements/mechanics/materials.hh"]
-        includes += ["pyikarus/python/finiteElements/materials/material.hh"]
+        includes += ["ikarus/finiteElements/mechanics/materials.hh"]
+        includes += ["ikarus/python/finiteElements/materials/material.hh"]
         moduleName = func.__name__+"_" + hashIt(element_type)
         module = generator.load(
             includes=includes,
             typeName=element_type,
             moduleName=moduleName
         )
```

### Comparing `pyikarus-0.3.0.dev202310000050/python/pyikarus/utils/__init__.py` & `pyikarus-0.3.0.dev202310000051/python/ikarus/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 def boundaryPatch(gridView,booleanVector) :
     dune.generator.addToFlags(pre="-DCMAKE_PREFIX_PATH=$ENV{CMAKE_PREFIX_PATH}")
     generator = MySimpleGenerator("BoundaryPatch", "Ikarus::Python")
     element_type = f"BoundaryPatch<{gridView.cppTypeName}>"
 
     includes = []
     includes += ["dune/fufem/boundarypatch.hh"]
-    includes += ["pyikarus/python/utils/boundarypatch.hh"]
+    includes += ["ikarus/python/utils/boundarypatch.hh"]
     moduleName = "boundaryPatch_" + hashIt(element_type)
     module = generator.load(
         includes=includes,
         typeName=element_type,
         moduleName=moduleName
     )
     return module.BoundaryPatch(gridView,booleanVector)
```

### Comparing `pyikarus-0.3.0.dev202310000050/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.0.dev202310000051/python/pyikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.0.dev202310000050
+Version: 0.3.0.dev202310000051
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
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000050 Home-page:
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.0.dev202310000051 Home-page:
 Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++ Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 (GPL) Requires-Python: >=3.4 Description-Content-Type: text/markdown License-
 File: LICENSE.md  # Ikarus [![Debian](https://github.com/ikarus-project/ikarus/
 actions/workflows/debian.yml/badge.svg)](https://github.com/ikarus-project/
 ikarus/actions/workflows/debian.yml) [![codecov](https://codecov.io/gh/ikarus-
```

### Comparing `pyikarus-0.3.0.dev202310000050/setup.py` & `pyikarus-0.3.0.dev202310000051/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 try:
     from dune.packagemetadata import metaData
 except ImportError:
     from packagemetadata import metaData
 from skbuild import setup
 
 # When building a new package, update the version numbers below and run:
-#
+# acess docker container with mounted repo to /tmp/Ikarus
+# build _ikarus
 # cd
 #  /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # > /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 # install locally:  pip install -v --pre --log logfile --find-links file://$PWD/dist ikarus==version
 # apt update
@@ -21,16 +22,17 @@
 # cat << EOF > ~/.pypirc
 # The current working directory is: $PWD
 # You are logged in as $(whoami)
 # EOF
 # nano ~/.pypirc
 # python -m venv /dune/dune-common/build-cmake/dune-env/
 # source /dune/dune-common/build-cmake/dune-env/bin/activate
-# pip install pyikarus  --no-build-isolation
+# pip install ikarus  --no-build-isolation
 
-pyikarusVersion = "0.3.0.dev202310000050" #+ datetime.today().time().strftime("%H%M%S")
+ikarusVersion = "0.3.0.dev202310000051" #+ datetime.today().time().strftime("%H%M%S")
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
-metadata["version"] = pyikarusVersion
+metadata["version"] = ikarusVersion
+metadata["name"] = "pyikarus"
 
 setup(**metadata)
```

