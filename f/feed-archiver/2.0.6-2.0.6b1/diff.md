# Comparing `tmp/feed-archiver-2.0.6.tar.gz` & `tmp/feed-archiver-2.0.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-2.0.6.tar", last modified: Wed May 10 13:18:22 2023, max compression
+gzip compressed data, was "feed-archiver-2.0.6b1.tar", last modified: Wed May 10 11:39:18 2023, max compression
```

## Comparing `feed-archiver-2.0.6.tar` & `feed-archiver-2.0.6b1.tar`

### file list

```diff
@@ -1,296 +1,296 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      675 2023-05-10 12:46:18.000000 feed-archiver-2.0.6/.cz.toml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      643 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1842 2023-05-10 12:40:08.000000 feed-archiver-2.0.6/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1609 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4073 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/.github/workflows/build-test.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1842 2023-05-10 12:40:08.000000 feed-archiver-2.0.6/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4532 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/.gitlab-ci.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      877 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2543 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/.prospector.yaml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/.reuse/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1011 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/.reuse/dep5
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/.tox/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/.tox/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5403 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4955 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/Dockerfile
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/LICENSES/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1071 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/LICENSES/MIT.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    60694 2023-05-10 12:40:08.000000 feed-archiver-2.0.6/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-05-10 12:46:18.000000 feed-archiver-2.0.6/NEWS-VERSION.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5298 2023-05-10 12:46:18.000000 feed-archiver-2.0.6/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26298 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/PKG-INFO
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    25157 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3861 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2860 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/bin/cz-check-bump
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1040 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/bin/entrypoint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1202 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/bin/get-base-version
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      422 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/bin/hadolint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1521 2023-05-10 12:40:08.000000 feed-archiver-2.0.6/bin/host-install
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/build-host/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2228 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/build-host/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1576 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/build-host/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      849 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/build-host/README.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/build-host/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2148 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/build-host/bin/entrypoint
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/build-host/requirements-py310.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/build-host/requirements-py311.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/build-host/requirements-py37.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/build-host/requirements-py38.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/build-host/requirements-py39.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      104 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/build-host/requirements.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/dist/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      222 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/dist/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1054 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/docker-compose-servarr.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6217 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1167 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/gitlab-runner/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/gitlab-runner/config/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1423 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      666 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      246 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      427 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/home/.pypirc.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      187 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/newsfragments/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/nginx/templates/default.conf.template
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2320 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/pyproject.toml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/requirements/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      679 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/requirements/build.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/requirements/py310/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2382 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/requirements/py310/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5616 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py310/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2073 2023-05-10 11:16:51.000000 feed-archiver-2.0.6/requirements/py310/test.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1137 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py310/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/requirements/py311/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2382 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/requirements/py311/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5444 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py311/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1958 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/requirements/py311/test.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1137 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py311/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/requirements/py37/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2659 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/requirements/py37/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6224 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py37/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2493 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/requirements/py37/test.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1485 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py37/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/requirements/py38/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2502 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/requirements/py38/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5791 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py38/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2206 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/requirements/py38/test.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1270 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py38/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/requirements/py39/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2380 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/requirements/py39/build.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5778 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py39/devel.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2206 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/requirements/py39/test.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1270 2023-05-10 11:09:34.000000 feed-archiver-2.0.6/requirements/py39/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4497 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2207 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feed_archiver.egg-info/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/src/feed_archiver.egg-info/.gitignore
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26298 2023-05-10 13:18:22.000000 feed-archiver-2.0.6/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     8097 2023-05-10 13:18:22.000000 feed-archiver-2.0.6/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-05-10 13:18:22.000000 feed-archiver-2.0.6/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-05-10 13:18:22.000000 feed-archiver-2.0.6/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      382 2023-05-10 13:18:22.000000 feed-archiver-2.0.6/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-05-10 13:18:22.000000 feed-archiver-2.0.6/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5388 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      303 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11902 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/archive.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/enclosures/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3457 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/src/feedarchiver/enclosures/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8255 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/enclosures/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2068 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/enclosures/template.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    35025 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7174 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9960 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/empty/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/archives/empty/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/empty-feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/empty-items/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/relink/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/relink-wo-suffix/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/empty-items/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/empty-items/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/empty-items/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.371156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.375156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3386 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4357 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10933 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15151 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7536 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2265 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8247 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      160 2023-05-10 13:18:22.000000 feed-archiver-2.0.6/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      273 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/towncrier.toml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3632 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/tox.ini
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/var/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/var-docker/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      229 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/var-docker/py310/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py310/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/var-docker/py310/.tox/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py310/.tox/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/var-docker/py310/feed_archiver.egg-info/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/var-docker/py310/feed_archiver.egg-info/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/var-docker/py311/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py311/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.379156 feed-archiver-2.0.6/var-docker/py311/.tox/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py311/.tox/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py311/feed_archiver.egg-info/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/var-docker/py311/feed_archiver.egg-info/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py37/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py37/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py37/.tox/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py37/.tox/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py37/feed_archiver.egg-info/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/var-docker/py37/feed_archiver.egg-info/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py38/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py38/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py38/.tox/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py38/.tox/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py38/feed_archiver.egg-info/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/var-docker/py38/feed_archiver.egg-info/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py39/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py39/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py39/.tox/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6/var-docker/py39/.tox/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 13:18:22.383157 feed-archiver-2.0.6/var-docker/py39/feed_archiver.egg-info/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6/var-docker/py39/feed_archiver.egg-info/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      677 2023-05-10 11:09:18.000000 feed-archiver-2.0.6b1/.cz.toml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      643 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/.dir-locals.el.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1953 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/.dockerignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1609 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/.env.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.699964 feed-archiver-2.0.6b1/.github/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/.github/workflows/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4073 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/.github/workflows/build-test.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1953 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4532 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/.gitlab-ci.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      877 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/.pre-commit-config.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2543 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/.prospector.yaml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/.reuse/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1011 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/.reuse/dep5
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/.tox/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/.tox/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5403 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/CONTRIBUTING.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4955 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/Dockerfile
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/LICENSES/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1071 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/LICENSES/MIT.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    60629 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      259 2023-05-10 11:09:15.000000 feed-archiver-2.0.6b1/NEWS-VERSION.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5205 2023-05-10 11:09:17.000000 feed-archiver-2.0.6b1/NEWS.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26244 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/PKG-INFO
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    25157 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/README.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3861 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/TODO.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2860 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/bin/cz-check-bump
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1040 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/bin/entrypoint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1202 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/bin/get-base-version
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      422 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/bin/hadolint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1480 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/bin/host-install
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/build-host/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2228 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/build-host/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1576 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/build-host/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      849 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/build-host/README.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/build-host/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2148 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/build-host/bin/entrypoint
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/build-host/requirements-py310.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/build-host/requirements-py311.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/build-host/requirements-py37.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/build-host/requirements-py38.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/build-host/requirements-py39.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      104 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/build-host/requirements.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/dist/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      222 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/dist/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1054 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/docker-compose-servarr.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6217 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/docker-compose.override.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1167 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/gitlab-runner/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/gitlab-runner/config/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1423 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      666 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/home/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      246 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/home/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      427 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/home/.pypirc.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      187 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/newsfragments/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.699964 feed-archiver-2.0.6b1/nginx/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/nginx/templates/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/nginx/templates/default.conf.template
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2320 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/pyproject.toml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/requirements/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      679 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/requirements/build.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/requirements/py310/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2382 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/requirements/py310/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5616 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py310/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2073 2023-05-10 11:16:51.000000 feed-archiver-2.0.6b1/requirements/py310/test.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1137 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py310/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/requirements/py311/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2382 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/requirements/py311/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5444 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py311/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1958 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/requirements/py311/test.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1137 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py311/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/requirements/py37/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2659 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/requirements/py37/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     6224 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py37/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2493 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/requirements/py37/test.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1485 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py37/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/requirements/py38/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2502 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/requirements/py38/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5791 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py38/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2206 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/requirements/py38/test.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1270 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py38/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/requirements/py39/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2380 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/requirements/py39/build.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5778 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py39/devel.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2206 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/requirements/py39/test.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1270 2023-05-10 11:09:34.000000 feed-archiver-2.0.6b1/requirements/py39/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/server/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4497 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/server/docker-compose.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2162 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/setup.cfg
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.699964 feed-archiver-2.0.6b1/src/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feed_archiver.egg-info/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/src/feed_archiver.egg-info/.gitignore
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26244 2023-05-10 11:39:18.000000 feed-archiver-2.0.6b1/src/feed_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     8097 2023-05-10 11:39:18.000000 feed-archiver-2.0.6b1/src/feed_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-05-10 11:39:18.000000 feed-archiver-2.0.6b1/src/feed_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-05-10 11:39:18.000000 feed-archiver-2.0.6b1/src/feed_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      382 2023-05-10 11:39:18.000000 feed-archiver-2.0.6b1/src/feed_archiver.egg-info/requires.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-05-10 11:39:18.000000 feed-archiver-2.0.6b1/src/feed_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5388 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      303 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/__main__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11902 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/archive.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/enclosures/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3457 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/src/feedarchiver/enclosures/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8255 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/enclosures/servarr.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2068 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/enclosures/template.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    35025 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7174 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/formats.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9960 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/__init__.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.699964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/downloads/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/empty/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/empty/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/empty-feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/empty-items/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/end-to-end/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/relink/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/relink-wo-suffix/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/simple/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.699964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.699964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.699964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.699964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.707964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/empty-items/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/empty-items/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/empty-items/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.703964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3386 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/test_archive.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4357 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/test_cli.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10933 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/test_download.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15151 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/test_feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7536 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/test_linking.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2265 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/tests/test_urls.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8247 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/src/feedarchiver/utils.py
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      162 2023-05-10 11:39:18.000000 feed-archiver-2.0.6b1/src/feedarchiver/version.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      273 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/towncrier.toml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3632 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/tox.ini
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      229 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py310/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py310/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py310/.tox/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py310/.tox/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py310/feed_archiver.egg-info/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/var-docker/py310/feed_archiver.egg-info/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py311/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py311/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py311/.tox/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py311/.tox/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py311/feed_archiver.egg-info/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/var-docker/py311/feed_archiver.egg-info/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py37/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py37/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py37/.tox/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py37/.tox/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py37/feed_archiver.egg-info/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/var-docker/py37/feed_archiver.egg-info/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py38/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py38/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py38/.tox/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py38/.tox/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py38/feed_archiver.egg-info/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/var-docker/py38/feed_archiver.egg-info/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py39/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py39/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py39/.tox/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-09 12:05:05.000000 feed-archiver-2.0.6b1/var-docker/py39/.tox/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-05-10 11:39:18.711964 feed-archiver-2.0.6b1/var-docker/py39/feed_archiver.egg-info/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      192 2023-05-10 11:08:23.000000 feed-archiver-2.0.6b1/var-docker/py39/feed_archiver.egg-info/.gitignore
```

### Comparing `feed-archiver-2.0.6/.cz.toml` & `feed-archiver-2.0.6b1/.cz.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "2.0.6"
+version = "2.0.6b1"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `feed-archiver-2.0.6/.dir-locals.el.in` & `feed-archiver-2.0.6b1/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/.dockerignore` & `feed-archiver-2.0.6b1/.dockerignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
 #
 # SPDX-License-Identifier: MIT
 
 # Backup files
 *~
 **/*~
+*.rej
+**/*.rej
 
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
 
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 downloads/
 eggs/
```

### Comparing `feed-archiver-2.0.6/.env.in` & `feed-archiver-2.0.6b1/.env.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/.github/workflows/build-test.yml` & `feed-archiver-2.0.6b1/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/.gitignore` & `feed-archiver-2.0.6b1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
 #
 # SPDX-License-Identifier: MIT
 
 # Backup files
 *~
 **/*~
+*.rej
+**/*.rej
 
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
 
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 downloads/
 eggs/
```

### Comparing `feed-archiver-2.0.6/.gitlab-ci.yml` & `feed-archiver-2.0.6b1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/.pre-commit-config.yaml` & `feed-archiver-2.0.6b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/.prospector.yaml` & `feed-archiver-2.0.6b1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/.reuse/dep5` & `feed-archiver-2.0.6b1/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/CONTRIBUTING.rst` & `feed-archiver-2.0.6b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/Dockerfile` & `feed-archiver-2.0.6b1/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/LICENSES/MIT.txt` & `feed-archiver-2.0.6b1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/Makefile` & `feed-archiver-2.0.6b1/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -937,16 +937,15 @@
 	    --copyright "Ross Patterson <me@rpatterson.net>" --license "MIT" "./"
 
 .PHONY: devel-upgrade
 ### Update all fixed/pinned dependencies to their latest available versions.
 devel-upgrade: ./.env.~out~ $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
 		build-docker
 	touch "./setup.cfg" "./requirements/build.txt.in" \
-	    "./build-host/requirements.txt.in" \
-	    "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
+	    "./build-host/requirements.txt.in"
 # Ensure the network is create first to avoid race conditions
 	docker compose create $(PROJECT_NAME)-devel
 	$(MAKE) -e -j PIP_COMPILE_ARGS="--upgrade" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=build-docker-requirements-%)
 # Update VCS hooks from remotes to the latest tag.
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit autoupdate
```

### Comparing `feed-archiver-2.0.6/NEWS.rst` & `feed-archiver-2.0.6b1/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-feed-archiver 2.0.6 (2023-05-10)
-================================
-
-No significant changes.
-
-
 feed-archiver 2.0.6b1 (2023-05-10)
 ==================================
 
 Bugfixes
 --------
 
 - Restore Python 3.7 compatibility following a dependency upgrade in v2.0.1b0.
```

### Comparing `feed-archiver-2.0.6/PKG-INFO` & `feed-archiver-2.0.6b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.6
+Version: 2.0.6b1
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: devel
 
 .. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
```

### Comparing `feed-archiver-2.0.6/README.rst` & `feed-archiver-2.0.6b1/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/TODO.rst` & `feed-archiver-2.0.6b1/TODO.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/bin/cz-check-bump` & `feed-archiver-2.0.6b1/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/bin/entrypoint` & `feed-archiver-2.0.6b1/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/bin/get-base-version` & `feed-archiver-2.0.6b1/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/bin/host-install` & `feed-archiver-2.0.6b1/bin/host-install`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     then
         sudo apt-get update
         sudo apt-get install -y "gettext-base" "python3-pip" "docker-compose-plugin" \
             "gnupg" "gh" "curl"
     else
         set +x
         echo "ERROR: OS not supported for installing host dependencies"
-        # TODO: Add OS-X/Darwin support.
         false
     fi
     if [ -e ./build-host/requirements-$(PYTHON_HOST_ENV).txt ]
     then
         pip3 install -r "./build-host/requirements-$(PYTHON_HOST_ENV).txt"
     else
         pip3 install -r "./build-host/requirements.txt.in"
```

### Comparing `feed-archiver-2.0.6/build-host/Dockerfile` & `feed-archiver-2.0.6b1/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/build-host/Makefile` & `feed-archiver-2.0.6b1/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/build-host/README.rst` & `feed-archiver-2.0.6b1/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/build-host/bin/entrypoint` & `feed-archiver-2.0.6b1/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/build-host/requirements-py310.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/build-host/requirements-py311.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/build-host/requirements-py37.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/build-host/requirements-py38.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/build-host/requirements-py39.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/docker-compose-servarr.yml` & `feed-archiver-2.0.6b1/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/docker-compose.override.yml` & `feed-archiver-2.0.6b1/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/docker-compose.yml` & `feed-archiver-2.0.6b1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/gitlab-runner/config/config.toml.in` & `feed-archiver-2.0.6b1/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/gitlab-runner/docker-compose.yml` & `feed-archiver-2.0.6b1/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/nginx/templates/default.conf.template` & `feed-archiver-2.0.6b1/nginx/templates/default.conf.template`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/pyproject.toml` & `feed-archiver-2.0.6b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/build.txt.in` & `feed-archiver-2.0.6b1/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py310/build.txt` & `feed-archiver-2.0.6b1/requirements/py310/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py310/devel.txt` & `feed-archiver-2.0.6b1/requirements/py310/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py310/test.txt` & `feed-archiver-2.0.6b1/requirements/py310/test.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py310/user.txt` & `feed-archiver-2.0.6b1/requirements/py310/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py311/build.txt` & `feed-archiver-2.0.6b1/requirements/py311/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py311/devel.txt` & `feed-archiver-2.0.6b1/requirements/py311/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py311/test.txt` & `feed-archiver-2.0.6b1/requirements/py311/test.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py311/user.txt` & `feed-archiver-2.0.6b1/requirements/py311/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py37/build.txt` & `feed-archiver-2.0.6b1/requirements/py37/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py37/devel.txt` & `feed-archiver-2.0.6b1/requirements/py37/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py37/test.txt` & `feed-archiver-2.0.6b1/requirements/py37/test.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py37/user.txt` & `feed-archiver-2.0.6b1/requirements/py37/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py38/build.txt` & `feed-archiver-2.0.6b1/requirements/py38/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py38/devel.txt` & `feed-archiver-2.0.6b1/requirements/py38/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py38/test.txt` & `feed-archiver-2.0.6b1/requirements/py38/test.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py38/user.txt` & `feed-archiver-2.0.6b1/requirements/py38/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py39/build.txt` & `feed-archiver-2.0.6b1/requirements/py39/build.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py39/devel.txt` & `feed-archiver-2.0.6b1/requirements/py39/devel.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py39/test.txt` & `feed-archiver-2.0.6b1/requirements/py39/test.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/requirements/py39/user.txt` & `feed-archiver-2.0.6b1/requirements/py39/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/server/docker-compose.yml` & `feed-archiver-2.0.6b1/server/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/setup.cfg` & `feed-archiver-2.0.6b1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3 :: Only
 	Topic :: Utilities
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
```

### Comparing `feed-archiver-2.0.6/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-2.0.6b1/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.6
+Version: 2.0.6b1
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: devel
 
 .. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
```

### Comparing `feed-archiver-2.0.6/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-2.0.6b1/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/__init__.py` & `feed-archiver-2.0.6b1/src/feedarchiver/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/archive.py` & `feed-archiver-2.0.6b1/src/feedarchiver/archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/enclosures/__init__.py` & `feed-archiver-2.0.6b1/src/feedarchiver/enclosures/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/enclosures/servarr.py` & `feed-archiver-2.0.6b1/src/feedarchiver/enclosures/servarr.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/enclosures/template.py` & `feed-archiver-2.0.6b1/src/feedarchiver/enclosures/template.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/feed.py` & `feed-archiver-2.0.6b1/src/feedarchiver/feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/formats.py` & `feed-archiver-2.0.6b1/src/feedarchiver/formats.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/__init__.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/archives/relink/.feed-archiver.yml` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/relink/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/test_archive.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/test_cli.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/test_download.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/test_feed.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/test_linking.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/tests/test_urls.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/src/feedarchiver/utils.py` & `feed-archiver-2.0.6b1/src/feedarchiver/utils.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.6/tox.ini` & `feed-archiver-2.0.6b1/tox.ini`

 * *Files identical despite different names*

