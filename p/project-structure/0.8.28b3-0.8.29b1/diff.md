# Comparing `tmp/project-structure-0.8.28b3.tar.gz` & `tmp/project-structure-0.8.29b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-structure-0.8.28b3.tar", last modified: Mon May  8 18:13:02 2023, max compression
+gzip compressed data, was "project-structure-0.8.29b1.tar", last modified: Wed May 10 09:10:40 2023, max compression
```

## Comparing `project-structure-0.8.28b3.tar` & `project-structure-0.8.29b1.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      821 2023-05-08 18:03:37.000000 project-structure-0.8.28b3/.cz.toml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      643 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.dir-locals.el.in
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1717 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.dockerignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1064 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.env.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.831143 project-structure-0.8.28b3/.github/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/.github/workflows/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4573 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.github/workflows/build-test.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1717 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     6288 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.gitlab-ci.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      877 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.pre-commit-config.yaml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2472 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.prospector.yaml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/.reuse/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      790 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.reuse/dep5
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/.tox/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5411 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/CONTRIBUTING.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4838 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/Dockerfile
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/LICENSES/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1071 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/LICENSES/MIT.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    59879 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/Makefile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      140 2023-05-08 18:03:35.000000 project-structure-0.8.28b3/NEWS-VERSION.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    13718 2023-05-08 18:03:37.000000 project-structure-0.8.28b3/NEWS.rst
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17800 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/PKG-INFO
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    16758 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/README.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4388 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/TODO.rst
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/bin/
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2860 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/cz-check-bump
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1052 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/entrypoint
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1202 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/get-base-version
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)      422 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/hadolint
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1480 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/bin/host-install
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/build-host/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2151 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/Dockerfile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1584 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/Makefile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      849 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/README.rst
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/build-host/bin/
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2152 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/bin/entrypoint
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      730 2023-05-08 18:12:07.000000 project-structure-0.8.28b3/build-host/requirements-py310.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      673 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements-py311.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      947 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements-py37.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements-py38.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements-py39.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      104 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/build-host/requirements.txt.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/dist/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      222 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/dist/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5277 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/docker-compose.override.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      741 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/docker-compose.yml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/gitlab-runner/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/gitlab-runner/config/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1423 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      666 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/home/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      246 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/home/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      427 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/home/.pypirc.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/newsfragments/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      187 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/newsfragments/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1862 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/pyproject.toml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      679 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/build.txt.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py310/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py310/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4720 2023-05-08 18:12:07.000000 project-structure-0.8.28b3/requirements/py310/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      864 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py310/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      257 2023-05-08 18:12:07.000000 project-structure-0.8.28b3/requirements/py310/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py311/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py311/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4548 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py311/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      749 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py311/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      264 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py311/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py37/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2659 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py37/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5138 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py37/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1072 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py37/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      399 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py37/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py38/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2502 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py38/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4760 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py38/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py38/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py38/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/requirements/py39/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2380 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py39/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4747 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py39/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py39/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/requirements/py39/user.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1660 2023-05-08 18:13:02.839143 project-structure-0.8.28b3/setup.cfg
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.831143 project-structure-0.8.28b3/src/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/src/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/project_structure.egg-info/.gitignore
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17800 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/PKG-INFO
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)     2597 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)        1 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)       60 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/entry_points.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)      151 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/requires.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)       17 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/src/projectstructure/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4356 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/__init__.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      303 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/__main__.py
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/src/projectstructure/tests/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      165 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/tests/__init__.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4457 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/tests/test_cli.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      495 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/src/projectstructure/utils.py
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)      164 2023-05-08 18:13:02.000000 project-structure-0.8.28b3/src/projectstructure/version.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      281 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/towncrier.toml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3579 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/tox.ini
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      229 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py310/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py310/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py310/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py310/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py310/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py310/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py311/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py311/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py311/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py311/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py311/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py311/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py37/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py37/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py37/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py37/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py37/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py37/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py38/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py38/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py38/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py38/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py38/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py38/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py39/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py39/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py39/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py39/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-08 18:13:02.835143 project-structure-0.8.28b3/var-docker/py39/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-08 18:02:29.000000 project-structure-0.8.28b3/var-docker/py39/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      821 2023-05-10 09:05:29.000000 project-structure-0.8.29b1/.cz.toml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      643 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.dir-locals.el.in
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1717 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.dockerignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1418 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.env.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.276727 project-structure-0.8.29b1/.github/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.276727 project-structure-0.8.29b1/.github/workflows/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4646 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/.github/workflows/build-test.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1717 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     6365 2023-05-10 09:04:31.000000 project-structure-0.8.29b1/.gitlab-ci.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      877 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2472 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/.prospector.yaml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.276727 project-structure-0.8.29b1/.reuse/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      790 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.reuse/dep5
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.tox/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5411 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/CONTRIBUTING.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4942 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/Dockerfile
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/LICENSES/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1071 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/LICENSES/MIT.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    60235 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/Makefile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      140 2023-05-10 09:05:27.000000 project-structure-0.8.29b1/NEWS-VERSION.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    14153 2023-05-10 09:05:28.000000 project-structure-0.8.29b1/NEWS.rst
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17800 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/PKG-INFO
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    16758 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/README.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4388 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/TODO.rst
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/bin/
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2860 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/cz-check-bump
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1052 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/entrypoint
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1202 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/get-base-version
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)      422 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/hadolint
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1480 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/host-install
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/build-host/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2264 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/Dockerfile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1584 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/Makefile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      849 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/README.rst
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/build-host/bin/
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2152 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/bin/entrypoint
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      730 2023-05-10 09:05:42.000000 project-structure-0.8.29b1/build-host/requirements-py310.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      673 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements-py311.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      947 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements-py37.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements-py38.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements-py39.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      104 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements.txt.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/dist/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      222 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/dist/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5301 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/docker-compose.override.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      741 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/docker-compose.yml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/gitlab-runner/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/gitlab-runner/config/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1423 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      666 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/home/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      246 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/home/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      427 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/home/.pypirc.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/newsfragments/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      187 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/newsfragments/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1862 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/pyproject.toml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      679 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/build.txt.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py310/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py310/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4720 2023-05-10 09:05:42.000000 project-structure-0.8.29b1/requirements/py310/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      864 2023-05-10 09:07:28.000000 project-structure-0.8.29b1/requirements/py310/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      257 2023-05-10 09:05:42.000000 project-structure-0.8.29b1/requirements/py310/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py311/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py311/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4548 2023-05-10 00:03:59.000000 project-structure-0.8.29b1/requirements/py311/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      749 2023-05-10 00:03:39.000000 project-structure-0.8.29b1/requirements/py311/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      264 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/requirements/py311/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py37/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2659 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py37/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5138 2023-05-10 08:44:47.000000 project-structure-0.8.29b1/requirements/py37/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1072 2023-05-10 08:44:40.000000 project-structure-0.8.29b1/requirements/py37/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      399 2023-05-10 08:44:38.000000 project-structure-0.8.29b1/requirements/py37/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py38/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2502 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py38/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4760 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/requirements/py38/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/requirements/py38/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/requirements/py38/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py39/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2380 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py39/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4747 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/requirements/py39/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/requirements/py39/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/requirements/py39/user.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1660 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/setup.cfg
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.276727 project-structure-0.8.29b1/src/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/src/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/src/project_structure.egg-info/.gitignore
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17800 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)     2597 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)        1 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)       60 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)      151 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/requires.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)       17 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/src/projectstructure/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4356 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/src/projectstructure/__init__.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      303 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/src/projectstructure/__main__.py
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/src/projectstructure/tests/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      165 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/src/projectstructure/tests/__init__.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4457 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/src/projectstructure/tests/test_cli.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      495 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/src/projectstructure/utils.py
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)      164 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/projectstructure/version.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      281 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/towncrier.toml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3652 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/tox.ini
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      229 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py310/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py310/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py310/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py310/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py310/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py310/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py311/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py311/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py311/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py311/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py311/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py311/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py37/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py37/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py37/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py37/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py37/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py37/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py38/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py38/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py38/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py38/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/var-docker/py38/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py38/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/var-docker/py39/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py39/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/var-docker/py39/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py39/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/var-docker/py39/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py39/project_structure.egg-info/.gitignore
```

### Comparing `project-structure-0.8.28b3/.cz.toml` & `project-structure-0.8.29b1/.cz.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 # TEMPLATE: Update these versions to the latest version for your project and ensure the
 # tag exists both locally and on the project's remote:
 changelog_start_rev = "v0.0.0"
-version = "0.8.28b3"
+version = "0.8.29b1"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `project-structure-0.8.28b3/.dir-locals.el.in` & `project-structure-0.8.29b1/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/.dockerignore` & `project-structure-0.8.29b1/.dockerignore`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/.env.in` & `project-structure-0.8.29b1/.env.in`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
 #
 # SPDX-License-Identifier: MIT
 
-# Make non-default `./docker-compose*.yml` files the default
-# https://pscheit.medium.com/docker-compose-advanced-configuration-541356d121de#9aa6
-COMPOSE_PATH_SEPARATOR=:
-COMPOSE_FILE=./docker-compose.yml:./gitlab-runner/docker-compose.yml:./docker-compose.override.yml
-
 # Capture local values specific to this checkout:
 TZ=${TZ}
 PUID=${PUID}
 PGID=${PGID}
-# Absolute path of the git repo checkout, useful where relative paths can't be used:
-CHECKOUT_DIR=${CHECKOUT_DIR}
-# Build host variables:
-DOCKER_GID=${DOCKER_GID}
 
-# Release variables:
-DOCKER_USER=${DOCKER_USER}
+# Release Secrets:
 # Best to create and use a token.  Note that the token must have the `admin`/"Read,
 # Write, Delete" scope, aka "ACCESS PERMISSIONS":
 # https://hub.docker.com/settings/security?generateToken=true
 DOCKER_PASS=${DOCKER_PASS}
-
 # Project host credentials used here and in CI/CD to support local testing/debugging:
 CI_REGISTRY_PASSWORD=${CI_REGISTRY_PASSWORD}
 PROJECT_GITHUB_PAT=${PROJECT_GITHUB_PAT}
+
+# Constants specific to this project and/or checkout used in variable substitutions in
+# `./docker-compose*.yml`.  Should not be modified during the normal course of
+# development:
+# Project specific values:
+PROJECT_NAMESPACE=${PROJECT_NAMESPACE}
+PROJECT_NAME=${PROJECT_NAME}
+# Absolute path of the git repo checkout, useful where relative paths can't be used:
+CHECKOUT_DIR=${CHECKOUT_DIR}
+# The Docker Hub user or organization:
+DOCKER_USER=${DOCKER_USER}
+# Make non-default `./docker-compose*.yml` files the default:
+# https://pscheit.medium.com/docker-compose-advanced-configuration-541356d121de#9aa6
+COMPOSE_PATH_SEPARATOR=:
+COMPOSE_FILE=./docker-compose.yml:./gitlab-runner/docker-compose.yml:./docker-compose.override.yml
+# Build host variables, used only for reproducing CI/CD locally:
+DOCKER_GID=${DOCKER_GID}
```

### Comparing `project-structure-0.8.28b3/.github/workflows/build-test.yml` & `project-structure-0.8.29b1/.github/workflows/build-test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,39 @@
 #   A GitHub "Classic" Personal Access Token with scopes: `repo`, `workflow`,
 #   `packages`, and `project`
 # - `PYPI_PASSWORD`:
 #   A PyPI API token
 # - `TEST_PYPI_PASSWORD`:
 #   A PyPI API token
 
+env:
+  PUID: "1001"
+  PGID: "123"
+  # Project specific values:
+  PROJECT_NAMESPACE: "rpatterson"
+  PROJECT_NAME: "project-structure"
+  # Requires the secrets to be added to GitHub either through the web UI or the
+  # GitHub CLI tool:
+  # https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
+  GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
+  GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
+  DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
+  # Enable the GitHub CLI
+  PROJECT_GITHUB_PAT: "${{ secrets.PROJECT_GITHUB_PAT }}"
+  # Tell the `./Makefile` about GitHub specific environment details:
+  CI_IS_FORK: >-
+    ${{
+      (
+        (
+          (github.repository_owner != '${PROJECT_NAMESPACE}')
+          || (github.event.pull_request.head.repo.owner.login != '${PROJECT_NAMESPACE}')
+        ) && 'true'
+      ) || 'false'
+    }}
+
 on:
   # Only run on branches, not tags:
   # https://github.com/orgs/community/discussions/25615#discussioncomment-3397691
   push:
     branches:
       - "**"
     tags:
@@ -35,35 +60,15 @@
 jobs:
 
   build-test:
     runs-on: "ubuntu-latest"
     container:
       image: "ghcr.io/rpatterson/project-structure:build-host"
       env:
-        PUID: "1001"
-        PGID: "123"
         CHECKOUT_DIR: "${{ github.workspace }}"
-        # Requires the secrets to be added to GitHub either through the web UI or the
-        # GitHub CLI tool:
-        # https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
-        GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
-        GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
-        DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
-        # Enable the GitHub CLI
-        PROJECT_GITHUB_PAT: "${{ secrets.PROJECT_GITHUB_PAT }}"
-        # Tell the `./Makefile` about GitHub specific environment details:
-        CI_IS_FORK: >-
-          ${{
-            (
-              (
-                (github.repository_owner != 'rpatterson')
-                || (github.event.pull_request.head.repo.owner.login != 'rpatterson')
-              ) && 'true'
-            ) || 'false'
-          }}
     permissions:
       packages: "write"
       checks: "write"
     strategy:
       matrix:
         PYTHON_MINORS:
           - "3.10"
@@ -101,16 +106,19 @@
         uses: "dorny/test-reporter@main"
         # run this step even if previous step failed
         if: >-
           (success() || failure())
           && (
             (! github.event.pull_request)
             || ! (
-              (github.repository_owner == 'rpatterson')
-              && (github.event.pull_request.head.repo.owner.login != 'rpatterson')
+              (github.repository_owner == '${PROJECT_NAMESPACE}')
+              && (
+                github.event.pull_request.head.repo.owner.login
+                != '${PROJECT_NAMESPACE}'
+              )
             )
           )
         with:
           name: "Test Suite Reports"
           path: >-
             ./build/*/*test-junit.xml,
             ./build/*/prospector-xunit.xml
```

### Comparing `project-structure-0.8.28b3/.gitignore` & `project-structure-0.8.29b1/.gitignore`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/.gitlab-ci.yml` & `project-structure-0.8.29b1/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -34,32 +34,34 @@
 #   A GitLab Personal or Project Access Token formatted as an HTTP authentication prefix
 #   to the hostname, e.g.:
 #     https://token-name:token-value@gitlab.com/rpatterson/project-structure.git
 #
 # All that can be masked should be.  All should be protected except `CODECOV_TOKEN` and
 # `DOCKER_PASS`.
 
+variables:
+  # Variables controlling behavior:
+  PUID: "1001"
+  PGID: "1001"
+  # Project specific values:
+  PROJECT_NAMESPACE: "rpatterson"
+  # Uncomment to get more debugging output:
+  # DEBUG: "true"
+
 default:
   image:
-    name: "$CI_TEMPLATE_REGISTRY_HOST/rpatterson/$CI_PROJECT_NAME:build-host"
+    name: "$CI_TEMPLATE_REGISTRY_HOST/$PROJECT_NAMESPACE/$CI_PROJECT_NAME:build-host"
     entrypoint:
       - "docker-entrypoint.sh"
   services:
     - "docker:dind"
   before_script:
     - "chown -R $PUID:$PGID ./"
   # TODO: Debug stale venv issues and restore cache once fixed
 
-variables:
-  # Variables controlling behavior:
-  PUID: "1001"
-  PGID: "1001"
-  # Uncomment to get more debugging output:
-  # DEBUG: "true"
-
 stages:
   - "build-test"
   - "release"
   - "release-bump"
   - "release-version"
   - "scheduled"
   - "merge-upgrade"
@@ -130,15 +132,15 @@
         /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9]+[^0-9].+$/
           ) || (
             $CI_COMMIT_BRANCH == "main"
             && $CI_COMMIT_TITLE =~
         /^build\(release\): Version [0-9]+\.[0-9]+\.[0-9]+.* → [0-9]+\.[0-9]+\.[0-9]+$/
           )
         )
-        && $CI_PROJECT_NAMESPACE == "rpatterson"
+        && $CI_PROJECT_NAMESPACE == $PROJECT_NAMESPACE
   script:
     - >-
       entrypoint make -e release-pkgs test-clean
   artifacts:
     paths:
       - "./dist/project?structure-*"
```

### Comparing `project-structure-0.8.28b3/.pre-commit-config.yaml` & `project-structure-0.8.29b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/.prospector.yaml` & `project-structure-0.8.29b1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/.reuse/dep5` & `project-structure-0.8.29b1/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/CONTRIBUTING.rst` & `project-structure-0.8.29b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/Dockerfile` & `project-structure-0.8.29b1/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 
 # Stay as close to a vanilla Python environment as possible
 ARG PYTHON_MINOR=3.10
 FROM python:${PYTHON_MINOR} AS base
 # Defensive shell options:
 SHELL ["/bin/bash", "-eu", "-o", "pipefail", "-c"]
 
+# Project contstants:
+ARG PROJECT_NAMESPACE=rpatterson
+ARG PROJECT_NAME=project-structure
+
 # Least volatile layers first:
 # https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
-LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/project-structure"
-LABEL org.opencontainers.image.documentation="https://gitlab.com/rpatterson/project-structure"
-LABEL org.opencontainers.image.source="https://gitlab.com/rpatterson/project-structure"
+LABEL org.opencontainers.image.url="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECT_NAME}"
+LABEL org.opencontainers.image.documentation="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECpT_NAME}"
+LABEL org.opencontainers.image.source="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECT_NAME}"
 LABEL org.opencontainers.image.title="Project Structure"
 LABEL org.opencontainers.image.description="Project structure foundation or template"
 LABEL org.opencontainers.image.licenses="MIT"
 LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
 LABEL org.opencontainers.image.vendor="rpatterson.net"
 LABEL org.opencontainers.image.base.name="docker.io/library/python:${PYTHON_MINOR}"
 
 # Find the same home directory even when run as another user, e.g. `root`.
-ENV HOME="/home/project-structure"
+ENV HOME="/home/${PROJECT_NAME}"
 ENTRYPOINT [ "entrypoint" ]
 CMD [ "project-structure" ]
 
 # Put the `ENTRYPOINT` on the `$PATH`
 COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
 
 # Install OS packages needed for the image `ENDPOINT`:
@@ -37,15 +41,15 @@
     echo 'Binary::apt::APT::Keep-Downloaded-Packages "true";' \
     >"/etc/apt/apt.conf.d/keep-cache"
 RUN --mount=type=cache,target=/var/cache/apt,sharing=locked \
     --mount=type=cache,target=/var/lib/apt,sharing=locked \
     apt-get update && \
     apt-get install --no-install-recommends -y "gosu=1.12-1+b6"
 
-WORKDIR "/usr/local/src/project-structure/"
+WORKDIR "/usr/local/src/${PROJECT_NAME}/"
 # Install dependencies with fixed versions in a separate layer to optimize build times
 # because this step takes the most time and changes the least frequently.
 ARG PYTHON_ENV=py310
 COPY [ "./requirements/${PYTHON_ENV}/user.txt", "./requirements/${PYTHON_ENV}/" ]
 # hadolint ignore=DL3042
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
     pip3 install -r "./requirements/${PYTHON_ENV}/user.txt"
@@ -59,15 +63,15 @@
 
 # Stay as close to a vanilla environment as possible:
 FROM base AS user
 # Defensive shell options:
 SHELL ["/bin/bash", "-eu", "-o", "pipefail", "-c"]
 
 # Least volatile layers first:
-WORKDIR "/home/project-structure/"
+WORKDIR "/home/${PROJECT_NAME}/"
 
 # Install this package in the most common/standard Python way while still being able to
 # build the image locally.
 ARG PYTHON_WHEEL
 COPY [ "${PYTHON_WHEEL}", "${PYTHON_WHEEL}" ]
 # hadolint ignore=DL3013,DL3042
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
@@ -83,33 +87,33 @@
 SHELL ["/bin/bash", "-eu", "-o", "pipefail", "-c"]
 
 # Least volatile layers first:
 LABEL org.opencontainers.image.title="Project Structure Development"
 LABEL org.opencontainers.image.description="Project structure foundation or template, development image"
 
 # Activate the Python virtual environment
-ENV VIRTUAL_ENV="/usr/local/src/project-structure/.tox/${PYTHON_ENV}"
+ENV VIRTUAL_ENV="/usr/local/src/${PROJECT_NAME}/.tox/${PYTHON_ENV}"
 ENV PATH="${VIRTUAL_ENV}/bin:${PATH}"
 # Remain in the checkout `WORKDIR` and make the build tools the default
 # command to run.
-WORKDIR "/usr/local/src/project-structure/"
+WORKDIR "/usr/local/src/${PROJECT_NAME}/"
 # Have to use the shell form of `CMD` because we need variable substitution:
 # hadolint ignore=DL3025
 CMD tox -e "${PYTHON_ENV}"
 
 # Then add everything that might contribute to efficient development.
 
 # Simulate the parts of the host install process from `./Makefile` needed for
 # development in the image:
 COPY [ "./build-host/requirements.txt.in", "./build-host/" ]
 # hadolint ignore=DL3042
 RUN --mount=type=cache,target=/root/.cache,sharing=locked \
     mkdir -pv "${HOME}/.local/var/log/" && \
     pip3 install -r "./build-host/requirements.txt.in" | \
-        tee -a "${HOME}/.local/var/log/project-structure-host-install.log"
+        tee -a "${HOME}/.local/var/log/${PROJECT_NAME}-host-install.log"
 
 # Match local development tool chain and avoid time consuming redundant package
 # installs.  Initialize the `$ tox -e py3##` Python virtual environment to install this
 # package and all the development tools into the image:
 COPY [ \
     "./requirements/${PYTHON_ENV}/test.txt", \
     "./requirements/${PYTHON_ENV}/devel.txt", \
```

### Comparing `project-structure-0.8.28b3/LICENSES/MIT.txt` & `project-structure-0.8.29b1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/Makefile` & `project-structure-0.8.29b1/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 #
 # To ease discovery for new contributors, variables that act as options affecting
 # behavior are at the top.  Then skip to `## Top-level targets:` below to find targets
 # intended for use by developers.  The real work, however, is in the recipes for real
 # targets that follow.  If making changes here, please start by reading the philosophy
 # commentary at the bottom of this file.
 
+# Project specific values:
+export PROJECT_NAMESPACE=rpatterson
+export PROJECT_NAME=project-structure
+
 # Variables used as options to control behavior:
 export TEMPLATE_IGNORE_EXISTING=false
 # https://devguide.python.org/versions/#supported-versions
 PYTHON_SUPPORTED_MINORS=3.10
 export DOCKER_USER=merpatterson
 # TEMPLATE: See comments towards the bottom and update.
 GPG_SIGNING_KEYID=2EFF7CCE6828E359
-CI_UPSTREAM_NAMESPACE=rpatterson
-CI_PROJECT_NAME=project-structure
 
 
 ## "Private" Variables:
 
 # Variables that aren't likely to be of concern those just using and reading top-level
 # targets.  Mostly variables whose values are derived from the environment or other
 # values.  If adding a variable whose value isn't a literal constant or intended for use
@@ -92,14 +94,16 @@
 endif
 export PYTHON_MINOR
 export PYTHON_ENV=py$(subst .,,$(PYTHON_MINOR))
 PYTHON_SHORT_MINORS=$(subst .,,$(PYTHON_MINORS))
 PYTHON_ENVS=$(PYTHON_SHORT_MINORS:%=py%)
 PYTHON_ALL_ENVS=$(PYTHON_ENVS) build
 PYTHON_EXTRAS=test devel
+PYTHON_PROJECT_PACKAGE=$(subst -,,$(PROJECT_NAME))
+PYTHON_PROJECT_GLOB=$(subst -,?,$(PROJECT_NAME))
 export PYTHON_WHEEL=
 
 # Values derived from VCS/git:
 VCS_LOCAL_BRANCH:=$(shell git branch --show-current)
 CI_COMMIT_BRANCH=
 GITHUB_REF_TYPE=
 GITHUB_REF_NAME=
@@ -262,14 +266,16 @@
 DOCKER_COMPOSE_RUN_ARGS+= --rm
 ifeq ($(shell tty),not a tty)
 DOCKER_COMPOSE_RUN_ARGS+= -T
 endif
 export DOCKER_PASS
 
 # Values derived from or overridden by CI environments:
+CI_UPSTREAM_NAMESPACE=$(PROJECT_NAMESPACE)
+CI_PROJECT_NAME=$(PROJECT_NAME)
 ifeq ($(CI),true)
 TEMPLATE_IGNORE_EXISTING=true
 endif
 GITHUB_REPOSITORY_OWNER=$(CI_UPSTREAM_NAMESPACE)
 # Determine if this checkout is a fork of the upstream project:
 CI_IS_FORK=false
 ifeq ($(GITLAB_CI),true)
@@ -396,15 +402,15 @@
 ## Build Targets:
 #
 # Recipes that make artifacts needed for by end-users, development tasks, other recipes.
 
 .PHONY: build
 ### Set up everything for development from a checkout, local and in containers.
 build: ./.git/hooks/pre-commit ./.env.~out~ \
-		$(HOME)/.local/var/log/project-structure-host-install.log \
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
 		build-docker
 
 .PHONY: $(PYTHON_ENVS:%=build-requirements-%)
 ### Compile fixed/pinned dependency versions if necessary.
 $(PYTHON_ENVS:%=build-requirements-%):
 # Avoid parallel tox recreations stomping on each other
 	$(MAKE) -e "$(@:build-requirements-%=./.tox/%/bin/pip-compile)"
@@ -434,22 +440,22 @@
 build-pkgs: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var-docker/$(PYTHON_ENV)/log/build-devel.log
 # Defined as a .PHONY recipe so that multiple targets can depend on this as a
 # pre-requisite and it will only be run once per invocation.
 	rm -vf ./dist/*
 # Build Python packages/distributions from the development Docker container for
 # consistency/reproducibility.
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    tox run -e "$(PYTHON_ENV)" --pkg-only
 # Copy the wheel to a location accessible to all containers:
 	cp -lfv "$$(
 	    ls -t ./var-docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.whl | head -n 1
 	)" "./dist/"
 # Also build the source distribution:
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    tox run -e "$(PYTHON_ENV)" --override "testenv.package=sdist" --pkg-only
 	cp -lfv "$$(
 	    ls -t ./var-docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.tar.gz | head -n 1
 	)" "./dist/"
 
 ## Docker Build Targets:
 #
@@ -566,15 +572,15 @@
 
 .PHONY: $(PYTHON_MINORS:%=build-docker-requirements-%)
 ### Pull container images and compile fixed/pinned dependency versions if necessary.
 $(PYTHON_MINORS:%=build-docker-requirements-%): ./.env.~out~
 	export PYTHON_MINOR="$(@:build-docker-requirements-%=%)"
 	export PYTHON_ENV="py$(subst .,,$(@:build-docker-requirements-%=%))"
 	$(MAKE) -e "./var-docker/$${PYTHON_ENV}/log/build-devel.log"
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    make -e PYTHON_MINORS="$(@:build-docker-requirements-%=%)" \
 	    PIP_COMPILE_ARGS="$(PIP_COMPILE_ARGS)" \
 	    build-requirements-py$(subst .,,$(@:build-docker-requirements-%=%))
 
 
 ## Test Targets:
 #
@@ -585,23 +591,29 @@
 test: test-docker-lint test-docker
 
 .PHONY: test-local
 ### Run the full suite of tests, coverage checks, and linters on the local host.
 test-local:
 	tox $(TOX_RUN_ARGS) -e "$(TOX_ENV_LIST)"
 
+.PHONY: test-lint
+### Perform any linter or style checks, including non-code checks.
+test-lint: $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log
+# Run non-code checks, e.g. documentation:
+	tox run -e "build"
+
 .PHONY: test-debug
 ### Run tests directly on the host and invoke the debugger on errors/failures.
 test-debug: ./.tox/$(PYTHON_ENV)/log/editable.log
 	$(TOX_EXEC_ARGS) -- pytest --pdb
 
 .PHONY: test-docker
 ### Run the full suite of tests, coverage checks, and code linters in containers.
-test-docker: build-pkgs $(HOME)/.local/var/log/project-structure-host-install.log \
-		build-docker ./var/log/codecov-install.log
+test-docker: build-pkgs $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
+		build-docker
 	tox run $(TOX_EXEC_OPTS) --notest -e "build"
 	$(MAKE) -e -j PYTHON_WHEEL="$(call current_pkg,.whl)" \
 	    DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --progress plain" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=test-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=test-docker-%)
@@ -612,35 +624,35 @@
 	    PYTHON_MINOR="$(@:test-docker-%=%)" \
 	    PYTHON_ENV="py$(subst .,,$(@:test-docker-%=%))" \
 	    test-docker-pyminor
 
 .PHONY: test-docker-pyminor
 ### Run the full suite of tests inside a docker container for this Python version.
 test-docker-pyminor: build-docker-$(PYTHON_MINOR) \
-		$(HOME)/.local/var/log/project-structure-host-install.log \
-		./var/log/codecov-install.log
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log
 	docker_run_args="--rm"
 	if [ ! -t 0 ]
 	then
 # No fancy output when running in parallel
 	    docker_run_args+=" -T"
 	fi
 # Ensure the dist/package has been correctly installed in the image
-	docker compose run --no-deps $${docker_run_args} project-structure \
-	    python -m projectstructure --help
-	docker compose run --no-deps $${docker_run_args} project-structure \
-	    project-structure --help
+	docker compose run --no-deps $${docker_run_args} $(PROJECT_NAME) \
+	    python -m "$(PYTHON_PROJECT_PACKAGE)" --help
+	docker compose run --no-deps $${docker_run_args} $(PROJECT_NAME) \
+	    $(PROJECT_NAME) --help
 # Run from the development Docker container for consistency
-	docker compose run $${docker_run_args} project-structure-devel \
+	docker compose run $${docker_run_args} $(PROJECT_NAME)-devel \
 	    make -e PYTHON_MINORS="$(PYTHON_MINORS)" PYTHON_WHEEL="$(PYTHON_WHEEL)" \
 	        test-local
 # Upload any build or test artifacts to CI/CD providers
 ifeq ($(GITLAB_CI),true)
 ifeq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 ifneq ($(CODECOV_TOKEN),)
+	$(MAKE) "./var/log/codecov-install.log"
 	codecov --nonZero -t "$(CODECOV_TOKEN)" \
 	    --file "./build/$(PYTHON_ENV)/coverage.xml"
 else ifneq ($(CI_IS_FORK),true)
 	set +x
 	echo "ERROR: CODECOV_TOKEN missing from ./.env or CI secrets"
 	false
 endif
@@ -654,15 +666,15 @@
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./build-host/Dockerfile"
 
 .PHONY: test-push
 ### Perform any checks that should only be run before pushing.
 test-push: $(VCS_FETCH_TARGETS) \
-		$(HOME)/.local/var/log/project-structure-host-install.log \
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
 		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env.~out~
 	vcs_compare_rev="$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)"
 ifeq ($(CI),true)
 ifneq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 # Don't waste CI time, only check for the canonical version:
 	exit
 endif
@@ -687,15 +699,15 @@
 	then
 	    exit
 	elif (( $$exit_code != 0 ))
 	then
 	    exit $$exit_code
 	else
 	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
-	        project-structure-devel $(TOX_EXEC_ARGS) -- \
+	        $(PROJECT_NAME)-devel $(TOX_EXEC_ARGS) -- \
 	        towncrier check --compare-with "$${vcs_compare_rev}"
 	fi
 
 .PHONY: test-clean
 ### Confirm that the checkout is free of uncommitted VCS changes.
 test-clean:
 	if [ -n "$$(git status --porcelain)" ]
@@ -713,33 +725,33 @@
 
 .PHONY: release
 ### Publish installable Python packages and container images as required by commits.
 release: release-pkgs release-docker
 
 .PHONY: release-pkgs
 ### Publish installable Python packages to PyPI if conventional commits require.
-release-pkgs: $(HOME)/.local/var/log/project-structure-host-install.log \
+release-pkgs: $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
 		./var/log/git-remotes.log \
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) ~/.pypirc.~out~ \
 		./.env.~out~
 # Only release from the `main` or `develop` branches:
 ifeq ($(RELEASE_PUBLISH),true)
 # Import the private signing key from CI secrets
 	$(MAKE) -e ./var/log/gpg-import.log
 # Bump the version and build the final release packages:
 	$(MAKE) -e build-pkgs
 # https://twine.readthedocs.io/en/latest/#using-twine
-	./.tox/build/bin/twine check ./dist/project?structure-*
+	$(TOX_EXEC_BUILD_ARGS) -- twine check ./dist/$(PYTHON_PROJECT_GLOB)-*
 # The VCS remote should reflect the release before the release is published to ensure
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
-	./.tox/build/bin/twine upload -s -r "$(PYPI_REPO)" \
-	    ./dist/project?structure-*
+	$(TOX_EXEC_BUILD_ARGS) -- twine upload -s -r "$(PYPI_REPO)" \
+	    ./dist/$(PYTHON_PROJECT_GLOB)-*
 	export VERSION=$$($(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project)
 # Create a GitLab release
 	./.tox/build/bin/twine upload -s -r "gitlab" \
 	    ./dist/project?structure-*
 	release_cli_args="--description ./NEWS-VERSION.rst"
 	release_cli_args+=" --tag-name v$${VERSION}"
 	release_cli_args+=" --assets-link {\
@@ -750,15 +762,15 @@
 	release_cli_args+=" --assets-link {\
 	\"name\":\"GitLab-PyPI-Package-Registry\",\
 	\"url\":\"$(CI_SERVER_URL)/$(CI_PROJECT_PATH)/-/packages/\",\
 	\"link_type\":\"package\"\
 	}"
 	release_cli_args+=" --assets-link {\
 	\"name\":\"Docker-Hub-Container-Registry\",\
-	\"url\":\"https://hub.docker.com/r/merpatterson/$(CI_PROJECT_NAME)/tags\",\
+	\"url\":\"https://hub.docker.com/r/$(DOCKER_USER)/$(CI_PROJECT_NAME)/tags\",\
 	\"link_type\":\"image\"\
 	}"
 	docker compose pull gitlab-release-cli
 	docker compose run --rm gitlab-release-cli release-cli \
 	    --server-url "$(CI_SERVER_URL)" --project-id "$(CI_PROJECT_ID)" \
 	    create $${release_cli_args}
 # Create a GitHub release
@@ -795,23 +807,23 @@
 # Update Docker Hub `README.md` using the `./README.rst` reStructuredText version using
 # the official/canonical Python version:
 ifeq ($(VCS_BRANCH),main)
 	if [ "$${PYTHON_ENV}" == "$(PYTHON_HOST_ENV)" ]
 	then
 	    $(MAKE) -e "./var/log/docker-login-DOCKER.log"
 	    docker compose pull --quiet pandoc docker-pushrm
-	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) docker-pushrm
+	    docker compose up docker-pushrm
 	fi
 endif
 
 .PHONY: release-bump
 ### Bump the package version if on a branch that should trigger a release.
 release-bump: ~/.gitconfig $(VCS_RELEASE_FETCH_TARGETS) \
 		./var/log/git-remotes.log \
-		$(HOME)/.local/var/log/project-structure-host-install.log \
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
 		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env.~out~
 	if ! git diff --cached --exit-code
 	then
 	    set +x
 	    echo "CRITICAL: Cannot bump version with staged changes"
 	    false
 	fi
@@ -852,21 +864,21 @@
 # Capture the release notes for *just this* release for creating the GitHub release.
 # Have to run before the real `$ towncrier build` run without the `--draft` option
 # because after that the `newsfragments` will have been deleted.
 	next_version=$$(
 	    $(TOX_EXEC_BUILD_ARGS) -qq -- cz bump $${cz_bump_args} --yes --dry-run |
 	    sed -nE 's|.* ([^ ]+) *→ *([^ ]+).*|\2|p;q'
 	) || true
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    $(TOX_EXEC_ARGS) -qq -- \
 	    towncrier build --version "$${next_version}" --draft --yes \
 	    >"./NEWS-VERSION.rst"
 	git add -- "./NEWS-VERSION.rst"
 # Build and stage the release notes to be commited by `$ cz bump`:
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    $(TOX_EXEC_ARGS) -- towncrier build --version "$${next_version}" --yes
 # Increment the version in VCS
 	$(TOX_EXEC_BUILD_ARGS) -- cz bump $${cz_bump_args}
 # Ensure the container image reflects the version bump but we don't need to update the
 # requirements again.
 	touch \
 	    $(PYTHON_ENVS:%=./requirements/%/user.txt) \
@@ -898,31 +910,31 @@
 
 ## Development Targets:
 #
 # Recipes used by developers to make changes to the code.
 
 .PHONY: devel-format
 ### Automatically correct code in this checkout according to linters and style checkers.
-devel-format: $(HOME)/.local/var/log/project-structure-host-install.log
+devel-format: $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log
 	$(TOX_EXEC_ARGS) -- autoflake -r -i --remove-all-unused-imports \
 		--remove-duplicate-keys --remove-unused-variables \
-		--remove-unused-variables "./src/projectstructure/"
-	$(TOX_EXEC_ARGS) -- autopep8 -v -i -r "./src/projectstructure/"
-	$(TOX_EXEC_ARGS) -- black "./src/projectstructure/"
+		--remove-unused-variables "./src/$(PYTHON_PROJECT_PACKAGE)/"
+	$(TOX_EXEC_ARGS) -- autopep8 -v -i -r "./src/$(PYTHON_PROJECT_PACKAGE)/"
+	$(TOX_EXEC_ARGS) -- black "./src/$(PYTHON_PROJECT_PACKAGE)/"
 	$(TOX_EXEC_ARGS) -- reuse addheader -r --skip-unrecognised \
 	    --copyright "Ross Patterson <me@rpatterson.net>" --license "MIT" "./"
 
 .PHONY: devel-upgrade
 ### Update all fixed/pinned dependencies to their latest available versions.
-devel-upgrade: ./.env.~out~ $(HOME)/.local/var/log/project-structure-host-install.log \
-		./var-docker/$(PYTHON_ENV)/log/build-devel.log
+devel-upgrade: ./.env.~out~ $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
+		build-docker
 	touch "./setup.cfg" "./requirements/build.txt.in" \
 	    "./build-host/requirements.txt.in"
 # Ensure the network is create first to avoid race conditions
-	docker compose create project-structure-devel
+	docker compose create $(PROJECT_NAME)-devel
 	$(MAKE) -e -j PIP_COMPILE_ARGS="--upgrade" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=build-docker-requirements-%)
 # Update VCS hooks from remotes to the latest tag.
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit autoupdate
 
 .PHONY: devel-upgrade-branch
@@ -996,15 +1008,15 @@
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit uninstall \
 	    --hook-type "pre-commit" --hook-type "commit-msg" --hook-type "pre-push" \
 	    || true
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit clean || true
 	git clean -dfx -e "/var" -e "var-docker/" -e "/.env" -e "*~"
 	git clean -dfx "./var-docker/py*/.tox/" \
 	    "./var-docker/py*/project_structure.egg-info/"
-	rm -rfv "./var/log/" "./var-docker/py*/log/"
+	rm -rfv "./var/log/" ./var-docker/py*/log/
 
 
 ## Real Targets:
 #
 # Recipes that make actual changes and create and update files for the target.
 
 # Manage fixed/pinned versions in `./requirements/**.txt` files.  Has to be run for each
@@ -1052,21 +1064,21 @@
 
 # Targets used as pre-requisites to ensure virtual environments managed by tox have been
 # created and can be used directly to save time on Tox's overhead when we don't need
 # Tox's logic about when to update/recreate them, e.g.:
 #     $ ./.tox/build/bin/cz --help
 # Mostly useful for build/release tools.
 $(PYTHON_ALL_ENVS:%=./.tox/%/bin/pip-compile):
-	$(MAKE) -e "$(HOME)/.local/var/log/project-structure-host-install.log"
+	$(MAKE) -e "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
 	tox run $(TOX_EXEC_OPTS) -e "$(@:.tox/%/bin/pip-compile=%)" --notest
 # Workaround tox's `usedevelop = true` not working with `./pyproject.toml`.  Use as a
 # prerequisite when using Tox-managed virtual environments directly and changes to code
 # need to take effect immediately.
 $(PYTHON_ENVS:%=./.tox/%/log/editable.log):
-	$(MAKE) -e "$(HOME)/.local/var/log/project-structure-host-install.log"
+	$(MAKE) -e "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
 	mkdir -pv "$(dir $(@))"
 	tox exec $(TOX_EXEC_OPTS) -e "$(@:./.tox/%/log/editable.log=%)" -- \
 	    pip3 install -e "./" |& tee -a "$(@)"
 
 ## Docker real targets:
 
 # Build the development image:
@@ -1080,33 +1092,33 @@
 	mkdir -pv "$(dir $(@))"
 ifeq ($(DOCKER_BUILD_PULL),true)
 # Pull the development image and simulate as if it had been built here.
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
 	    touch "$(@)" "./var-docker/$(PYTHON_ENV)/log/rebuild.log"
 # Ensure the virtualenv in the volume is also current:
-	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
+	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	        tox run $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)" --notest
 	    exit
 	fi
 endif
 	$(MAKE) -e DOCKER_VARIANT="devel" DOCKER_BUILD_ARGS="--load" \
 	    build-docker-build | tee -a "$(@)"
 # Represent that host install is baked into the image in the `${HOME}` bind volume:
-	docker compose run --rm -T --workdir "/home/project-structure/" \
-	    --entrypoint "mkdir" project-structure-devel -pv "./.local/var/log/"
-	docker run --rm --workdir "/home/project-structure/" --entrypoint "cat" \
-	    "$$(docker compose config --images project-structure-devel | head -n 1)" \
-	    "./.local/var/log/project-structure-host-install.log" |
-	    docker compose run --rm -T --workdir "/home/project-structure/" \
-	        --entrypoint "tee" project-structure-devel -a \
-	        "./.local/var/log/project-structure-host-install.log" >"/dev/null"
+	docker compose run --rm -T --workdir "/home/$(PROJECT_NAME)/" \
+	    $(PROJECT_NAME)-devel mkdir -pv "./.local/var/log/"
+	docker run --rm --workdir "/home/$(PROJECT_NAME)/" --entrypoint "cat" \
+	    "$$(docker compose config --images $(PROJECT_NAME)-devel | head -n 1)" \
+	    "./.local/var/log/$(PROJECT_NAME)-host-install.log" |
+	    docker compose run --rm -T --workdir "/home/$(PROJECT_NAME)/" \
+	        $(PROJECT_NAME)-devel tee -a \
+	        "./.local/var/log/$(PROJECT_NAME)-host-install.log" >"/dev/null"
 # Update the pinned/frozen versions, if needed, using the container.  If changed, then
 # we may need to re-build the container image again to ensure it's current and correct.
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) project-structure-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    make -e PYTHON_MINORS="$(PYTHON_MINOR)" build-requirements-$(PYTHON_ENV)
 ifeq ($(CI),true)
 # On CI, any changes from compiling requirements is a failure so no need to waste time
 # rebuilding images:
 	touch "$(@)"
 else
 	$(MAKE) -e "$(@)"
@@ -1139,15 +1151,15 @@
 ./.env.~out~: ./.env.in
 	$(call expand_template,$(<),$(@))
 
 # Install all tools required by recipes that have to be installed externally on the
 # host.  Use a target file outside this checkout to support multiple checkouts.  Use a
 # target specific to this project so that other projects can use the same approach but
 # with different requirements.
-$(HOME)/.local/var/log/project-structure-host-install.log: ./bin/host-install \
+$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log: ./bin/host-install \
 		./build-host/requirements.txt.in
 	mkdir -pv "$(dir $(@))"
 	"$(<)" |& tee -a "$(@)"
 
 # https://docs.docker.com/build/building/multi-platform/#building-multi-platform-images
 $(HOME)/.local/var/log/docker-multi-platform-host-install.log:
 	mkdir -pv "$(dir $(@))"
@@ -1210,21 +1222,21 @@
 	then
 # If the local branch doesn't exist, fall back to the pre-release branch:
 	    git fetch $${git_fetch_args} "$${branch_path%%/*}" "develop" |&
 	        tee -a "$(@)"
 	fi
 
 ./.git/hooks/pre-commit:
-	$(MAKE) -e "$(HOME)/.local/var/log/project-structure-host-install.log"
+	$(MAKE) -e "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit install \
 	    --hook-type "pre-commit" --hook-type "commit-msg" --hook-type "pre-push"
 
 # Capture any project initialization tasks for reference.  Not actually usable.
 ./pyproject.toml:
-	$(MAKE) -e "$(HOME)/.local/var/log/project-structure-host-install.log"
+	$(MAKE) -e "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
 	$(TOX_EXEC_BUILD_ARGS) -- cz init
 
 # Tell Emacs where to find checkout-local tools needed to check the code.
 ./.dir-locals.el.~out~: ./.dir-locals.el.in
 	$(call expand_template,$(<),$(@))
 
 # Ensure minimal VCS configuration, mostly useful in automation such as CI.
@@ -1269,15 +1281,15 @@
 	$(call expand_template,$(<),$(@))
 
 ./var/log/docker-login-DOCKER.log:
 	$(MAKE) "./.env.~out~"
 	mkdir -pv "$(dir $(@))"
 	if [ -n "$${DOCKER_PASS}" ]
 	then
-	    printenv "DOCKER_PASS" | docker login -u "merpatterson" --password-stdin
+	    printenv "DOCKER_PASS" | docker login -u "$(DOCKER_USER)" --password-stdin
 	elif [ "$(CI_IS_FORK)" != "true" ]
 	then
 	    echo "ERROR: DOCKER_PASS missing from ./.env or CI secrets"
 	    false
 	fi
 	date | tee -a "$(@)"
 # TEMPLATE: Add a cleanup rule for the GitLab container registry under the project
@@ -1392,32 +1404,39 @@
 # *but* it is required to expand templates.  We can't use a sub-make because any
 # expanded templates we use in `include ...` directives, such as `./.env`, are updated
 # as targets when reading the `./Makefile` leading to endless recursion.
 define expand_template=
 if ! which envsubst
 then
     mkdir -pv "$(HOME)/.local/var/log/"
-    ./bin/host-install >"$(HOME)/.local/var/log/project-structure-host-install.log"
+    ./bin/host-install >"$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
+fi
+if [ "$(2:%.~out~=%)" -nt "$(1)" ]
+then
+    envsubst <"$(1)" >"$(2)"
+    exit
+fi
+if [ ! -e "$(2:%.~out~=%)" ]
+then
+    touch -d "@0" "$(2:%.~out~=%)"
 fi
-is_target_newer="0"
-test "$(2:%.~out~=%)" -nt "$(1)" || is_target_newer="$${?}"
-touch "$(2:%.~out~=%)"
 if [ "$(CI)" != "true" ]
 then
     envsubst <"$(1)" | diff -u "$(2:%.~out~=%)" "-" || true
 fi
 set +x
 echo "WARNING:Template $(1) has been updated."
 echo "        Reconcile changes and \`$$ touch $(2:%.~out~=%)\`."
 set -x
 if [ ! -s "$(2:%.~out~=%)" ]
 then
     envsubst <"$(1)" >"$(2:%.~out~=%)"
+    touch -d "@0" "$(2:%.~out~=%)"
 fi
-if [ "$(TEMPLATE_IGNORE_EXISTING)" == "true" ] || (( "$${is_target_newer}" == 0 ))
+if [ "$(TEMPLATE_IGNORE_EXISTING)" == "true" ]
 then
     envsubst <"$(1)" >"$(2)"
     exit
 fi
 exit 1
 endef
 
@@ -1503,15 +1522,15 @@
 ## Maintainer targets:
 #
 # Recipes not used during the normal course of development.
 
 .PHONY: pull-docker
 ### Pull an existing image best to use as a cache for building new images
 pull-docker: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		$(HOME)/.local/var/log/project-structure-host-install.log
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log
 	export VERSION=$$($(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project)
 	for vcs_branch in $(VCS_BRANCHES)
 	do
 	    docker_tag="$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${vcs_branch}"
 	    for docker_image in $(DOCKER_IMAGES)
 	    do
 	        if docker pull "$${docker_image}:$${docker_tag}"
```

### Comparing `project-structure-0.8.28b3/NEWS.rst` & `project-structure-0.8.29b1/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+project-structure 0.8.29b1 (2023-05-10)
+=======================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+project-structure 0.8.29b0 (2023-05-10)
+=======================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Tue May  9 09:31:01 PM UTC 2023.
+
+
+project-structure 0.8.28 (2023-05-08)
+=====================================
+
+No significant changes.
+
+
 project-structure 0.8.28b3 (2023-05-08)
 =======================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `project-structure-0.8.28b3/PKG-INFO` & `project-structure-0.8.29b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-structure
-Version: 0.8.28b3
+Version: 0.8.29b1
 Summary: Project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `project-structure-0.8.28b3/README.rst` & `project-structure-0.8.29b1/README.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/TODO.rst` & `project-structure-0.8.29b1/TODO.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/bin/cz-check-bump` & `project-structure-0.8.29b1/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/bin/entrypoint` & `project-structure-0.8.29b1/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/bin/get-base-version` & `project-structure-0.8.29b1/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/bin/host-install` & `project-structure-0.8.29b1/bin/host-install`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/build-host/Dockerfile` & `project-structure-0.8.29b1/build-host/Dockerfile`

 * *Files 12% similar despite different names*

```diff
@@ -22,32 +22,36 @@
     "py3-pip" \
     "gnupg" \
     "curl" \
     "tar" \
     "github-cli" \
     && rm -rf /var/cache/apk/*
 
+# Project contstants:
+ARG PROJECT_NAMESPACE=rpatterson
+ARG PROJECT_NAME=project-structure
+
 # Find the same home directory even when run as another user, e.g. `root`.
 ENV HOME="/home/runner"
 # Add user installs to PATH
 ENV PATH="${HOME}/.local/bin:${PATH}"
 
 COPY [ "./requirements-py310.txt", "${HOME}/.local/lib/" ]
 RUN mkdir -pv "${HOME}/.local/var/log/" && \
     pip3 install --no-cache-dir --user -r "${HOME}/.local/lib/requirements-py310.txt" \
-    >"${HOME}/.local/var/log/project-structure-host-install.log"
+    >"${HOME}/.local/var/log/${PROJECT_NAME}-host-install.log"
 
 COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
 ENTRYPOINT [ "docker-entrypoint.sh", "entrypoint" ]
 CMD [ "make", "-e", "build-docker" ]
 
 # https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
-LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/project-structure"
-LABEL org.opencontainers.image.documentation="https://gitlab.com/rpatterson/project-structure"
-LABEL org.opencontainers.image.source="https://gitlab.com/rpatterson/project-structure"
+LABEL org.opencontainers.image.url="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECT_NAME}"
+LABEL org.opencontainers.image.documentation="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECT_NAME}"
+LABEL org.opencontainers.image.source="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECT_NAME}"
 LABEL org.opencontainers.image.title="Project Structure Build Host"
 LABEL org.opencontainers.image.description="Project structure foundation or template, build host"
 LABEL org.opencontainers.image.licenses="MIT"
 LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
 LABEL org.opencontainers.image.vendor="rpatterson.net"
 LABEL org.opencontainers.image.base.name="docker.io/library/docker:latest"
 # Build-time `LABEL`s
```

### Comparing `project-structure-0.8.28b3/build-host/Makefile` & `project-structure-0.8.29b1/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/build-host/README.rst` & `project-structure-0.8.29b1/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/build-host/bin/entrypoint` & `project-structure-0.8.29b1/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/build-host/requirements-py310.txt` & `project-structure-0.8.29b1/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/build-host/requirements-py311.txt` & `project-structure-0.8.29b1/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/build-host/requirements-py37.txt` & `project-structure-0.8.29b1/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/build-host/requirements-py38.txt` & `project-structure-0.8.29b1/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/build-host/requirements-py39.txt` & `project-structure-0.8.29b1/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/docker-compose.override.yml` & `project-structure-0.8.29b1/docker-compose.override.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,36 +8,36 @@
 version: "3.8"
 
 services:
 
   # Configuration specific to development:
   project-structure:
     image: "\
-      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/project-structure\
-      :${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
-    container_name: "project-structure-checkout"
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/${PROJECT_NAMESPACE:?}\
+      /${PROJECT_NAME:?}:${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
+    container_name: "${PROJECT_NAME:?}-checkout"
     build:
       context: "${CHECKOUT_DIR:-.}/"
       target: "user"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
     volumes:
       # Preserve caches caches between container runs
-      - "${CHECKOUT_DIR:-.}/home/:/home/project-structure/"
+      - "${CHECKOUT_DIR:-.}/home/:/home/${PROJECT_NAME:?}/"
 
   ## Contianers used for development and release:
 
   # Container for use by developers:
   project-structure-devel:
     image: "\
-      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/project-structure\
-      :devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
-    container_name: "project-structure-devel"
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/${PROJECT_NAMESPACE:?}\
+      /${PROJECT_NAME:?}:devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
+    container_name: "${PROJECT_NAME:?}-devel"
     profiles:
       - "test"
     build:
       context: "${CHECKOUT_DIR:-.}/"
       target: "devel"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
@@ -50,37 +50,37 @@
       PGID: "${PGID:-${PUID:-1000}}"
       # Variables from the environment we want to be passed through into the container:
       CI: "${CI:-false}"
       # DEBUG: "true"
     volumes:
       # Ensure local changes are reflected inside the container.
       - "${CHECKOUT_DIR:-.}/bin/entrypoint:/usr/local/bin/entrypoint"
-      - "${CHECKOUT_DIR:-.}/:/usr/local/src/project-structure/"
+      - "${CHECKOUT_DIR:-.}/:/usr/local/src/${PROJECT_NAME:?}/"
       # Preserve caches caches between container runs
-      - "${CHECKOUT_DIR:-.}/home/:/home/project-structure/"
+      - "${CHECKOUT_DIR:-.}/home/:/home/${PROJECT_NAME:?}/"
       # Avoid any clashes between image variants and/or the local host at both build and
       # run-time.
       - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}/\
-        :/usr/local/src/project-structure/var/"
+        :/usr/local/src/${PROJECT_NAME:?}/var/"
       - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}/.tox/\
-        :/usr/local/src/project-structure/.tox/"
+        :/usr/local/src/${PROJECT_NAME:?}/.tox/"
       - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}\
         /project_structure.egg-info/\
-        :/usr/local/src/project-structure/src/project_structure.egg-info/"
+        :/usr/local/src/${PROJECT_NAME:?}/src/project_structure.egg-info/"
 
   # https://github.com/hadolint/hadolint#how-to-use
   hadolint:
     image: "ghcr.io/hadolint/hadolint"
     profiles:
       - "test"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
-      - "${CHECKOUT_DIR:-.}/:/usr/local/src/project-structure/"
-    working_dir: "/usr/local/src/project-structure/"
+      - "${CHECKOUT_DIR:-.}/:/usr/local/src/${PROJECT_NAME:-}/"
+    working_dir: "/usr/local/src/${PROJECT_NAME:-}/"
     command: >-
       hadolint "./Dockerfile"
 
   pandoc:
     image: "pandoc/core"
     profiles:
       - "release"
@@ -104,39 +104,39 @@
     depends_on:
       pandoc:
         condition: "service_completed_successfully"
     profiles:
       - "release"
     environment:
       TZ: "${TZ:-Etc/UTC}"
-      DOCKER_USER: "${DOCKER_USER:-merpatterson}"
-      DOCKER_PASS: "${DOCKER_PASS}"
+      DOCKER_USER: "${DOCKER_USER:-}"
+      DOCKER_PASS: "${DOCKER_PASS:-}"
     volumes:
       - "${CHECKOUT_DIR:-.}/:/data/"
     command: >-
       --file "/data/README.md"
       --short "Project structure foundation or template"
-      --debug "merpatterson/project-structure"
+      --debug "${DOCKER_USER:-}/${PROJECT_NAME:-}"
 
   gitlab-release-cli:
     image: "${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/gitlab-org/release-cli:latest"
     profiles:
       - "release"
     environment:
       CI_JOB_TOKEN: "${CI_JOB_TOKEN:-}"
     volumes:
-      - "./:/usr/local/src/project-structure/"
-    working_dir: "/usr/local/src/project-structure/"
+      - "./:/usr/local/src/${PROJECT_NAME:-}/"
+    working_dir: "/usr/local/src/${PROJECT_NAME:-}/"
 
   ## Containers related to CI/CD:
 
   # The container in which CI/CD is run:
   build-host:
     image: "\
-      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/project-structure\
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/${DOCKER_USER:-}/${PROJECT_NAME:-}\
       :build-host"
     profiles:
       - "ci"
     build: "${CHECKOUT_DIR:-.}/build-host/"
     privileged: true
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
```

### Comparing `project-structure-0.8.28b3/docker-compose.yml` & `project-structure-0.8.29b1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/gitlab-runner/config/config.toml.in` & `project-structure-0.8.29b1/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/gitlab-runner/docker-compose.yml` & `project-structure-0.8.29b1/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/pyproject.toml` & `project-structure-0.8.29b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/build.txt.in` & `project-structure-0.8.29b1/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py310/build.txt` & `project-structure-0.8.29b1/requirements/py310/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
```

### Comparing `project-structure-0.8.28b3/requirements/py310/devel.txt` & `project-structure-0.8.29b1/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py310/test.txt` & `project-structure-0.8.29b1/requirements/py310/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py311/build.txt` & `project-structure-0.8.29b1/requirements/py311/build.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
```

### Comparing `project-structure-0.8.28b3/requirements/py311/devel.txt` & `project-structure-0.8.29b1/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py311/test.txt` & `project-structure-0.8.29b1/requirements/py311/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py37/build.txt` & `project-structure-0.8.29b1/requirements/py37/build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
```

### Comparing `project-structure-0.8.28b3/requirements/py37/devel.txt` & `project-structure-0.8.29b1/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py37/test.txt` & `project-structure-0.8.29b1/requirements/py37/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py38/build.txt` & `project-structure-0.8.29b1/requirements/py38/build.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
```

### Comparing `project-structure-0.8.28b3/requirements/py38/devel.txt` & `project-structure-0.8.29b1/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py38/test.txt` & `project-structure-0.8.29b1/requirements/py38/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py39/build.txt` & `project-structure-0.8.29b1/requirements/py39/build.txt`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
```

### Comparing `project-structure-0.8.28b3/requirements/py39/devel.txt` & `project-structure-0.8.29b1/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/requirements/py39/test.txt` & `project-structure-0.8.29b1/requirements/py39/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/setup.cfg` & `project-structure-0.8.29b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/src/project_structure.egg-info/PKG-INFO` & `project-structure-0.8.29b1/src/project_structure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-structure
-Version: 0.8.28b3
+Version: 0.8.29b1
 Summary: Project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
```

### Comparing `project-structure-0.8.28b3/src/project_structure.egg-info/SOURCES.txt` & `project-structure-0.8.29b1/src/project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/src/projectstructure/__init__.py` & `project-structure-0.8.29b1/src/projectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/src/projectstructure/tests/test_cli.py` & `project-structure-0.8.29b1/src/projectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.28b3/tox.ini` & `project-structure-0.8.29b1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 [tox]
 # https://devguide.python.org/versions/#supported-versions
 envlist = py{310,311,39,38,37}
 # https://tox.wiki/en/latest/example/package.html#setuptools
 isolated_build = True
 
+[project]
+name = project-structure
+package = projectstructure
+
 [testenv]
 description = Run the project test suite
 package = wheel
 wheel_build_env = .pkg
 passenv =
     HOME
     PYTHON_HOST_ENV
@@ -32,44 +36,44 @@
 commands =
 # Create a directory for artifacts not managed by `$ tox`:
     python -c 'import pathlib; \
         pathlib.Path("./build/{envname}").mkdir(parents=True, exist_ok=True)'
 # Fail fast.  Run quick tests and checks first to save time in the inner loop of
 # development iteration.
     pyroma --min="10" "./"
-    black --check "./src/projectstructure/"
+    black --check "./src/{[project]package}/"
 # https://github.com/PyCQA/prospector/issues/599#issue-1600120419
     pylint --output-format \
         "colorized,parseable:{envdir}/pylint.parseable,json:{envdir}/pylint.json,msvs:{envdir}/pylint.msvs" \
-        "./src/projectstructure/"
+        "./src/{[project]package}/"
 # https://pawamoy.github.io/posts/python-static-code-analysis-tools/#prospector
     prospector \
         --output-format "emacs:./build/{envname}/prospector-emacs.txt" \
         --output-format "grouped:./build/{envname}/prospector-grouped.txt" \
         --output-format "json:./build/{envname}/prospector.json" \
         --output-format "pylint:./build/{envname}/prospector.pylint" \
         --output-format "text:./build/{envname}/prospector.txt" \
         --output-format "vscode:./build/{envname}/prospector-vscode.txt" \
         --output-format "xunit:./build/{envname}/prospector-xunit.xml" \
         --output-format "yaml:./build/{envname}/prospector.yaml" \
         --output-format "grouped" \
-        "./src/projectstructure/"
+        "./src/{[project]package}/"
 # https://github.com/PyCQA/prospector/issues/599#issue-1600120419
-    vulture "./src/projectstructure/"
+    vulture "./src/{[project]package}/"
 # https://xenon.readthedocs.io/en/latest/#an-actual-example
     xenon --max-absolute "A" --max-modules "A" --max-average "A" \
-        "./src/projectstructure/"
+        "./src/{[project]package}/"
 # Check documentation as much a possible:
     rstcheck -r "./README.rst" "./CONTRIBUTING.rst" "./TODO.rst" \
         "./newsfragments/"
 # Check copyright and licensing:
     reuse lint
 # Ensure this package is correctly installed into this environment.
-    python -m "projectstructure" --help
-    project-structure --help
+    python -m "{[project]package}" --help
+    {[project]name} --help
 # Run more time consuming tests and checks last.
     coverage run --data-file="./build/{envname}/.coverage" -m {[testenv]commands}
     coverage json --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -o "./build/{envname}/coverage.json"
     coverage lcov --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -o "./build/{envname}/coverage-lcov.info"
     coverage xml --fail-under=0 --data-file="./build/{envname}/.coverage" \
```

