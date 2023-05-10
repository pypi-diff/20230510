# Comparing `tmp/project-structure-0.8.29b1.tar.gz` & `tmp/project-structure-0.8.30b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project-structure-0.8.29b1.tar", last modified: Wed May 10 09:10:40 2023, max compression
+gzip compressed data, was "project-structure-0.8.30b0.tar", last modified: Wed May 10 12:23:33 2023, max compression
```

## Comparing `project-structure-0.8.29b1.tar` & `project-structure-0.8.30b0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      821 2023-05-10 09:05:29.000000 project-structure-0.8.29b1/.cz.toml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      643 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.dir-locals.el.in
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1717 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.dockerignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1418 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.env.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.276727 project-structure-0.8.29b1/.github/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.276727 project-structure-0.8.29b1/.github/workflows/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4646 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/.github/workflows/build-test.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1717 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     6365 2023-05-10 09:04:31.000000 project-structure-0.8.29b1/.gitlab-ci.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      877 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.pre-commit-config.yaml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2472 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/.prospector.yaml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.276727 project-structure-0.8.29b1/.reuse/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      790 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.reuse/dep5
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/.tox/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5411 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/CONTRIBUTING.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4942 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/Dockerfile
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/LICENSES/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1071 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/LICENSES/MIT.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    60235 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/Makefile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      140 2023-05-10 09:05:27.000000 project-structure-0.8.29b1/NEWS-VERSION.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    14153 2023-05-10 09:05:28.000000 project-structure-0.8.29b1/NEWS.rst
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17800 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/PKG-INFO
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    16758 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/README.rst
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4388 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/TODO.rst
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/bin/
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2860 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/cz-check-bump
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1052 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/entrypoint
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1202 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/get-base-version
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)      422 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/hadolint
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1480 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/bin/host-install
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/build-host/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2264 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/Dockerfile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1584 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/Makefile
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      849 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/README.rst
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/build-host/bin/
--rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2152 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/bin/entrypoint
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      730 2023-05-10 09:05:42.000000 project-structure-0.8.29b1/build-host/requirements-py310.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      673 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements-py311.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      947 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements-py37.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements-py38.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements-py39.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      104 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/build-host/requirements.txt.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/dist/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      222 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/dist/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5301 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/docker-compose.override.yml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      741 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/docker-compose.yml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/gitlab-runner/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/gitlab-runner/config/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1423 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      666 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/home/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      246 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/home/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      427 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/home/.pypirc.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/newsfragments/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      187 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/newsfragments/.gitignore
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1862 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/pyproject.toml
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      679 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/build.txt.in
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py310/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py310/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4720 2023-05-10 09:05:42.000000 project-structure-0.8.29b1/requirements/py310/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      864 2023-05-10 09:07:28.000000 project-structure-0.8.29b1/requirements/py310/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      257 2023-05-10 09:05:42.000000 project-structure-0.8.29b1/requirements/py310/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py311/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py311/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4548 2023-05-10 00:03:59.000000 project-structure-0.8.29b1/requirements/py311/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      749 2023-05-10 00:03:39.000000 project-structure-0.8.29b1/requirements/py311/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      264 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/requirements/py311/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py37/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2659 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py37/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5138 2023-05-10 08:44:47.000000 project-structure-0.8.29b1/requirements/py37/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1072 2023-05-10 08:44:40.000000 project-structure-0.8.29b1/requirements/py37/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      399 2023-05-10 08:44:38.000000 project-structure-0.8.29b1/requirements/py37/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py38/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2502 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py38/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4760 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/requirements/py38/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/requirements/py38/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/requirements/py38/user.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/requirements/py39/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2380 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/requirements/py39/build.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4747 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/requirements/py39/devel.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/requirements/py39/test.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/requirements/py39/user.txt
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1660 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/setup.cfg
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.276727 project-structure-0.8.29b1/src/
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/src/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/src/project_structure.egg-info/.gitignore
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17800 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/PKG-INFO
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)     2597 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/SOURCES.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)        1 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/dependency_links.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)       60 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/entry_points.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)      151 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/requires.txt
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)       17 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/project_structure.egg-info/top_level.txt
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/src/projectstructure/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4356 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/src/projectstructure/__init__.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      303 2023-05-10 08:48:46.000000 project-structure-0.8.29b1/src/projectstructure/__main__.py
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/src/projectstructure/tests/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      165 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/src/projectstructure/tests/__init__.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4457 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/src/projectstructure/tests/test_cli.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      495 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/src/projectstructure/utils.py
--rw-r--r--   0 project-structure  (1001) project-structure  (1001)      164 2023-05-10 09:10:40.000000 project-structure-0.8.29b1/src/projectstructure/version.py
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      281 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/towncrier.toml
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3652 2023-05-09 23:59:52.000000 project-structure-0.8.29b1/tox.ini
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      229 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py310/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py310/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py310/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py310/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py310/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py310/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py311/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py311/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py311/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py311/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py311/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py311/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py37/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py37/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py37/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py37/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py37/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py37/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py38/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py38/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.280727 project-structure-0.8.29b1/var-docker/py38/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py38/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/var-docker/py38/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py38/project_structure.egg-info/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/var-docker/py39/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py39/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/var-docker/py39/.tox/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py39/.tox/.gitignore
-drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 09:10:40.284727 project-structure-0.8.29b1/var-docker/py39/project_structure.egg-info/
--rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-09 23:50:09.000000 project-structure-0.8.29b1/var-docker/py39/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      821 2023-05-10 12:18:58.000000 project-structure-0.8.30b0/.cz.toml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      643 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/.dir-locals.el.in
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1606 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/.dockerignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1418 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/.env.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.040652 project-structure-0.8.30b0/.github/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/.github/workflows/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4646 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/.github/workflows/build-test.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1606 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     6365 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/.gitlab-ci.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      877 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/.pre-commit-config.yaml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2472 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/.prospector.yaml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/.reuse/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      790 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/.reuse/dep5
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/.tox/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5411 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/CONTRIBUTING.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4942 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/Dockerfile
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/LICENSES/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1071 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/LICENSES/MIT.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    60300 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/Makefile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      140 2023-05-10 12:18:56.000000 project-structure-0.8.30b0/NEWS-VERSION.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    14397 2023-05-10 12:18:57.000000 project-structure-0.8.30b0/NEWS.rst
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17856 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/PKG-INFO
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)    16758 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/README.rst
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4388 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/TODO.rst
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/bin/
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2860 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/bin/cz-check-bump
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1052 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/bin/entrypoint
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1202 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/bin/get-base-version
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)      422 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/bin/hadolint
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     1521 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/bin/host-install
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/build-host/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2264 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/Dockerfile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1584 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/Makefile
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      849 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/README.rst
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/build-host/bin/
+-rwxrwxrwx   0 project-structure  (1001) project-structure  (1001)     2152 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/bin/entrypoint
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      730 2023-05-10 12:19:13.000000 project-structure-0.8.30b0/build-host/requirements-py310.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      673 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/requirements-py311.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      947 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/requirements-py37.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/requirements-py38.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      728 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/requirements-py39.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      104 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/build-host/requirements.txt.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/dist/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      222 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/dist/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5301 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/docker-compose.override.yml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      741 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/docker-compose.yml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/gitlab-runner/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/gitlab-runner/config/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1423 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      666 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/home/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      246 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/home/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      427 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/home/.pypirc.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/newsfragments/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      187 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/newsfragments/.gitignore
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1862 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/pyproject.toml
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/requirements/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      679 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/requirements/build.txt.in
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/requirements/py310/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/requirements/py310/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4720 2023-05-10 12:19:13.000000 project-structure-0.8.30b0/requirements/py310/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      864 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py310/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      257 2023-05-10 12:19:13.000000 project-structure-0.8.30b0/requirements/py310/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/requirements/py311/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2382 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/requirements/py311/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4548 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py311/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      749 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py311/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      264 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py311/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/requirements/py37/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2659 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/requirements/py37/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     5138 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py37/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1072 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py37/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      399 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py37/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/requirements/py38/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2502 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/requirements/py38/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4760 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py38/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py38/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py38/user.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/requirements/py39/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     2380 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/requirements/py39/build.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4747 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py39/devel.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      862 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py39/test.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      262 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/requirements/py39/user.txt
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     1705 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/setup.cfg
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/src/
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.044652 project-structure-0.8.30b0/src/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/src/project_structure.egg-info/.gitignore
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)    17856 2023-05-10 12:23:33.000000 project-structure-0.8.30b0/src/project_structure.egg-info/PKG-INFO
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)     2597 2023-05-10 12:23:33.000000 project-structure-0.8.30b0/src/project_structure.egg-info/SOURCES.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)        1 2023-05-10 12:23:33.000000 project-structure-0.8.30b0/src/project_structure.egg-info/dependency_links.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)       60 2023-05-10 12:23:33.000000 project-structure-0.8.30b0/src/project_structure.egg-info/entry_points.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)      151 2023-05-10 12:23:33.000000 project-structure-0.8.30b0/src/project_structure.egg-info/requires.txt
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)       17 2023-05-10 12:23:33.000000 project-structure-0.8.30b0/src/project_structure.egg-info/top_level.txt
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/src/projectstructure/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4356 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/src/projectstructure/__init__.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      303 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/src/projectstructure/__main__.py
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/src/projectstructure/tests/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      165 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/src/projectstructure/tests/__init__.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     4457 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/src/projectstructure/tests/test_cli.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      495 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/src/projectstructure/utils.py
+-rw-r--r--   0 project-structure  (1001) project-structure  (1001)      164 2023-05-10 12:23:33.000000 project-structure-0.8.30b0/src/projectstructure/version.py
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      281 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/towncrier.toml
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)     3652 2023-05-10 12:14:06.000000 project-structure-0.8.30b0/tox.ini
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      229 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py310/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py310/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py310/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py310/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py310/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py310/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py311/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py311/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py311/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py311/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py311/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py311/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py37/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py37/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py37/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py37/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py37/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py37/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py38/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py38/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py38/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py38/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py38/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py38/project_structure.egg-info/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py39/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py39/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py39/.tox/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py39/.tox/.gitignore
+drwxr-xr-x   0 project-structure  (1001) project-structure  (1001)        0 2023-05-10 12:23:33.048652 project-structure-0.8.30b0/var-docker/py39/project_structure.egg-info/
+-rw-rw-rw-   0 project-structure  (1001) project-structure  (1001)      192 2023-05-10 11:46:40.000000 project-structure-0.8.30b0/var-docker/py39/project_structure.egg-info/.gitignore
```

### Comparing `project-structure-0.8.29b1/.cz.toml` & `project-structure-0.8.30b0/.cz.toml`

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
-version = "0.8.29b1"
+version = "0.8.30b0"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `project-structure-0.8.29b1/.dir-locals.el.in` & `project-structure-0.8.30b0/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/.dockerignore` & `project-structure-0.8.30b0/.dockerignore`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 # SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
 #
 # SPDX-License-Identifier: MIT
 
 # Backup files
 *~
 **/*~
-*.rej
-**/*.rej
 
 # Byte-compiled / optimized / DLL files
 __pycache__
 **/__pycache__
 *.py[cod]
 **/*.py[cod]
 *$py.class
 **/*$py.class
 
 # C extensions
 *.so
 **/.so
 
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 downloads/
 eggs/
```

### Comparing `project-structure-0.8.29b1/.env.in` & `project-structure-0.8.30b0/.env.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/.github/workflows/build-test.yml` & `project-structure-0.8.30b0/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/.gitignore` & `project-structure-0.8.30b0/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 # SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
 #
 # SPDX-License-Identifier: MIT
 
 # Backup files
 *~
 **/*~
-*.rej
-**/*.rej
 
 # Byte-compiled / optimized / DLL files
 __pycache__
 **/__pycache__
 *.py[cod]
 **/*.py[cod]
 *$py.class
 **/*$py.class
 
 # C extensions
 *.so
 **/.so
 
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 downloads/
 eggs/
```

### Comparing `project-structure-0.8.29b1/.gitlab-ci.yml` & `project-structure-0.8.30b0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/.pre-commit-config.yaml` & `project-structure-0.8.30b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/.prospector.yaml` & `project-structure-0.8.30b0/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/.reuse/dep5` & `project-structure-0.8.30b0/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/CONTRIBUTING.rst` & `project-structure-0.8.30b0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/Dockerfile` & `project-structure-0.8.30b0/Dockerfile`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/LICENSES/MIT.txt` & `project-structure-0.8.30b0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/Makefile` & `project-structure-0.8.30b0/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -924,15 +924,16 @@
 	    --copyright "Ross Patterson <me@rpatterson.net>" --license "MIT" "./"
 
 .PHONY: devel-upgrade
 ### Update all fixed/pinned dependencies to their latest available versions.
 devel-upgrade: ./.env.~out~ $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
 		build-docker
 	touch "./setup.cfg" "./requirements/build.txt.in" \
-	    "./build-host/requirements.txt.in"
+	    "./build-host/requirements.txt.in" \
+	    "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
 # Ensure the network is create first to avoid race conditions
 	docker compose create $(PROJECT_NAME)-devel
 	$(MAKE) -e -j PIP_COMPILE_ARGS="--upgrade" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=build-docker-requirements-%)
 # Update VCS hooks from remotes to the latest tag.
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit autoupdate
```

### Comparing `project-structure-0.8.29b1/NEWS.rst` & `project-structure-0.8.30b0/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+project-structure 0.8.30b0 (2023-05-10)
+=======================================
+
+Bugfixes
+--------
+
+- Simulate a patch release. (simulate)
+
+
+project-structure 0.8.29 (2023-05-10)
+=====================================
+
+No significant changes.
+
+
 project-structure 0.8.29b1 (2023-05-10)
 =======================================
 
 Bugfixes
 --------
 
 - Simulate a patch release. (simulate)
```

### Comparing `project-structure-0.8.29b1/PKG-INFO` & `project-structure-0.8.30b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-structure
-Version: 0.8.29b1
+Version: 0.8.30b0
 Summary: Project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: devel
 
 .. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
```

### Comparing `project-structure-0.8.29b1/README.rst` & `project-structure-0.8.30b0/README.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/TODO.rst` & `project-structure-0.8.30b0/TODO.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/bin/cz-check-bump` & `project-structure-0.8.30b0/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/bin/entrypoint` & `project-structure-0.8.30b0/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/bin/get-base-version` & `project-structure-0.8.30b0/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/bin/host-install` & `project-structure-0.8.30b0/bin/host-install`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     then
         sudo apt-get update
         sudo apt-get install -y "gettext-base" "python3-pip" "docker-compose-plugin" \
             "gnupg" "gh" "curl"
     else
         set +x
         echo "ERROR: OS not supported for installing host dependencies"
+        # TODO: Add OS-X/Darwin support.
         false
     fi
     if [ -e ./build-host/requirements-$(PYTHON_HOST_ENV).txt ]
     then
         pip3 install -r "./build-host/requirements-$(PYTHON_HOST_ENV).txt"
     else
         pip3 install -r "./build-host/requirements.txt.in"
```

### Comparing `project-structure-0.8.29b1/build-host/Dockerfile` & `project-structure-0.8.30b0/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/build-host/Makefile` & `project-structure-0.8.30b0/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/build-host/README.rst` & `project-structure-0.8.30b0/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/build-host/bin/entrypoint` & `project-structure-0.8.30b0/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/build-host/requirements-py310.txt` & `project-structure-0.8.30b0/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/build-host/requirements-py311.txt` & `project-structure-0.8.30b0/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/build-host/requirements-py37.txt` & `project-structure-0.8.30b0/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/build-host/requirements-py38.txt` & `project-structure-0.8.30b0/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/build-host/requirements-py39.txt` & `project-structure-0.8.30b0/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/docker-compose.override.yml` & `project-structure-0.8.30b0/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/docker-compose.yml` & `project-structure-0.8.30b0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/gitlab-runner/config/config.toml.in` & `project-structure-0.8.30b0/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/gitlab-runner/docker-compose.yml` & `project-structure-0.8.30b0/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/pyproject.toml` & `project-structure-0.8.30b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/build.txt.in` & `project-structure-0.8.30b0/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py310/build.txt` & `project-structure-0.8.30b0/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py310/devel.txt` & `project-structure-0.8.30b0/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py310/test.txt` & `project-structure-0.8.30b0/requirements/py310/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py311/build.txt` & `project-structure-0.8.30b0/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py311/devel.txt` & `project-structure-0.8.30b0/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py311/test.txt` & `project-structure-0.8.30b0/requirements/py311/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py37/build.txt` & `project-structure-0.8.30b0/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py37/devel.txt` & `project-structure-0.8.30b0/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py37/test.txt` & `project-structure-0.8.30b0/requirements/py37/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py38/build.txt` & `project-structure-0.8.30b0/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py38/devel.txt` & `project-structure-0.8.30b0/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py38/test.txt` & `project-structure-0.8.30b0/requirements/py38/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py39/build.txt` & `project-structure-0.8.30b0/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py39/devel.txt` & `project-structure-0.8.30b0/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/requirements/py39/test.txt` & `project-structure-0.8.30b0/requirements/py39/test.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/setup.cfg` & `project-structure-0.8.30b0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3 :: Only
 	Topic :: Utilities
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
```

### Comparing `project-structure-0.8.29b1/src/project_structure.egg-info/PKG-INFO` & `project-structure-0.8.30b0/src/project_structure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-structure
-Version: 0.8.29b1
+Version: 0.8.30b0
 Summary: Project structure foundation or template, CLI console scripts.
 Home-page: https://gitlab.com/rpatterson/project-structure
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: template,structure
 Classifier: Development Status :: 4 - Beta
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: devel
 
 .. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
```

### Comparing `project-structure-0.8.29b1/src/project_structure.egg-info/SOURCES.txt` & `project-structure-0.8.30b0/src/project_structure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/src/projectstructure/__init__.py` & `project-structure-0.8.30b0/src/projectstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/src/projectstructure/tests/test_cli.py` & `project-structure-0.8.30b0/src/projectstructure/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `project-structure-0.8.29b1/tox.ini` & `project-structure-0.8.30b0/tox.ini`

 * *Files identical despite different names*

