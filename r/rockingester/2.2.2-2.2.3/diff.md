# Comparing `tmp/rockingester-2.2.2.tar.gz` & `tmp/rockingester-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockingester-2.2.2.tar", last modified: Fri May  5 11:39:18 2023, max compression
+gzip compressed data, was "rockingester-2.2.3.tar", last modified: Wed May 10 15:50:11 2023, max compression
```

## Comparing `rockingester-2.2.2.tar` & `rockingester-2.2.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.218304 rockingester-2.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.198303 rockingester-2.2.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.198303 rockingester-2.2.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-05 11:39:04.000000 rockingester-2.2.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.198303 rockingester-2.2.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-05 11:39:04.000000 rockingester-2.2.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-05 11:39:04.000000 rockingester-2.2.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.198303 rockingester-2.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.190303 rockingester-2.2.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.198303 rockingester-2.2.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.198303 rockingester-2.2.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.202303 rockingester-2.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-05 11:39:04.000000 rockingester-2.2.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-05 11:39:04.000000 rockingester-2.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-05 11:39:04.000000 rockingester-2.2.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 11:39:04.000000 rockingester-2.2.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.202303 rockingester-2.2.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 11:39:04.000000 rockingester-2.2.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-05 11:39:04.000000 rockingester-2.2.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 11:39:04.000000 rockingester-2.2.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-05 11:39:04.000000 rockingester-2.2.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 11:39:04.000000 rockingester-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-05 11:39:18.218304 rockingester-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-05 11:39:04.000000 rockingester-2.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.202303 rockingester-2.2.2/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-05 11:39:04.000000 rockingester-2.2.2/configurations/development.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.202303 rockingester-2.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.190303 rockingester-2.2.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.202303 rockingester-2.2.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.202303 rockingester-2.2.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.202303 rockingester-2.2.2/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.206303 rockingester-2.2.2/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/explanations/22-developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/explanations/23-testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/explanations/24-devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/explanations/25-docs-structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/explanations/51-todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.206303 rockingester-2.2.2/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/how-to/01-installing_development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.206303 rockingester-2.2.2/docs/user/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.206303 rockingester-2.2.2/docs/user/reference/api/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/reference/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/reference/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/reference/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.206303 rockingester-2.2.2/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 11:39:04.000000 rockingester-2.2.2/docs/user/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-05 11:39:04.000000 rockingester-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:39:18.218304 rockingester-2.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.194303 rockingester-2.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.206303 rockingester-2.2.2/src/rockingester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-05 11:39:18.000000 rockingester-2.2.2/src/rockingester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-05 11:39:18.000000 rockingester-2.2.2/src/rockingester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:39:18.000000 rockingester-2.2.2/src/rockingester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 11:39:18.000000 rockingester-2.2.2/src/rockingester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 11:39:18.000000 rockingester-2.2.2/src/rockingester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 11:39:18.000000 rockingester-2.2.2/src/rockingester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.210303 rockingester-2.2.2/src/rockingester_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.210303 rockingester-2.2.2/src/rockingester_api/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.210303 rockingester-2.2.2/src/rockingester_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.210303 rockingester-2.2.2/src/rockingester_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_cli/subcommands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.214303 rockingester-2.2.2/src/rockingester_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 11:39:18.000000 rockingester-2.2.2/src/rockingester_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.214303 rockingester-2.2.2/src/rockingester_lib/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/collectors/collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/collectors/direct_poll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.214303 rockingester-2.2.2/src/rockingester_lib/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-05 11:39:04.000000 rockingester-2.2.2/src/rockingester_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.214303 rockingester-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:04.000000 rockingester-2.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-05 11:39:04.000000 rockingester-2.2.2/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:39:18.214303 rockingester-2.2.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-05 11:39:04.000000 rockingester-2.2.2/tests/configurations/direct_poll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-05 11:39:04.000000 rockingester-2.2.2/tests/configurations/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-05 11:39:04.000000 rockingester-2.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-05 11:39:04.000000 rockingester-2.2.2/tests/test_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.588741 rockingester-2.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-10 15:49:50.000000 rockingester-2.2.3/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-10 15:49:50.000000 rockingester-2.2.3/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 15:49:50.000000 rockingester-2.2.3/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.572741 rockingester-2.2.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-10 15:49:50.000000 rockingester-2.2.3/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-10 15:49:50.000000 rockingester-2.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-10 15:49:50.000000 rockingester-2.2.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-10 15:49:50.000000 rockingester-2.2.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.576741 rockingester-2.2.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 15:49:50.000000 rockingester-2.2.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-10 15:49:50.000000 rockingester-2.2.3/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-10 15:49:50.000000 rockingester-2.2.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-10 15:49:50.000000 rockingester-2.2.3/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 15:49:50.000000 rockingester-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-10 15:50:11.588741 rockingester-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-10 15:49:50.000000 rockingester-2.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-10 15:49:50.000000 rockingester-2.2.3/configurations/development.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.572741 rockingester-2.2.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/22-developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/23-testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/24-devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/25-docs-structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/explanations/51-todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/how-to/01-installing_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/reference/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/reference/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/reference/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/reference/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 15:49:50.000000 rockingester-2.2.3/docs/user/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-10 15:49:50.000000 rockingester-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:50:11.588741 rockingester-2.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.572741 rockingester-2.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/src/rockingester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16864 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.580741 rockingester-2.2.3/src/rockingester_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_api/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/subcommands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 15:50:11.000000 rockingester-2.2.3/src/rockingester_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_lib/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/collectors/direct_poll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/src/rockingester_lib/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 15:49:50.000000 rockingester-2.2.3/src/rockingester_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:50:11.584741 rockingester-2.2.3/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/configurations/direct_poll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/configurations/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-10 15:49:50.000000 rockingester-2.2.3/tests/test_collector.py
```

### Comparing `rockingester-2.2.2/.dae-devops/Makefile` & `rockingester-2.2.3/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.dae-devops/docs/conventions.rst` & `rockingester-2.2.3/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.dae-devops/docs/developing.rst` & `rockingester-2.2.3/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.dae-devops/docs/devops.rst` & `rockingester-2.2.3/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.dae-devops/docs/docs_structure.rst` & `rockingester-2.2.3/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.dae-devops/docs/installing.rst` & `rockingester-2.2.3/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.dae-devops/docs/testing.rst` & `rockingester-2.2.3/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.dae-devops/project.yaml` & `rockingester-2.2.3/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.devcontainer/Dockerfile` & `rockingester-2.2.3/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.devcontainer/devcontainer.json` & `rockingester-2.2.3/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.github/CONTRIBUTING.rst` & `rockingester-2.2.3/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.github/actions/install_requirements/action.yml` & `rockingester-2.2.3/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.github/dependabot.yml` & `rockingester-2.2.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.github/pages/make_switcher.py` & `rockingester-2.2.3/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.github/workflows/code.yml` & `rockingester-2.2.3/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.github/workflows/docs.yml` & `rockingester-2.2.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.github/workflows/docs_clean.yml` & `rockingester-2.2.3/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.github/workflows/linkcheck.yml` & `rockingester-2.2.3/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.gitignore` & `rockingester-2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.gitlab-ci.yml` & `rockingester-2.2.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/.vscode/launch.json` & `rockingester-2.2.3/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/LICENSE` & `rockingester-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/PKG-INFO` & `rockingester-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.2.2
+Version: 2.2.3
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.2.2/README.rst` & `rockingester-2.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/configurations/development.yaml` & `rockingester-2.2.3/configurations/development.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/docs/conf.py` & `rockingester-2.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/docs/images/dls-favicon.ico` & `rockingester-2.2.3/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/docs/images/dls-logo.svg` & `rockingester-2.2.3/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/docs/index.rst` & `rockingester-2.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/docs/user/explanations/25-docs-structure.rst` & `rockingester-2.2.3/docs/user/explanations/25-docs-structure.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/docs/user/index.rst` & `rockingester-2.2.3/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/pyproject.toml` & `rockingester-2.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester.egg-info/PKG-INFO` & `rockingester-2.2.3/src/rockingester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockingester
-Version: 2.2.2
+Version: 2.2.3
 Summary: XChem Business Knowledge Unit. Service, Client, API, persistent store.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rockingester-2.2.2/src/rockingester.egg-info/SOURCES.txt` & `rockingester-2.2.3/src/rockingester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_api/collectors/aiohttp.py` & `rockingester-2.2.3/src/rockingester_api/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_api/collectors/collectors.py` & `rockingester-2.2.3/src/rockingester_api/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_api/collectors/context.py` & `rockingester-2.2.3/src/rockingester_api/collectors/context.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_api/context_base.py` & `rockingester-2.2.3/src/rockingester_api/context_base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_api/exceptions.py` & `rockingester-2.2.3/src/rockingester_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_api/thing.py` & `rockingester-2.2.3/src/rockingester_api/thing.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_api/things.py` & `rockingester-2.2.3/src/rockingester_api/things.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_cli/main.py` & `rockingester-2.2.3/src/rockingester_cli/main.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_cli/subcommands/base.py` & `rockingester-2.2.3/src/rockingester_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_cli/subcommands/service.py` & `rockingester-2.2.3/src/rockingester_cli/subcommands/service.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_cli/version.py` & `rockingester-2.2.3/src/rockingester_cli/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_lib/__main__.py` & `rockingester-2.2.3/src/rockingester_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_lib/collectors/aiohttp.py` & `rockingester-2.2.3/src/rockingester_lib/collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_lib/collectors/base.py` & `rockingester-2.2.3/src/rockingester_lib/collectors/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_lib/collectors/collectors.py` & `rockingester-2.2.3/src/rockingester_lib/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_lib/collectors/context.py` & `rockingester-2.2.3/src/rockingester_lib/collectors/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,20 +71,18 @@
 
         Stop service if one was started and releases any client resources.
         """
 
         if self.server is not None:
             if self.context_specification.get("start_as") == "process":
                 logger.info(
-                    "[NEWSHUT] in context exit, sending shutdown to client process"
+                    "[DISSHU] in context exit, sending shutdown to client process"
                 )
                 # Put in request to shutdown the server.
                 await self.server.client_shutdown()
-                logger.info(
-                    "[NEWSHUT] in context exit, sent shutdown to client process"
-                )
+                logger.info("[DISSHU] in context exit, sent shutdown to client process")
 
             if self.context_specification.get("start_as") == "coro":
                 await self.server.direct_shutdown()
 
             if self.context_specification.get("start_as") == "direct":
                 await self.server.deactivate()
```

### Comparing `rockingester-2.2.2/src/rockingester_lib/collectors/direct_poll.py` & `rockingester-2.2.3/src/rockingester_lib/collectors/direct_poll.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_lib/contexts/base.py` & `rockingester-2.2.3/src/rockingester_lib/contexts/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_lib/exceptions.py` & `rockingester-2.2.3/src/rockingester_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/src/rockingester_lib/version.py` & `rockingester-2.2.3/src/rockingester_lib/version.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/tests/base.py` & `rockingester-2.2.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/tests/configurations/direct_poll.yaml` & `rockingester-2.2.3/tests/configurations/direct_poll.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/tests/configurations/service.yaml` & `rockingester-2.2.3/tests/configurations/service.yaml`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/tests/conftest.py` & `rockingester-2.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rockingester-2.2.2/tests/test_collector.py` & `rockingester-2.2.3/tests/test_collector.py`

 * *Files identical despite different names*

