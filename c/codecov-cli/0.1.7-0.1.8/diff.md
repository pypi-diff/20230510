# Comparing `tmp/codecov-cli-0.1.7.tar.gz` & `tmp/codecov-cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codecov-cli-0.1.7.tar", last modified: Thu May  4 14:42:13 2023, max compression
+gzip compressed data, was "codecov-cli-0.1.8.tar", last modified: Wed May 10 07:34:28 2023, max compression
```

## Comparing `codecov-cli-0.1.7.tar` & `codecov-cli-0.1.8.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/codecov_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/codecov_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/base_picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/create_report_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/get_report_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/labelanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/staticanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/fallbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/appveyor_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/azure_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/bitrise_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/buildkite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/circleci.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/cirrus_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/codebuild.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/droneci.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/github_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/gitlab_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/teamcity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/travis_ci.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/woodpeckerci.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/folder_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/helpers/versioning_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/gcov.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/pycoverage.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/plugins/xcode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/runners/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/runners/dan_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/runners/python_standard_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/runners/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/commit/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/commit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/commit/base_picking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/report/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/report/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.336343 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/finders.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/staticanalysis/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.340343 codecov-cli-0.1.7/codecov_cli/services/upload/
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/coverage_file_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/legacy_upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/network_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/upload_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/services/upload/upload_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/codecov_cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/codecov_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 14:42:13.000000 codecov-cli-0.1.7/codecov_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.340343 codecov-cli-0.1.7/languages/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/languages/languages.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/languages/treesitterjavascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.340343 codecov-cli-0.1.7/languages/treesitterjavascript/src/
--rw-r--r--   0 runner    (1001) docker     (123)  2277994 2023-05-04 14:41:50.000000 codecov-cli-0.1.7/languages/treesitterjavascript/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-04 14:41:50.000000 codecov-cli-0.1.7/languages/treesitterjavascript/src/scanner.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.340343 codecov-cli-0.1.7/languages/treesitterjavascript/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-04 14:41:50.000000 codecov-cli-0.1.7/languages/treesitterjavascript/src/tree_sitter/parser.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.332343 codecov-cli-0.1.7/languages/treesitterpython/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/languages/treesitterpython/src/
--rw-r--r--   0 runner    (1001) docker     (123)  2658198 2023-05-04 14:41:51.000000 codecov-cli-0.1.7/languages/treesitterpython/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-04 14:41:51.000000 codecov-cli-0.1.7/languages/treesitterpython/src/scanner.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/languages/treesitterpython/src/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-04 14:41:51.000000 codecov-cli-0.1.7/languages/treesitterpython/src/tree_sitter/parser.h
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:42:13.344343 codecov-cli-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-04 14:41:47.000000 codecov-cli-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/codecov_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/codecov_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/base_picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/create_report_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/get_report_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/labelanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/staticanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/fallbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/codecov_cli/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/appveyor_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/azure_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/bitbucket_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/bitrise_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/buildkite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/circleci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/cirrus_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/codebuild.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/droneci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/github_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/gitlab_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/teamcity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/travis_ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/woodpeckerci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/folder_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/helpers/versioning_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/gcov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/pycoverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/plugins/xcode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/runners/dan_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5570 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/runners/python_standard_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/runners/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/commit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/commit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/commit/base_picking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.997497 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/finders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/staticanalysis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.001498 codecov-cli-0.1.8/codecov_cli/services/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/coverage_file_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/legacy_upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/network_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/upload_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/services/upload/upload_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/codecov_cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/codecov_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 07:34:27.000000 codecov-cli-0.1.8/codecov_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.001498 codecov-cli-0.1.8/languages/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/languages/languages.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/languages/treesitterjavascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.001498 codecov-cli-0.1.8/languages/treesitterjavascript/src/
+-rw-r--r--   0 runner    (1001) docker     (123)  2277994 2023-05-10 07:34:04.000000 codecov-cli-0.1.8/languages/treesitterjavascript/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-10 07:34:04.000000 codecov-cli-0.1.8/languages/treesitterjavascript/src/scanner.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.001498 codecov-cli-0.1.8/languages/treesitterjavascript/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-10 07:34:04.000000 codecov-cli-0.1.8/languages/treesitterjavascript/src/tree_sitter/parser.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:27.993497 codecov-cli-0.1.8/languages/treesitterpython/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/languages/treesitterpython/src/
+-rw-r--r--   0 runner    (1001) docker     (123)  2658198 2023-05-10 07:34:05.000000 codecov-cli-0.1.8/languages/treesitterpython/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-10 07:34:05.000000 codecov-cli-0.1.8/languages/treesitterpython/src/scanner.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/languages/treesitterpython/src/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-10 07:34:05.000000 codecov-cli-0.1.8/languages/treesitterpython/src/tree_sitter/parser.h
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 07:34:28.005498 codecov-cli-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-10 07:34:02.000000 codecov-cli-0.1.8/setup.py
```

### Comparing `codecov-cli-0.1.7/LICENSE` & `codecov-cli-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/PKG-INFO` & `codecov-cli-0.1.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,65 @@
-Metadata-Version: 2.1
-Name: codecov-cli
-Version: 0.1.7
-Summary: Codecov Command Line Interface
-Author: Codecov
-Author-email: support@codecov.io
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CodecovCLI 
 
 [![codecov](https://codecov.io/gh/codecov/codecov-cli/branch/master/graph/badge.svg?token=jN0CICuA6Z)](https://codecov.io/gh/codecov/codecov-cli)
 
-CodecovCLI is a new way for users to interact with Codecov directly from the user’s terminal or CI platform. Many Codecov features that require the user’s interference can be done via the codecovCLI. It saves commits, creates reports, uploads coverage and has many more amazing features.
+CodecovCLI is a new way for users to interact with Codecov directly from the user’s terminal or CI platform. Many Codecov features that require the user’s interference can be done via the codecovCLI. It saves commits, creates reports, uploads coverage and has many more features.
 
 - [Installing](#installing)
+  - [Using PIP](#using-pip)
+  - [As a Binary](#as-a-binary)
 - [Usage](#usage)
 - [Codecov-cli Commands](#codecov-cli-commands)
   - [create-commit](#create-commit)
   - [create-report](#create-report)
   - [do-upload](#do-upload)
   - [create-report-results](#create-report-results)
   - [get-report-results](#get-report-results)
   - [pr-base-picking](#pr-base-picking)
 - [How to upload to Codecov](#how-to-upload-to-codecov)
-- [How to Local upload](#how-to-local-upload)
-- [Plugin System](#plugin-system)
+- [How to Use Local Upload](#how-to-use-local-upload)
+- [Work in Progress Features](#work-in-progress-features)
+  - [Plugin System](#plugin-system)
+  - [Static Analysis](#static-analysis)
 - [Contributions](#contributions)
   - [Requirements](#requirements)
   - [Guidelines](#guidelines)
 - [Releases](#releases)
 
 # Installing
 
-To use codecov-cli in your local machine, or your CI workflows, you need to install it
+## Using PIP
+To use codecov-cli in your local machine, or your CI workflows, you need to install it:
 
 `pip install codecov-cli`
 
-The above command will download the latest version of Codecov-cli. If you wish to use a specific version, releases can be viewed [here](). 
-You can also find Codecovcli [here](https://cli.codecov.io/) or in the [Github releases](https://github.com/codecov/codecov-cli/releases) where you can download the binary distributable files. 
+The above command will download the latest version of Codecov-cli. If you wish to use a specific version, releases can be viewed [here](https://pypi.org/project/codecov-cli/#history). 
+
+## As a Binary
+If you would like to use the CLI in an environment that does not have access to Python / PIP, you can install the CLI as a compiled binary. Linux and macOS releases can be found [here](https://cli.codecov.io/), along with SHASUMs and signatures for each released version. Binary releases are also available via [Github releases](https://github.com/codecov/codecov-cli/releases) on this repository. 
 
 # Usage 
 If the installation is successful, running `codecovcli --help` will output the available commands along with the different general options that can be used with them. 
 ```
 Usage: codecovcli [OPTIONS] COMMAND [ARGS]...
 ```
-Codecov-cli supports inputs from the user. These inputs, along with their descriptions and usage contexts, are listed in the table below:
+Codecov-cli supports user input. These inputs, along with their descriptions and usage contexts, are listed in the table below:
 
 | Input  | Description | Usage |
 | :---:     |     :---:   |    :---:   |
 | `--auto-load-params-from`  | The CI/CD platform   | Optional |
 | `--codecov-yml-path` | The path for your codecov.yml  | Optional
 | `--enterprise-url` | Change the upload host (Enterprise use) | Optional
 | `--version` | Codecov-cli's version | Optional
 | `--verbose` or `-v` | Run the cli with verbose logging | Optional 
 
 # Codecov-cli Commands
 | Command  | Description | 
 | :---:     |     :---:   |    
-| `create-commit` | Saves the commit's metadata in codecov, only need to do it once for a commit 
+| `create-commit` | Saves the commit's metadata in codecov, it's only necessry to run this once per commit 
 | `create-report` | Creates an empty report in codecov with initial data e.g. report name, report's commit 
 | `do-upload` | Searches for and uploads coverage data to codecov 
 | `create-report-results` | Used for local upload. It tells codecov that you finished local uploading and want it to calculate the results for you to get them locally.
 | `get-report-results` | Used for local upload. It asks codecov to provide you the report results you calculated with the previous command. 
 | `pr-base-picking` | Tells codecov that you want to explicitly define a base for your PR
 
 >**Note**: Every command has its own different options that will be mentioned later in this doc. Codecov will try to load these options from your CI environment variables, if not, it will try to load them from git, if not found, you may need to add them manually. 
@@ -155,79 +153,90 @@
 |--base-sha | Base commit SHA (with 40 chars) | Required
 |--pr  | Pull Request id to associate commit with | Required
 |--slug | owner/repo slug | Required
 |-t, --token| Codecov upload token | Required
 |--service | Git provider. Options: github, gitlab, bitbucket, github_enterprise, gitlab_enterprise, bitbucket_server | Optional
 |--help | Shows usage, and command options
 
-# How to upload to Codecov
-In your CI workflow, you need to add these commands: 
+# How to Upload to Codecov
+If desired, the CLI can be used as a replacement for our [NodeJS Binary Uploader](https://github.com/codecov/uploader). To use the CLI to upload from your CI workflow, you need to add these commands: 
+
 ```
 pip install codecovcli
 codecovcli create-commit
 codecovcli create-report
 codecovcli do-upload
 ```
 You can customize the commands with the options aligned with each command. 
 
-# How to Local upload: 
-If you CI workflow takes too much time to run, and you have to wait for it to finish to know the coverage results, you can make your changes locally, make a PR and then run these commands:  
+# How to Use Local Upload
+
+The CLI also supports "dry run" local uploading. This is useful if you prefer to see Codecov status checks and coverage reporting locally, in your terminal, as opposed to opening a PR and waiting for your full CI to run. Local uploads do not interfere with regular uploads made from your CI for any given commit / Pull Request. 
+
+Local Upload is accomplished as follows:
+
 ```
 pip install codecovcli
 codecovcli create-commit
 codecovcli create-report --code <CODE>
 codecovcli do-upload --report-code <CODE>
 codecovcli create-report-results --code <CODE>
 codecovcli get-report-results --code <CODE>
 ```
 
 Codecov will calculate the coverage results, and return them in your terminal, telling you whether your PR will fail or pass the coverage check.
 
+Note: In order for Local Upload to work, it must be used against a commit on the origin repository. Local Upload does not work for arbitrary diffs or uncommitted changes on your local machine. 
+
+# Work in Progress Features
+
+The following features are somewhat implemented in code, but are not yet meant for use. These features will be documented once they are fully implemented in the CLI. 
 
-# Plugin System
+## Plugin System
 
-In some of the commands, there is a plugin system. For most cases, one might find that changing them is not really needed. But in some cases, have some custom logic run would be beneficial
+To provide extensibility to some of its commands, the CLI makes use of a plugin system. For most cases, the default commands are sufficient. But in some cases, having some custom logic specific to your use case can be beneficial. Note that full documentation of the plugin system is pending, as the feature is still heavily a work in progress.
 
+## Static Analysis
 
-WIP
+The CLI can perform basic static analysis on Python code today. This static analysis is meant to power more future looking Codecov features and, as such, is not required or in active use today. As more functionality dependent on static analysis becomes available for use, we will document static analysis in detail here. 
 
 # Contributions
 
 ## Requirements
 
-To start, most of this package is a normal Python package. The main different thing is the static analysis tool that uses both git submodules and c code
+Most of this package is a very conventional Python package. The main difference is the static the CLI's analysis module uses both git submodules and C code
 
-Before installing, one should pull the submodules with
+Before installing, one should pull the submodules with:
 
 ```
 git submodule update --init
 ```
 Then, install dependencies with
 ```
 pip install -r requirements.txt 
 python setup.py develop
 ```
 
-The c code shouldn't require anything in most places, but it might ask you to install compilers and stuff. Most of the times you can find the instructions online given the error message
+The C code shouldn't require anything additional setup to get running, but depending on your enviroment, you may be prompted to install compilers and supporting tools. If errors are generating during installation, it is likely due to missing dependencies / tools required of the C code. In many cases, resulting error messages should be clear enough to determine what is missing and how to install it, but common errors will be collected here as they are encountered.
 
 ## Guidelines
 
-There are a few guidelines when developing in this systems. We have a few notable folders:
+There are a few guidelines when developing in this systems. Some notable folders:
 
-1. `commands` - It's the folder that interacts with the caller. This is where the commands themselves should live. They are not meant to do heavy lifting. They only do wiring, which is mostly parsing the input parameters
-2. `services` - It's where the heavy logic lives. It's mostly organizaed by which command needs them.
-3. `helpers` - This is meant for logic that is probably useful accross different commands. For example, logging helpers, or the logic the searches folders
+1. `commands` - It's the folder that interacts with the caller. This is where the commands themselves should reside. These commands are not meant to do heavy lifting. They only do wiring, which is mostly parsing the input parameters. 
+2. `services` - It's where the heavy logic resides. It's mostly organizaed by which command needs them. Commands should generally be thin wrappers around these services.
+3. `helpers` - This is meant for logic that is useful accross different commands. For example, logging helpers, or the logic the searches folders.
 
 # Releases
 
 The standard way to making a new release is the following:
-1)  Open a PR that increases the version number in setup.py. As a rule of thumb, just add one to the micro version (number most to the right).
+1)  Open a PR that increases the version number in setup.py. As a rule of thumb, just add one to the micro/patch version (e.g., v0.1.6 -> v0.1.7).
 
 2) Get the up-to-date master branch locally and run the `tag.release` command from the Makefile.
 
 `$ make tag.release version=v<VERSION_NUM>`
 
 The version tag must match the regex defined on the Makefile (`tag_regex := ^v([0-9]{1,}\.){2}[0-9]{1,}([-_]\w+)?$`).
 
 >**Note**: \
 >Releases with `test` word in them are created as `draft`. \
->Releases with `beta` work in them are created as `pre-release`.
+>Releases with `beta` word in them are created as `pre-release`.
```

### Comparing `codecov-cli-0.1.7/README.md` & `codecov-cli-0.1.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,74 @@
+Metadata-Version: 2.1
+Name: codecov-cli
+Version: 0.1.8
+Summary: Codecov Command Line Interface
+Author: Codecov
+Author-email: support@codecov.io
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # CodecovCLI 
 
 [![codecov](https://codecov.io/gh/codecov/codecov-cli/branch/master/graph/badge.svg?token=jN0CICuA6Z)](https://codecov.io/gh/codecov/codecov-cli)
 
-CodecovCLI is a new way for users to interact with Codecov directly from the user’s terminal or CI platform. Many Codecov features that require the user’s interference can be done via the codecovCLI. It saves commits, creates reports, uploads coverage and has many more amazing features.
+CodecovCLI is a new way for users to interact with Codecov directly from the user’s terminal or CI platform. Many Codecov features that require the user’s interference can be done via the codecovCLI. It saves commits, creates reports, uploads coverage and has many more features.
 
 - [Installing](#installing)
+  - [Using PIP](#using-pip)
+  - [As a Binary](#as-a-binary)
 - [Usage](#usage)
 - [Codecov-cli Commands](#codecov-cli-commands)
   - [create-commit](#create-commit)
   - [create-report](#create-report)
   - [do-upload](#do-upload)
   - [create-report-results](#create-report-results)
   - [get-report-results](#get-report-results)
   - [pr-base-picking](#pr-base-picking)
 - [How to upload to Codecov](#how-to-upload-to-codecov)
-- [How to Local upload](#how-to-local-upload)
-- [Plugin System](#plugin-system)
+- [How to Use Local Upload](#how-to-use-local-upload)
+- [Work in Progress Features](#work-in-progress-features)
+  - [Plugin System](#plugin-system)
+  - [Static Analysis](#static-analysis)
 - [Contributions](#contributions)
   - [Requirements](#requirements)
   - [Guidelines](#guidelines)
 - [Releases](#releases)
 
 # Installing
 
-To use codecov-cli in your local machine, or your CI workflows, you need to install it
+## Using PIP
+To use codecov-cli in your local machine, or your CI workflows, you need to install it:
 
 `pip install codecov-cli`
 
-The above command will download the latest version of Codecov-cli. If you wish to use a specific version, releases can be viewed [here](). 
-You can also find Codecovcli [here](https://cli.codecov.io/) or in the [Github releases](https://github.com/codecov/codecov-cli/releases) where you can download the binary distributable files. 
+The above command will download the latest version of Codecov-cli. If you wish to use a specific version, releases can be viewed [here](https://pypi.org/project/codecov-cli/#history). 
+
+## As a Binary
+If you would like to use the CLI in an environment that does not have access to Python / PIP, you can install the CLI as a compiled binary. Linux and macOS releases can be found [here](https://cli.codecov.io/), along with SHASUMs and signatures for each released version. Binary releases are also available via [Github releases](https://github.com/codecov/codecov-cli/releases) on this repository. 
 
 # Usage 
 If the installation is successful, running `codecovcli --help` will output the available commands along with the different general options that can be used with them. 
 ```
 Usage: codecovcli [OPTIONS] COMMAND [ARGS]...
 ```
-Codecov-cli supports inputs from the user. These inputs, along with their descriptions and usage contexts, are listed in the table below:
+Codecov-cli supports user input. These inputs, along with their descriptions and usage contexts, are listed in the table below:
 
 | Input  | Description | Usage |
 | :---:     |     :---:   |    :---:   |
 | `--auto-load-params-from`  | The CI/CD platform   | Optional |
 | `--codecov-yml-path` | The path for your codecov.yml  | Optional
 | `--enterprise-url` | Change the upload host (Enterprise use) | Optional
 | `--version` | Codecov-cli's version | Optional
 | `--verbose` or `-v` | Run the cli with verbose logging | Optional 
 
 # Codecov-cli Commands
 | Command  | Description | 
 | :---:     |     :---:   |    
-| `create-commit` | Saves the commit's metadata in codecov, only need to do it once for a commit 
+| `create-commit` | Saves the commit's metadata in codecov, it's only necessry to run this once per commit 
 | `create-report` | Creates an empty report in codecov with initial data e.g. report name, report's commit 
 | `do-upload` | Searches for and uploads coverage data to codecov 
 | `create-report-results` | Used for local upload. It tells codecov that you finished local uploading and want it to calculate the results for you to get them locally.
 | `get-report-results` | Used for local upload. It asks codecov to provide you the report results you calculated with the previous command. 
 | `pr-base-picking` | Tells codecov that you want to explicitly define a base for your PR
 
 >**Note**: Every command has its own different options that will be mentioned later in this doc. Codecov will try to load these options from your CI environment variables, if not, it will try to load them from git, if not found, you may need to add them manually. 
@@ -146,79 +162,90 @@
 |--base-sha | Base commit SHA (with 40 chars) | Required
 |--pr  | Pull Request id to associate commit with | Required
 |--slug | owner/repo slug | Required
 |-t, --token| Codecov upload token | Required
 |--service | Git provider. Options: github, gitlab, bitbucket, github_enterprise, gitlab_enterprise, bitbucket_server | Optional
 |--help | Shows usage, and command options
 
-# How to upload to Codecov
-In your CI workflow, you need to add these commands: 
+# How to Upload to Codecov
+If desired, the CLI can be used as a replacement for our [NodeJS Binary Uploader](https://github.com/codecov/uploader). To use the CLI to upload from your CI workflow, you need to add these commands: 
+
 ```
 pip install codecovcli
 codecovcli create-commit
 codecovcli create-report
 codecovcli do-upload
 ```
 You can customize the commands with the options aligned with each command. 
 
-# How to Local upload: 
-If you CI workflow takes too much time to run, and you have to wait for it to finish to know the coverage results, you can make your changes locally, make a PR and then run these commands:  
+# How to Use Local Upload
+
+The CLI also supports "dry run" local uploading. This is useful if you prefer to see Codecov status checks and coverage reporting locally, in your terminal, as opposed to opening a PR and waiting for your full CI to run. Local uploads do not interfere with regular uploads made from your CI for any given commit / Pull Request. 
+
+Local Upload is accomplished as follows:
+
 ```
 pip install codecovcli
 codecovcli create-commit
 codecovcli create-report --code <CODE>
 codecovcli do-upload --report-code <CODE>
 codecovcli create-report-results --code <CODE>
 codecovcli get-report-results --code <CODE>
 ```
 
 Codecov will calculate the coverage results, and return them in your terminal, telling you whether your PR will fail or pass the coverage check.
 
+Note: In order for Local Upload to work, it must be used against a commit on the origin repository. Local Upload does not work for arbitrary diffs or uncommitted changes on your local machine. 
+
+# Work in Progress Features
+
+The following features are somewhat implemented in code, but are not yet meant for use. These features will be documented once they are fully implemented in the CLI. 
 
-# Plugin System
+## Plugin System
 
-In some of the commands, there is a plugin system. For most cases, one might find that changing them is not really needed. But in some cases, have some custom logic run would be beneficial
+To provide extensibility to some of its commands, the CLI makes use of a plugin system. For most cases, the default commands are sufficient. But in some cases, having some custom logic specific to your use case can be beneficial. Note that full documentation of the plugin system is pending, as the feature is still heavily a work in progress.
 
+## Static Analysis
 
-WIP
+The CLI can perform basic static analysis on Python code today. This static analysis is meant to power more future looking Codecov features and, as such, is not required or in active use today. As more functionality dependent on static analysis becomes available for use, we will document static analysis in detail here. 
 
 # Contributions
 
 ## Requirements
 
-To start, most of this package is a normal Python package. The main different thing is the static analysis tool that uses both git submodules and c code
+Most of this package is a very conventional Python package. The main difference is the static the CLI's analysis module uses both git submodules and C code
 
-Before installing, one should pull the submodules with
+Before installing, one should pull the submodules with:
 
 ```
 git submodule update --init
 ```
 Then, install dependencies with
 ```
 pip install -r requirements.txt 
 python setup.py develop
 ```
 
-The c code shouldn't require anything in most places, but it might ask you to install compilers and stuff. Most of the times you can find the instructions online given the error message
+The C code shouldn't require anything additional setup to get running, but depending on your enviroment, you may be prompted to install compilers and supporting tools. If errors are generating during installation, it is likely due to missing dependencies / tools required of the C code. In many cases, resulting error messages should be clear enough to determine what is missing and how to install it, but common errors will be collected here as they are encountered.
 
 ## Guidelines
 
-There are a few guidelines when developing in this systems. We have a few notable folders:
+There are a few guidelines when developing in this systems. Some notable folders:
 
-1. `commands` - It's the folder that interacts with the caller. This is where the commands themselves should live. They are not meant to do heavy lifting. They only do wiring, which is mostly parsing the input parameters
-2. `services` - It's where the heavy logic lives. It's mostly organizaed by which command needs them.
-3. `helpers` - This is meant for logic that is probably useful accross different commands. For example, logging helpers, or the logic the searches folders
+1. `commands` - It's the folder that interacts with the caller. This is where the commands themselves should reside. These commands are not meant to do heavy lifting. They only do wiring, which is mostly parsing the input parameters. 
+2. `services` - It's where the heavy logic resides. It's mostly organizaed by which command needs them. Commands should generally be thin wrappers around these services.
+3. `helpers` - This is meant for logic that is useful accross different commands. For example, logging helpers, or the logic the searches folders.
 
 # Releases
 
 The standard way to making a new release is the following:
-1)  Open a PR that increases the version number in setup.py. As a rule of thumb, just add one to the micro version (number most to the right).
+1)  Open a PR that increases the version number in setup.py. As a rule of thumb, just add one to the micro/patch version (e.g., v0.1.6 -> v0.1.7).
 
 2) Get the up-to-date master branch locally and run the `tag.release` command from the Makefile.
 
 `$ make tag.release version=v<VERSION_NUM>`
 
 The version tag must match the regex defined on the Makefile (`tag_regex := ^v([0-9]{1,}\.){2}[0-9]{1,}([-_]\w+)?$`).
 
 >**Note**: \
 >Releases with `test` word in them are created as `draft`. \
->Releases with `beta` work in them are created as `pre-release`.
+>Releases with `beta` word in them are created as `pre-release`.
```

### Comparing `codecov-cli-0.1.7/codecov_cli/commands/base_picking.py` & `codecov-cli-0.1.8/codecov_cli/commands/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/commands/commit.py` & `codecov-cli-0.1.8/codecov_cli/commands/commit.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/commands/create_report_result.py` & `codecov-cli-0.1.8/codecov_cli/commands/create_report_result.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/commands/get_report_results.py` & `codecov-cli-0.1.8/codecov_cli/commands/get_report_results.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/commands/labelanalysis.py` & `codecov-cli-0.1.8/codecov_cli/commands/labelanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/commands/report.py` & `codecov-cli-0.1.8/codecov_cli/commands/report.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/commands/staticanalysis.py` & `codecov-cli-0.1.8/codecov_cli/commands/staticanalysis.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/commands/upload.py` & `codecov-cli-0.1.8/codecov_cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/fallbacks.py` & `codecov-cli-0.1.8/codecov_cli/fallbacks.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/__init__.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/appveyor_ci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/appveyor_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/azure_pipelines.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/azure_pipelines.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/base.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/base.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/bitbucket_ci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/bitbucket_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/bitrise_ci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/bitrise_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/buildkite.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/buildkite.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/circleci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/circleci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/cirrus_ci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/cirrus_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/codebuild.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/codebuild.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/droneci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/droneci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/github_actions.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/github_actions.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/gitlab_ci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/gitlab_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/heroku.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/heroku.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/jenkins.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/jenkins.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/local.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/local.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/teamcity.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/teamcity.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/travis_ci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/travis_ci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/ci_adapters/woodpeckerci.py` & `codecov-cli-0.1.8/codecov_cli/helpers/ci_adapters/woodpeckerci.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/encoder.py` & `codecov-cli-0.1.8/codecov_cli/helpers/encoder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/folder_searcher.py` & `codecov-cli-0.1.8/codecov_cli/helpers/folder_searcher.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/git.py` & `codecov-cli-0.1.8/codecov_cli/helpers/git.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/logging_utils.py` & `codecov-cli-0.1.8/codecov_cli/helpers/logging_utils.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/request.py` & `codecov-cli-0.1.8/codecov_cli/helpers/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,19 @@
         status_code=resp.status_code, error=None, warnings=[], text=resp.text
     )
 
 
 def log_warnings_and_errors_if_any(
     sending_result: RequestResult, process_desc: str, fail_on_error: bool = False
 ):
+    logger.info(
+        f"Process {process_desc} complete",
+    )
     logger.debug(
-        f"Process {process_desc} complete.",
+        f"{process_desc} result",
         extra=dict(extra_log_attributes=dict(result=sending_result)),
     )
     if sending_result.warnings:
         number_warnings = len(sending_result.warnings)
         pluralization = "s" if number_warnings > 1 else ""
         logger.info(
             f"{process_desc} process had {number_warnings} warning{pluralization}",
```

### Comparing `codecov-cli-0.1.7/codecov_cli/helpers/versioning_systems.py` & `codecov-cli-0.1.8/codecov_cli/helpers/versioning_systems.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/main.py` & `codecov-cli-0.1.8/codecov_cli/main.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/plugins/__init__.py` & `codecov-cli-0.1.8/codecov_cli/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/plugins/gcov.py` & `codecov-cli-0.1.8/codecov_cli/plugins/gcov.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/plugins/pycoverage.py` & `codecov-cli-0.1.8/codecov_cli/plugins/pycoverage.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/plugins/xcode.py` & `codecov-cli-0.1.8/codecov_cli/plugins/xcode.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/runners/__init__.py` & `codecov-cli-0.1.8/codecov_cli/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/runners/dan_runner.py` & `codecov-cli-0.1.8/codecov_cli/runners/dan_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/runners/python_standard_runner.py` & `codecov-cli-0.1.8/codecov_cli/runners/python_standard_runner.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/commit/__init__.py` & `codecov-cli-0.1.8/codecov_cli/services/commit/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/commit/base_picking.py` & `codecov-cli-0.1.8/codecov_cli/services/commit/base_picking.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/report/__init__.py` & `codecov-cli-0.1.8/codecov_cli/services/report/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/__init__.py` & `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py` & `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/ecmascriptsix.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/__init__.py` & `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py` & `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/analyzers/python/node_wrappers.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/staticanalysis/finders.py` & `codecov-cli-0.1.8/codecov_cli/services/staticanalysis/finders.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/upload/__init__.py` & `codecov-cli-0.1.8/codecov_cli/services/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/upload/coverage_file_finder.py` & `codecov-cli-0.1.8/codecov_cli/services/upload/coverage_file_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/upload/legacy_upload_sender.py` & `codecov-cli-0.1.8/codecov_cli/services/upload/legacy_upload_sender.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/upload/network_finder.py` & `codecov-cli-0.1.8/codecov_cli/services/upload/network_finder.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli/services/upload/upload_collector.py` & `codecov-cli-0.1.8/codecov_cli/services/upload/upload_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     def generate_upload_data(self) -> UploadCollectionResult:
         for prep in self.preparation_plugins:
             logger.debug(f"Running preparation plugin: {type(prep)}")
             prep.run_preparation(self)
         logger.debug("Collecting relevant files")
         network = self.network_finder.find_files()
         coverage_files = self.coverage_file_finder.find_coverage_files()
-        logger.debug(f"Found {len(coverage_files)} coverage files to upload")
+        logger.info(f"Found {len(coverage_files)} coverage files to upload")
         for file in coverage_files:
-            logger.debug(f"> {file}")
+            logger.info(f"> {file}")
         return UploadCollectionResult(
             network=network,
             coverage_files=coverage_files,
             file_fixes=self._produce_file_fixes_for_network(network),
         )
```

### Comparing `codecov-cli-0.1.7/codecov_cli/services/upload/upload_sender.py` & `codecov-cli-0.1.8/codecov_cli/services/upload/upload_sender.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import json
+import logging
 import typing
 import uuid
 import zlib
 from typing import Any, Dict
 
 from codecov_cli.helpers.encoder import encode_slug
 from codecov_cli.helpers.request import (
@@ -13,14 +14,16 @@
 )
 from codecov_cli.types import (
     RequestResult,
     UploadCollectionResult,
     UploadCollectionResultFile,
 )
 
+logger = logging.getLogger("codecovcli")
+
 
 class UploadSender(object):
     def send_upload_data(
         self,
         upload_data: UploadCollectionResult,
         commit_sha: str,
         token: uuid.UUID,
@@ -42,27 +45,34 @@
             "ci_url": build_url,
             "flags": flags,
             "env": env_vars,
             "name": name,
             "job_code": job_code,
         }
 
+        # Data to upload to Codecov
         headers = get_token_header_or_fail(token)
         encoded_slug = encode_slug(slug)
         url = f"https://api.codecov.io/upload/{git_service}/{encoded_slug}/commits/{commit_sha}/reports/{report_code}/uploads"
-        resp = send_post_request(url=url, data=data, headers=headers)
-
-        if resp.status_code >= 400:
-            return resp
+        # Data that goes to storage
+        reports_payload = self._generate_payload(upload_data, env_vars)
 
-        resp_json_obj = json.loads(resp.text)
+        logger.debug("Sending upload request to Codecov")
+        resp_from_codecov = send_post_request(url=url, data=data, headers=headers)
+        if resp_from_codecov.status_code >= 400:
+            return resp_from_codecov
+        resp_json_obj = json.loads(resp_from_codecov.text)
+        logger.debug(
+            "Upload request to Codecov complete.",
+            extra=dict(extra_log_attributes=dict(response=resp_json_obj)),
+        )
         put_url = resp_json_obj["raw_upload_location"]
-        reports_payload = self._generate_payload(upload_data, env_vars)
-        resp = send_put_request(put_url, data=reports_payload)
-        return resp
+        logger.debug("Sending upload to storage")
+        resp_from_storage = send_put_request(put_url, data=reports_payload)
+        return resp_from_storage
 
     def _generate_payload(
         self, upload_data: UploadCollectionResult, env_vars: typing.Dict[str, str]
     ) -> bytes:
         network_files = upload_data.network
         payload = {
             "path_fixes": {
```

### Comparing `codecov-cli-0.1.7/codecov_cli/types.py` & `codecov-cli-0.1.8/codecov_cli/types.py`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/codecov_cli.egg-info/PKG-INFO` & `codecov-cli-0.1.8/codecov_cli.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,74 @@
 Metadata-Version: 2.1
 Name: codecov-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: Codecov Command Line Interface
 Author: Codecov
 Author-email: support@codecov.io
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CodecovCLI 
 
 [![codecov](https://codecov.io/gh/codecov/codecov-cli/branch/master/graph/badge.svg?token=jN0CICuA6Z)](https://codecov.io/gh/codecov/codecov-cli)
 
-CodecovCLI is a new way for users to interact with Codecov directly from the user’s terminal or CI platform. Many Codecov features that require the user’s interference can be done via the codecovCLI. It saves commits, creates reports, uploads coverage and has many more amazing features.
+CodecovCLI is a new way for users to interact with Codecov directly from the user’s terminal or CI platform. Many Codecov features that require the user’s interference can be done via the codecovCLI. It saves commits, creates reports, uploads coverage and has many more features.
 
 - [Installing](#installing)
+  - [Using PIP](#using-pip)
+  - [As a Binary](#as-a-binary)
 - [Usage](#usage)
 - [Codecov-cli Commands](#codecov-cli-commands)
   - [create-commit](#create-commit)
   - [create-report](#create-report)
   - [do-upload](#do-upload)
   - [create-report-results](#create-report-results)
   - [get-report-results](#get-report-results)
   - [pr-base-picking](#pr-base-picking)
 - [How to upload to Codecov](#how-to-upload-to-codecov)
-- [How to Local upload](#how-to-local-upload)
-- [Plugin System](#plugin-system)
+- [How to Use Local Upload](#how-to-use-local-upload)
+- [Work in Progress Features](#work-in-progress-features)
+  - [Plugin System](#plugin-system)
+  - [Static Analysis](#static-analysis)
 - [Contributions](#contributions)
   - [Requirements](#requirements)
   - [Guidelines](#guidelines)
 - [Releases](#releases)
 
 # Installing
 
-To use codecov-cli in your local machine, or your CI workflows, you need to install it
+## Using PIP
+To use codecov-cli in your local machine, or your CI workflows, you need to install it:
 
 `pip install codecov-cli`
 
-The above command will download the latest version of Codecov-cli. If you wish to use a specific version, releases can be viewed [here](). 
-You can also find Codecovcli [here](https://cli.codecov.io/) or in the [Github releases](https://github.com/codecov/codecov-cli/releases) where you can download the binary distributable files. 
+The above command will download the latest version of Codecov-cli. If you wish to use a specific version, releases can be viewed [here](https://pypi.org/project/codecov-cli/#history). 
+
+## As a Binary
+If you would like to use the CLI in an environment that does not have access to Python / PIP, you can install the CLI as a compiled binary. Linux and macOS releases can be found [here](https://cli.codecov.io/), along with SHASUMs and signatures for each released version. Binary releases are also available via [Github releases](https://github.com/codecov/codecov-cli/releases) on this repository. 
 
 # Usage 
 If the installation is successful, running `codecovcli --help` will output the available commands along with the different general options that can be used with them. 
 ```
 Usage: codecovcli [OPTIONS] COMMAND [ARGS]...
 ```
-Codecov-cli supports inputs from the user. These inputs, along with their descriptions and usage contexts, are listed in the table below:
+Codecov-cli supports user input. These inputs, along with their descriptions and usage contexts, are listed in the table below:
 
 | Input  | Description | Usage |
 | :---:     |     :---:   |    :---:   |
 | `--auto-load-params-from`  | The CI/CD platform   | Optional |
 | `--codecov-yml-path` | The path for your codecov.yml  | Optional
 | `--enterprise-url` | Change the upload host (Enterprise use) | Optional
 | `--version` | Codecov-cli's version | Optional
 | `--verbose` or `-v` | Run the cli with verbose logging | Optional 
 
 # Codecov-cli Commands
 | Command  | Description | 
 | :---:     |     :---:   |    
-| `create-commit` | Saves the commit's metadata in codecov, only need to do it once for a commit 
+| `create-commit` | Saves the commit's metadata in codecov, it's only necessry to run this once per commit 
 | `create-report` | Creates an empty report in codecov with initial data e.g. report name, report's commit 
 | `do-upload` | Searches for and uploads coverage data to codecov 
 | `create-report-results` | Used for local upload. It tells codecov that you finished local uploading and want it to calculate the results for you to get them locally.
 | `get-report-results` | Used for local upload. It asks codecov to provide you the report results you calculated with the previous command. 
 | `pr-base-picking` | Tells codecov that you want to explicitly define a base for your PR
 
 >**Note**: Every command has its own different options that will be mentioned later in this doc. Codecov will try to load these options from your CI environment variables, if not, it will try to load them from git, if not found, you may need to add them manually. 
@@ -155,79 +162,90 @@
 |--base-sha | Base commit SHA (with 40 chars) | Required
 |--pr  | Pull Request id to associate commit with | Required
 |--slug | owner/repo slug | Required
 |-t, --token| Codecov upload token | Required
 |--service | Git provider. Options: github, gitlab, bitbucket, github_enterprise, gitlab_enterprise, bitbucket_server | Optional
 |--help | Shows usage, and command options
 
-# How to upload to Codecov
-In your CI workflow, you need to add these commands: 
+# How to Upload to Codecov
+If desired, the CLI can be used as a replacement for our [NodeJS Binary Uploader](https://github.com/codecov/uploader). To use the CLI to upload from your CI workflow, you need to add these commands: 
+
 ```
 pip install codecovcli
 codecovcli create-commit
 codecovcli create-report
 codecovcli do-upload
 ```
 You can customize the commands with the options aligned with each command. 
 
-# How to Local upload: 
-If you CI workflow takes too much time to run, and you have to wait for it to finish to know the coverage results, you can make your changes locally, make a PR and then run these commands:  
+# How to Use Local Upload
+
+The CLI also supports "dry run" local uploading. This is useful if you prefer to see Codecov status checks and coverage reporting locally, in your terminal, as opposed to opening a PR and waiting for your full CI to run. Local uploads do not interfere with regular uploads made from your CI for any given commit / Pull Request. 
+
+Local Upload is accomplished as follows:
+
 ```
 pip install codecovcli
 codecovcli create-commit
 codecovcli create-report --code <CODE>
 codecovcli do-upload --report-code <CODE>
 codecovcli create-report-results --code <CODE>
 codecovcli get-report-results --code <CODE>
 ```
 
 Codecov will calculate the coverage results, and return them in your terminal, telling you whether your PR will fail or pass the coverage check.
 
+Note: In order for Local Upload to work, it must be used against a commit on the origin repository. Local Upload does not work for arbitrary diffs or uncommitted changes on your local machine. 
+
+# Work in Progress Features
+
+The following features are somewhat implemented in code, but are not yet meant for use. These features will be documented once they are fully implemented in the CLI. 
 
-# Plugin System
+## Plugin System
 
-In some of the commands, there is a plugin system. For most cases, one might find that changing them is not really needed. But in some cases, have some custom logic run would be beneficial
+To provide extensibility to some of its commands, the CLI makes use of a plugin system. For most cases, the default commands are sufficient. But in some cases, having some custom logic specific to your use case can be beneficial. Note that full documentation of the plugin system is pending, as the feature is still heavily a work in progress.
 
+## Static Analysis
 
-WIP
+The CLI can perform basic static analysis on Python code today. This static analysis is meant to power more future looking Codecov features and, as such, is not required or in active use today. As more functionality dependent on static analysis becomes available for use, we will document static analysis in detail here. 
 
 # Contributions
 
 ## Requirements
 
-To start, most of this package is a normal Python package. The main different thing is the static analysis tool that uses both git submodules and c code
+Most of this package is a very conventional Python package. The main difference is the static the CLI's analysis module uses both git submodules and C code
 
-Before installing, one should pull the submodules with
+Before installing, one should pull the submodules with:
 
 ```
 git submodule update --init
 ```
 Then, install dependencies with
 ```
 pip install -r requirements.txt 
 python setup.py develop
 ```
 
-The c code shouldn't require anything in most places, but it might ask you to install compilers and stuff. Most of the times you can find the instructions online given the error message
+The C code shouldn't require anything additional setup to get running, but depending on your enviroment, you may be prompted to install compilers and supporting tools. If errors are generating during installation, it is likely due to missing dependencies / tools required of the C code. In many cases, resulting error messages should be clear enough to determine what is missing and how to install it, but common errors will be collected here as they are encountered.
 
 ## Guidelines
 
-There are a few guidelines when developing in this systems. We have a few notable folders:
+There are a few guidelines when developing in this systems. Some notable folders:
 
-1. `commands` - It's the folder that interacts with the caller. This is where the commands themselves should live. They are not meant to do heavy lifting. They only do wiring, which is mostly parsing the input parameters
-2. `services` - It's where the heavy logic lives. It's mostly organizaed by which command needs them.
-3. `helpers` - This is meant for logic that is probably useful accross different commands. For example, logging helpers, or the logic the searches folders
+1. `commands` - It's the folder that interacts with the caller. This is where the commands themselves should reside. These commands are not meant to do heavy lifting. They only do wiring, which is mostly parsing the input parameters. 
+2. `services` - It's where the heavy logic resides. It's mostly organizaed by which command needs them. Commands should generally be thin wrappers around these services.
+3. `helpers` - This is meant for logic that is useful accross different commands. For example, logging helpers, or the logic the searches folders.
 
 # Releases
 
 The standard way to making a new release is the following:
-1)  Open a PR that increases the version number in setup.py. As a rule of thumb, just add one to the micro version (number most to the right).
+1)  Open a PR that increases the version number in setup.py. As a rule of thumb, just add one to the micro/patch version (e.g., v0.1.6 -> v0.1.7).
 
 2) Get the up-to-date master branch locally and run the `tag.release` command from the Makefile.
 
 `$ make tag.release version=v<VERSION_NUM>`
 
 The version tag must match the regex defined on the Makefile (`tag_regex := ^v([0-9]{1,}\.){2}[0-9]{1,}([-_]\w+)?$`).
 
 >**Note**: \
 >Releases with `test` word in them are created as `draft`. \
->Releases with `beta` work in them are created as `pre-release`.
+>Releases with `beta` word in them are created as `pre-release`.
```

### Comparing `codecov-cli-0.1.7/codecov_cli.egg-info/SOURCES.txt` & `codecov-cli-0.1.8/codecov_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/languages/treesitterjavascript/src/parser.c` & `codecov-cli-0.1.8/languages/treesitterjavascript/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/languages/treesitterjavascript/src/scanner.c` & `codecov-cli-0.1.8/languages/treesitterjavascript/src/scanner.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/languages/treesitterjavascript/src/tree_sitter/parser.h` & `codecov-cli-0.1.8/languages/treesitterjavascript/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/languages/treesitterpython/src/parser.c` & `codecov-cli-0.1.8/languages/treesitterpython/src/parser.c`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/languages/treesitterpython/src/scanner.cc` & `codecov-cli-0.1.8/languages/treesitterpython/src/scanner.cc`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/languages/treesitterpython/src/tree_sitter/parser.h` & `codecov-cli-0.1.8/languages/treesitterpython/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `codecov-cli-0.1.7/setup.py` & `codecov-cli-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="codecov-cli",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
     description="Codecov Command Line Interface",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Codecov",
     author_email="support@codecov.io",
     install_requires=["click", "requests", "PyYAML", "tree_sitter", "httpx"],
```

