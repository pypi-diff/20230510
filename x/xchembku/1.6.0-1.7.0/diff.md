# Comparing `tmp/xchembku-1.6.0.tar.gz` & `tmp/xchembku-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchembku-1.6.0.tar", last modified: Fri May  5 11:38:07 2023, max compression
+gzip compressed data, was "xchembku-1.7.0.tar", last modified: Wed May 10 06:06:25 2023, max compression
```

## Comparing `xchembku-1.6.0.tar` & `xchembku-1.7.0.tar`

### file list

```diff
@@ -1,157 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.072968 xchembku-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 11:37:56.000000 xchembku-1.6.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-05 11:37:56.000000 xchembku-1.6.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-05 11:37:56.000000 xchembku-1.6.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.056967 xchembku-1.6.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-05 11:37:56.000000 xchembku-1.6.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-05 11:37:56.000000 xchembku-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-05 11:37:56.000000 xchembku-1.6.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 11:37:56.000000 xchembku-1.6.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 11:37:56.000000 xchembku-1.6.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 11:37:56.000000 xchembku-1.6.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 11:37:56.000000 xchembku-1.6.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 11:37:56.000000 xchembku-1.6.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 11:37:56.000000 xchembku-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-05 11:38:07.072968 xchembku-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-05 11:37:56.000000 xchembku-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-05 11:37:56.000000 xchembku-1.6.0/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/explanations/25-docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 11:37:56.000000 xchembku-1.6.0/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-05 11:37:56.000000 xchembku-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:38:07.072968 xchembku-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.060967 xchembku-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/src/xchembku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 11:38:07.000000 xchembku-1.6.0/src/xchembku.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/src/xchembku_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/aiohttp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/context_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.064967 xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_api/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_api/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_plate_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_plate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_autolocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_droplocation_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_filter_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 11:38:06.000000 xchembku-1.6.0/src/xchembku_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/contexts/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.068968 xchembku-1.6.0/src/xchembku_lib/databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/database_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/normsql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/databases/table_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.072968 xchembku-1.6.0/src/xchembku_lib/datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-05 11:37:56.000000 xchembku-1.6.0/src/xchembku_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.072968 xchembku-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:38:07.072968 xchembku-1.6.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/configurations/direct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_crystal_plate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_crystal_well_autolocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_crystal_well_droplocation1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_crystal_well_droplocation2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_soakdb3_crystal_well.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-05 11:37:56.000000 xchembku-1.6.0/tests/test_swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.822313 xchembku-1.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.794311 xchembku-1.7.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.794311 xchembku-1.7.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-10 06:06:15.000000 xchembku-1.7.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.798311 xchembku-1.7.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-10 06:06:15.000000 xchembku-1.7.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-10 06:06:15.000000 xchembku-1.7.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.798311 xchembku-1.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.782310 xchembku-1.7.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.798311 xchembku-1.7.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.798311 xchembku-1.7.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.802311 xchembku-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-10 06:06:15.000000 xchembku-1.7.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-10 06:06:15.000000 xchembku-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-10 06:06:15.000000 xchembku-1.7.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-10 06:06:15.000000 xchembku-1.7.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.802311 xchembku-1.7.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 06:06:15.000000 xchembku-1.7.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-10 06:06:15.000000 xchembku-1.7.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-10 06:06:15.000000 xchembku-1.7.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-10 06:06:15.000000 xchembku-1.7.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 06:06:15.000000 xchembku-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-10 06:06:25.822313 xchembku-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-10 06:06:15.000000 xchembku-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.802311 xchembku-1.7.0/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-10 06:06:15.000000 xchembku-1.7.0/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.802311 xchembku-1.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.782310 xchembku-1.7.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.802311 xchembku-1.7.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.806311 xchembku-1.7.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.806311 xchembku-1.7.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.806311 xchembku-1.7.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/explanations/25-docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.806311 xchembku-1.7.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.806311 xchembku-1.7.0/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.806311 xchembku-1.7.0/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.810312 xchembku-1.7.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 06:06:15.000000 xchembku-1.7.0/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-10 06:06:15.000000 xchembku-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 06:06:25.826313 xchembku-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.790310 xchembku-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.810312 xchembku-1.7.0/src/xchembku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-05-10 06:06:25.000000 xchembku-1.7.0/src/xchembku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-10 06:06:25.000000 xchembku-1.7.0/src/xchembku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 06:06:25.000000 xchembku-1.7.0/src/xchembku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 06:06:25.000000 xchembku-1.7.0/src/xchembku.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-10 06:06:25.000000 xchembku-1.7.0/src/xchembku.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 06:06:25.000000 xchembku-1.7.0/src/xchembku.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.814312 xchembku-1.7.0/src/xchembku_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/aiohttp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/context_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.814312 xchembku-1.7.0/src/xchembku_api/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/crystal_plate_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/crystal_plate_objects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/crystal_plate_objects/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.814312 xchembku-1.7.0/src/xchembku_api/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.818312 xchembku-1.7.0/src/xchembku_api/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.818312 xchembku-1.7.0/src/xchembku_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/models/crystal_plate_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/models/crystal_plate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/models/crystal_plate_report_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/models/crystal_well_autolocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/models/crystal_well_droplocation_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/models/crystal_well_filter_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/models/crystal_well_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.818312 xchembku-1.7.0/src/xchembku_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.818312 xchembku-1.7.0/src/xchembku_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.818312 xchembku-1.7.0/src/xchembku_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 06:06:25.000000 xchembku-1.7.0/src/xchembku_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.818312 xchembku-1.7.0/src/xchembku_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/contexts/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.818312 xchembku-1.7.0/src/xchembku_lib/crystal_plate_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/crystal_plate_objects/swiss3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.822313 xchembku-1.7.0/src/xchembku_lib/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/databases/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/databases/database_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/databases/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/databases/normsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/databases/table_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.822313 xchembku-1.7.0/src/xchembku_lib/datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/direct_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/direct_crystal_plates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/direct_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-10 06:06:15.000000 xchembku-1.7.0/src/xchembku_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.822313 xchembku-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 06:06:25.822313 xchembku-1.7.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/configurations/direct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/test_crystal_plate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/test_crystal_plate_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6099 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/test_crystal_well_autolocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14750 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/test_crystal_well_droplocation1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/test_crystal_well_droplocation2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/test_soakdb3_crystal_well.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-10 06:06:15.000000 xchembku-1.7.0/tests/test_swiss3.py
```

### Comparing `xchembku-1.6.0/.dae-devops/Makefile` & `xchembku-1.7.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.dae-devops/docs/conventions.rst` & `xchembku-1.7.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.dae-devops/docs/developing.rst` & `xchembku-1.7.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.dae-devops/docs/devops.rst` & `xchembku-1.7.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.dae-devops/docs/docs_structure.rst` & `xchembku-1.7.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.dae-devops/docs/installing.rst` & `xchembku-1.7.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.dae-devops/docs/testing.rst` & `xchembku-1.7.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.dae-devops/project.yaml` & `xchembku-1.7.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.devcontainer/Dockerfile` & `xchembku-1.7.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.devcontainer/devcontainer.json` & `xchembku-1.7.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.github/CONTRIBUTING.rst` & `xchembku-1.7.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.github/actions/install_requirements/action.yml` & `xchembku-1.7.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.github/dependabot.yml` & `xchembku-1.7.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.github/pages/make_switcher.py` & `xchembku-1.7.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.github/workflows/code.yml` & `xchembku-1.7.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.github/workflows/docs.yml` & `xchembku-1.7.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.github/workflows/docs_clean.yml` & `xchembku-1.7.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.github/workflows/linkcheck.yml` & `xchembku-1.7.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.gitignore` & `xchembku-1.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.gitlab-ci.yml` & `xchembku-1.7.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/.vscode/launch.json` & `xchembku-1.7.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/LICENSE` & `xchembku-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/PKG-INFO` & `xchembku-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.6.0
+Version: 1.7.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.6.0/README.rst` & `xchembku-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/configurations/development.yaml` & `xchembku-1.7.0/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/docs/conf.py` & `xchembku-1.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/docs/images/dls-favicon.ico` & `xchembku-1.7.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/docs/images/dls-logo.svg` & `xchembku-1.7.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/docs/index.rst` & `xchembku-1.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/docs/user/explanations/25-docs-structure.rst` & `xchembku-1.7.0/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/docs/user/index.rst` & `xchembku-1.7.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/pyproject.toml` & `xchembku-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku.egg-info/PKG-INFO` & `xchembku-1.7.0/src/xchembku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchembku
-Version: 1.6.0
+Version: 1.7.0
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `xchembku-1.6.0/src/xchembku.egg-info/SOURCES.txt` & `xchembku-1.7.0/src/xchembku.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 src/xchembku_api/datafaces/__init__.py
 src/xchembku_api/datafaces/aiohttp.py
 src/xchembku_api/datafaces/constants.py
 src/xchembku_api/datafaces/context.py
 src/xchembku_api/datafaces/datafaces.py
 src/xchembku_api/models/crystal_plate_filter_model.py
 src/xchembku_api/models/crystal_plate_model.py
+src/xchembku_api/models/crystal_plate_report_model.py
 src/xchembku_api/models/crystal_well_autolocation_model.py
 src/xchembku_api/models/crystal_well_droplocation_model.py
 src/xchembku_api/models/crystal_well_filter_model.py
 src/xchembku_api/models/crystal_well_model.py
 src/xchembku_api/models/crystal_well_needing_droplocation_model.py
 src/xchembku_cli/__init__.py
 src/xchembku_cli/main.py
@@ -105,14 +106,15 @@
 src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py
 src/xchembku_lib/datafaces/direct_crystal_wells.py
 src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py
 tests/__init__.py
 tests/base.py
 tests/conftest.py
 tests/test_crystal_plate.py
+tests/test_crystal_plate_report.py
 tests/test_crystal_well_autolocation.py
 tests/test_crystal_well_droplocation1.py
 tests/test_crystal_well_droplocation2.py
 tests/test_soakdb3_crystal_well.py
 tests/test_swiss3.py
 tests/configurations/direct.yaml
 tests/configurations/service.yaml
```

### Comparing `xchembku-1.6.0/src/xchembku_api/context_base.py` & `xchembku-1.7.0/src/xchembku_api/context_base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/constants.py` & `xchembku-1.7.0/src/xchembku_api/crystal_plate_objects/constants.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_api/crystal_plate_objects/interface.py` & `xchembku-1.7.0/src/xchembku_api/crystal_plate_objects/interface.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_api/datafaces/aiohttp.py` & `xchembku-1.7.0/src/xchembku_api/datafaces/aiohttp.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Class for an aiohttp client.
 from xchembku_api.aiohttp_client import AiohttpClient
 
 # Dataface protocolj things.
 from xchembku_api.datafaces.constants import Commands, Keywords
 from xchembku_api.models.crystal_plate_filter_model import CrystalPlateFilterModel
 from xchembku_api.models.crystal_plate_model import CrystalPlateModel
+from xchembku_api.models.crystal_plate_report_model import CrystalPlateReportModel
 from xchembku_api.models.crystal_well_autolocation_model import (
     CrystalWellAutolocationModel,
 )
 from xchembku_api.models.crystal_well_droplocation_model import (
     CrystalWellDroplocationModel,
 )
 from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
@@ -114,14 +115,33 @@
 
         # Dicts are returned, so parse them into models.
         models = [CrystalPlateModel(**record) for record in records]
 
         return models
 
     # ----------------------------------------------------------------------------------------
+    async def report_crystal_plates(
+        self,
+        filter: CrystalPlateFilterModel,
+        why: Optional[str] = None,
+    ) -> List[CrystalPlateReportModel]:
+        """"""
+
+        records = await self.__send_protocolj(
+            "report_crystal_plates_serialized",
+            filter=filter.dict(),
+            why=why,
+        )
+
+        # Dicts are returned, so parse them into models.
+        models = [CrystalPlateReportModel(**record) for record in records]
+
+        return models
+
+    # ----------------------------------------------------------------------------------------
     async def fetch_crystal_wells_filenames(
         self,
         limit: int = 1,
         why: Optional[str] = None,
     ) -> List[CrystalWellModel]:
         """"""
 
@@ -312,23 +332,23 @@
 
         if self.__aiohttp_client is not None:
             await self.__aiohttp_client.open_client_session()
 
     # ----------------------------------------------------------------------------------------
     async def close_client_session(self):
         """"""
-        logger.debug(f"[ECHDON] {callsign(self)} in aexit")
+        logger.debug(f"[DISSHU] {callsign(self)} in aexit")
 
         if self.__aiohttp_client is not None:
             logger.debug(
-                f"[ECHDON] {callsign(self)} calling __aiohttp_client.close_client_session"
+                f"[DISSHU] {callsign(self)} calling __aiohttp_client.close_client_session"
             )
             await self.__aiohttp_client.close_client_session()
             logger.debug(
-                f"[ECHDON] {callsign(self)} called __aiohttp_client.close_client_session"
+                f"[DISSHU] {callsign(self)} called __aiohttp_client.close_client_session"
             )
 
     # ----------------------------------------------------------------------------------------
     async def client_report_health(self):
         """"""
 
         return await self.__aiohttp_client.client_report_health()
```

### Comparing `xchembku-1.6.0/src/xchembku_api/datafaces/context.py` & `xchembku-1.7.0/src/xchembku_api/datafaces/context.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 
         # Open client session to the service or direct connection.
         await self.interface.open_client_session()
 
     # ----------------------------------------------------------------------------------------
     async def aexit(self):
         """ """
-        logger.debug(f"[ECHDON] {callsign(self)} in aexit")
+        logger.debug(f"[DISSHU] {callsign(self)} in aexit")
 
         if self.interface is not None:
             logger.debug(
-                f"[ECHDON] {callsign(self)} calling close_client_session on {callsign(self.interface)}"
+                f"[DISSHU] {callsign(self)} calling close_client_session on {callsign(self.interface)}"
             )
             # Close client session to the service or direct connection.
             await self.interface.close_client_session()
-            logger.debug(f"[ECHDON] {callsign(self)} called close_client_session")
+            logger.debug(f"[DISSHU] {callsign(self)} called close_client_session")
 
             # Clear the global variable.  Important between pytests.
             xchembku_datafaces_set_default(None)
```

### Comparing `xchembku-1.6.0/src/xchembku_api/datafaces/datafaces.py` & `xchembku-1.7.0/src/xchembku_api/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_api/exceptions.py` & `xchembku-1.7.0/src/xchembku_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_api/models/crystal_plate_model.py` & `xchembku-1.7.0/src/xchembku_api/models/crystal_plate_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
     Typically this structure is populated and transmitted by the rockminer package.
     """
 
     uuid: str
     # ID from the Plate table.
     formulatrix__plate__id: int
+    # Name from the formulatrix "experiment" tree node.
+    formulatrix__experiment__name: Optional[str]
     # Directory stem where wells were mined from.
     # Also used by echolocator to format the export csv filename.
     rockminer_collected_stem: Optional[str] = None
     # The 4-letter barcode.
     barcode: str
     # The visit gleaned from the Formulatrix database.
     visit: str
```

### Comparing `xchembku-1.6.0/src/xchembku_api/models/crystal_well_autolocation_model.py` & `xchembku-1.7.0/src/xchembku_api/models/crystal_well_autolocation_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_api/models/crystal_well_droplocation_model.py` & `xchembku-1.7.0/src/xchembku_api/models/crystal_well_droplocation_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     crystal_well_uuid: Optional[str] = None
     confirmed_target_x: Optional[int] = None
     confirmed_target_y: Optional[int] = None
     confirmed_microns_x: Optional[int] = None
     confirmed_microns_y: Optional[int] = None
     is_usable: Optional[bool] = None
 
+    # True when exported to soakdb3.
+    is_exported_to_soakdb3: Optional[bool] = None
+
     # TODO: Add proper pydantic date parsing/valiation to CREATED_ON fields.
     created_on: Optional[str] = None
 
     def __init__(self, **kwargs):
         # Automatically cook up a uuid if it's not provided to the constructor.
         if "uuid" not in kwargs:
             kwargs["uuid"] = str(uuid.uuid4())
```

### Comparing `xchembku-1.6.0/src/xchembku_api/models/crystal_well_filter_model.py` & `xchembku-1.7.0/src/xchembku_api/models/crystal_well_filter_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,7 +19,8 @@
     barcode: Optional[str] = None
     anchor: Optional[str] = None
     limit: Optional[int] = None
     sortby: Optional[CrystalWellFilterSortbyEnum] = None
     direction: Optional[int] = None
     is_decided: Optional[bool] = None
     is_usable: Optional[bool] = None
+    is_exported_to_soakdb3: Optional[bool] = None
```

### Comparing `xchembku-1.6.0/src/xchembku_api/models/crystal_well_model.py` & `xchembku-1.7.0/src/xchembku_api/models/crystal_well_model.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py` & `xchembku-1.7.0/src/xchembku_api/models/crystal_well_needing_droplocation_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,7 +36,8 @@
     crystal_well_droplocation_uuid: Optional[str] = None
     confirmed_target_x: Optional[int] = None
     confirmed_target_y: Optional[int] = None
     confirmed_microns_x: Optional[int] = None
     confirmed_microns_y: Optional[int] = None
 
     is_usable: Optional[bool] = None
+    is_exported_to_soakdb3: Optional[bool] = None
```

### Comparing `xchembku-1.6.0/src/xchembku_cli/main.py` & `xchembku-1.7.0/src/xchembku_cli/main.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_cli/subcommands/base.py` & `xchembku-1.7.0/src/xchembku_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_cli/subcommands/service.py` & `xchembku-1.7.0/src/xchembku_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_cli/version.py` & `xchembku-1.7.0/src/xchembku_cli/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/__main__.py` & `xchembku-1.7.0/src/xchembku_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/contexts/base.py` & `xchembku-1.7.0/src/xchembku_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py` & `xchembku-1.7.0/src/xchembku_lib/crystal_plate_objects/crystal_plate_objects.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/crystal_plate_objects/swiss3.py` & `xchembku-1.7.0/src/xchembku_lib/crystal_plate_objects/swiss3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 import re
 from typing import Dict, Optional, Tuple
 
 # Base class for generic things.
-from dls_utilpack.describe import describe
 from dls_utilpack.thing import Thing
 
 # Types.
 from xchembku_api.crystal_plate_objects.constants import ThingTypes
 
 # Interface.
 from xchembku_api.crystal_plate_objects.interface import Interface
@@ -61,15 +60,14 @@
 
     # ----------------------------------------------------------------------------------------
     def compute_drop_location_microns(
         self,
         crystal_well_record: Dict,
     ) -> Tuple[Optional[int], Optional[int]]:
 
-        logger.debug(describe("crystal_well_record", crystal_well_record))
         if crystal_well_record.get("confirmed_target_x") is None:
             return (None, None)
         if crystal_well_record.get("confirmed_target_y") is None:
             return (None, None)
 
         x = int(
             0.5
```

### Comparing `xchembku-1.6.0/src/xchembku_lib/databases/databases.py` & `xchembku-1.7.0/src/xchembku_lib/databases/databases.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/databases/normsql.py` & `xchembku-1.7.0/src/xchembku_lib/databases/normsql.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/databases/table_definitions.py` & `xchembku-1.7.0/src/xchembku_lib/databases/table_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
                 elif field_type == bool:
                     sql_type = "BOOLEAN"
 
                 self.fields[field_name] = {"type": sql_type}
 
         # Add indexes.
         self.fields["formulatrix__plate__id"]["index"] = True
+        self.fields["formulatrix__experiment__name"]["index"] = True
         self.fields["barcode"]["index"] = True
         self.fields["visit"]["index"] = True
         self.fields["thing_type"]["index"] = True
         self.fields[CommonFieldnames.CREATED_ON]["index"] = True
 
 
 # ----------------------------------------------------------------------------------------
@@ -169,8 +170,9 @@
                     sql_type = "BOOLEAN"
 
                 self.fields[field_name] = {"type": sql_type}
 
         # Add indexes.
         self.fields["crystal_well_uuid"]["index"] = True
         self.fields["is_usable"]["index"] = True
+        self.fields["is_exported_to_soakdb3"]["index"] = True
         self.fields[CommonFieldnames.CREATED_ON]["index"] = True
```

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/aiohttp.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/context.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/context.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/datafaces.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/datafaces.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/direct.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/direct.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_base.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/direct_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,25 @@
         Thing.__init__(self, thing_type, specification)
 
         self.__database = None
 
     # ----------------------------------------------------------------------------------------
     async def start(self):
         # Connect to the database to create the schemas if they don't exist already.
-        # TODO: Consider if direct dataface needs a start method.
         await self.establish_database_connection()
 
+        # Make sure we are up to date with the latest database schema revision.
+        await self.__database.apply_revisions()
+
     # ----------------------------------------------------------------------------------------
     async def disconnect(self):
         if self.__database is not None:
-            logger.debug(f"{callsign(self)} disconnecting")
+            logger.debug(f"[DISSHU] {callsign(self)} disconnecting")
             await self.__database.disconnect()
-            logger.debug(f"{callsign(self)} disconnected")
+            logger.debug(f"[DISSHU] {callsign(self)} disconnected")
             self.__database = None
 
         # TODO: Figure out a better way to disconnect the dataface mixins.
         await self.disconnect_soakdb3_crystal_wells_mixin()
 
     # ----------------------------------------------------------------------------------------
     async def establish_database_connection(self):
@@ -124,12 +126,12 @@
         """"""
         # Connect to the database to create the schemas if they don't exist already.
         await self.establish_database_connection()
 
     # ----------------------------------------------------------------------------------------
     async def close_client_session(self):
         """"""
-        logger.debug(f"[ECHDON] {callsign(self)} in aexit, calling disconnect")
+        logger.debug(f"[DISSHU] {callsign(self)} in aexit, calling disconnect")
 
         await self.disconnect()
 
-        logger.debug(f"[ECHDON] {callsign(self)} in aexit, disconnected")
+        logger.debug(f"[DISSHU] {callsign(self)} in aexit, disconnected")
```

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/direct_crystal_well_autolocations.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/direct_crystal_well_droplocations.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         from xchembku_api.models.crystal_well_filter_model import CrystalWellFilterModel
 
         filter = CrystalWellFilterModel(anchor=model_dict["crystal_well_uuid"])
 
         # Get the well record.
         crystal_well_models = await self.fetch_crystal_wells_needing_droplocation(
             filter,
-            why=f"(crystal well for) {why}",
+            why=f"(crystal well for adding confirmed microns) {why}",
         )
 
         if len(crystal_well_models) == 0:
             raise RuntimeError(
                 "database integrity error: no crystal well for droplocation upsert"
             )
         crystal_well_model = crystal_well_models[0]
@@ -128,15 +128,17 @@
                         for field in list(model_dict.keys()):
                             if field not in only_fields:
                                 model_dict.pop(field)
 
                     # Convert confirmed target to microns and store in the dict.
                     await self.__add_confirmed_microns(model_dict, why=why)
 
-                    model_dict.pop("crystal_well_uuid")
+                    # Don't update the crystal_well_uuid since it is used as the key.
+                    if "crystal_well_uuid" in model_dict:
+                        model_dict.pop("crystal_well_uuid")
 
                     result = await self.update(
                         "crystal_well_droplocations",
                         model_dict,
                         "(crystal_well_uuid = ?)",
                         subs=[model.crystal_well_uuid],
                         why=why,
```

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_crystal_wells.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/direct_crystal_wells.py`

 * *Files 7% similar despite different names*

```diff
@@ -395,21 +395,46 @@
             sql += (
                 f"\n/* Include only crystal wells which have filter.is_usable = {filter.is_usable}. */"
                 f"\n{where} crystal_well_droplocations.is_usable = ?"
             )
             subs.append(filter.is_usable)
             where = "AND"
 
+        # Caller wants only those which are exported to soakdb3?
+        if filter.is_exported_to_soakdb3 is not None:
+            sql += (
+                f"\n/* Include only crystal wells which have been exported to soakdb3. */"
+                f"\n{where} crystal_well_droplocations.is_usable = True"
+            )
+            where = "AND"
+
         # Caller wants just the anchor record?
         if filter.anchor is not None and filter.direction is None:
             sql += (
                 "\n/* Get the crystal well at the anchor. */"
                 f"\n{where} crystal_wells.uuid = ?"
             )
             subs.append(filter.anchor)
+            where = "AND"
+
+        # Caller wants those in direction from the anchor record?
+        # This means we ne need the anchor to be in the rows,
+        # no matter if it would have been excluded by other filters.
+        if filter.anchor is not None and filter.direction is not None:
+            # We presume that all previous conjunctions were AND
+            # which have higher operator precedence than OR,
+            # so we can stick an OR on here at the end
+            if where == "AND":
+                where = "OR"
+            sql += (
+                "\n/* Always include the crystal well at the anchor. */"
+                f"\n{where} crystal_wells.uuid = ?"
+            )
+            subs.append(filter.anchor)
+            where = "AND"
 
         return sql
 
     # ----------------------------------------------------------------------------------------
     def __build_orderby(
         self,
         filter: CrystalWellFilterModel,
```

### Comparing `xchembku-1.6.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py` & `xchembku-1.7.0/src/xchembku_lib/datafaces/direct_soakdb3_crystal_wells.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/src/xchembku_lib/version.py` & `xchembku-1.7.0/src/xchembku_lib/version.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/tests/base.py` & `xchembku-1.7.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/tests/configurations/direct.yaml` & `xchembku-1.7.0/tests/configurations/direct.yaml`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/tests/configurations/service.yaml` & `xchembku-1.7.0/tests/configurations/service.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     # Format to make actual data_filename using data_label as token.
     data_path_pattern: "/dls/b29/data/2022/cy29757-3/Merlin/{data_label}_data.mib"
 
 logging_settings:
     console:
         enabled: True
         verbose: True
+        filters:
+            markers:
+                - "[DISSHU]"
     logfile:
         enabled: True
         directory: ${output_directory}/logfile.log
     graypy:
         enabled: False
         host: 172.23.7.128
         port: 12201
```

### Comparing `xchembku-1.6.0/tests/test_crystal_plate.py` & `xchembku-1.7.0/tests/test_crystal_plate.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/tests/test_crystal_well_autolocation.py` & `xchembku-1.7.0/tests/test_crystal_well_autolocation.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/tests/test_crystal_well_droplocation1.py` & `xchembku-1.7.0/tests/test_crystal_well_droplocation1.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/tests/test_crystal_well_droplocation2.py` & `xchembku-1.7.0/tests/test_crystal_well_droplocation2.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,15 @@
             CrystalWellFilterModel(
                 # Anchor at #2.
                 anchor=models[1].uuid,
                 visit=self.__visit,
                 sortby=CrystalWellFilterSortbyEnum.NUMBER_OF_CRYSTALS,
                 direction=1,
                 limit=1,
+                is_usable=True,
             ),
             [5],
             "anchored, forward",
         )
 
         await self.__check(
             dataface,
@@ -226,14 +227,15 @@
             CrystalWellFilterModel(
                 # Anchor at #2.
                 anchor=models[1].uuid,
                 visit=self.__visit,
                 sortby=CrystalWellFilterSortbyEnum.NUMBER_OF_CRYSTALS,
                 direction=-1,
                 limit=10,
+                is_usable=True,
             ),
             [4, 3],
             "anchored, reverse, all",
         )
 
     # ----------------------------------------------------------------------------------------
```

### Comparing `xchembku-1.6.0/tests/test_soakdb3_crystal_well.py` & `xchembku-1.7.0/tests/test_soakdb3_crystal_well.py`

 * *Files identical despite different names*

### Comparing `xchembku-1.6.0/tests/test_swiss3.py` & `xchembku-1.7.0/tests/test_swiss3.py`

 * *Files identical despite different names*

