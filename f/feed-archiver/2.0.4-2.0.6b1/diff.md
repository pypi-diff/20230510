# Comparing `tmp/feed-archiver-2.0.4.tar.gz` & `tmp/feed-archiver-2.0.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-2.0.4.tar", last modified: Sat Apr 29 16:41:33 2023, max compression
+gzip compressed data, was "feed-archiver-2.0.6b1.tar", last modified: Wed May 10 11:39:18 2023, max compression
```

## Comparing `feed-archiver-2.0.4.tar` & `feed-archiver-2.0.6b1.tar`

### file list

```diff
@@ -1,250 +1,296 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1150 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/.github/workflows/build-test.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/.gitignore
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     4357 2023-04-26 22:06:34.000000 feed-archiver-2.0.4/.gitlab-ci.yml
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      777 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/.prospector.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2481 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3218 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/Dockerfile.devel
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/LICENSE
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    60319 2023-04-26 22:06:34.000000 feed-archiver-2.0.4/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      173 2023-04-29 16:13:44.000000 feed-archiver-2.0.4/NEWS-VERSION.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4475 2023-04-29 16:13:44.000000 feed-archiver-2.0.4/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26172 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/PKG-INFO
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    25086 2023-04-29 09:13:48.000000 feed-archiver-2.0.4/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2759 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/bin/cz-check-bump
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/bin/entrypoint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/bin/get-base-version
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/bin/hadolint
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/build-host/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/build-host/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/build-host/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/build-host/README.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/build-host/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/build-host/bin/entrypoint
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py310.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py311.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py37.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py38.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py39.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-29 16:01:58.000000 feed-archiver-2.0.4/build-host/requirements.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/dist/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/dist/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/docker-compose-servarr.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5769 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      945 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/gitlab-runner/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/gitlab-runner/config/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      566 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/home/.pypirc.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/link-fallbacks.feature.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/nginx/templates/default.conf.template
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2938 2023-04-29 16:13:44.000000 feed-archiver-2.0.4/pyproject.toml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      668 2023-04-29 16:01:58.000000 feed-archiver-2.0.4/requirements/build.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py310/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2567 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py310/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6244 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py310/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-29 16:02:19.000000 feed-archiver-2.0.4/requirements/py310/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py311/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2529 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py311/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6018 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py311/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-29 16:03:05.000000 feed-archiver-2.0.4/requirements/py311/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py37/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2840 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py37/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6934 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py37/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-29 16:03:20.000000 feed-archiver-2.0.4/requirements/py37/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py38/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2668 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py38/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6284 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py38/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-29 16:03:09.000000 feed-archiver-2.0.4/requirements/py38/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py39/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2565 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py39/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6271 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py39/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-29 16:03:18.000000 feed-archiver-2.0.4/requirements/py39/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2152 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feed_archiver.egg-info/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26172 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7317 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/archive.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/enclosures/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/enclosures/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/enclosures/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/enclosures/template.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/newsfragments/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty-feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty-items/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink-wo-suffix/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      160 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3368 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/tox.ini
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

### Comparing `feed-archiver-2.0.4/.dockerignore` & `feed-archiver-2.0.6b1/.dockerignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Backup files
 *~
 **/*~
 *.rej
 **/*.rej
 
 # Byte-compiled / optimized / DLL files
@@ -12,27 +16,37 @@
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
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
-var/
+/var
+/var-docker
+/README.md
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
 
@@ -93,15 +107,15 @@
 # pyenv
 .python-version
 
 # celery beat schedule file
 celerybeat-schedule
 
 # dotenv
-.env
+/.env
 
 # virtualenv
 venv/
 ENV/
 
 # Spyder project settings
 .spyderproject
```

### Comparing `feed-archiver-2.0.4/.env.in` & `feed-archiver-2.0.6b1/.env.in`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,37 @@
-# Make non-default `./docker-compose*.yml` files the default
-# https://pscheit.medium.com/docker-compose-advanced-configuration-541356d121de#9aa6
-COMPOSE_PATH_SEPARATOR=:
-COMPOSE_FILE=./docker-compose.yml:./gitlab-runner/docker-compose.yml:./docker-compose-servarr.yml:./server/docker-compose.yml:./docker-compose.override.yml
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
 
-# Capture local values specific to this checkout
+# Capture local values specific to this checkout:
 TZ=${TZ}
 PUID=${PUID}
 PGID=${PGID}
-# Absolute path of the git repo checkout, useful where relative paths can't be used
-CHECKOUT_DIR=${CHECKOUT_DIR}
+FEED_ARCHIVE=$${__}{CHECKOUT_DIR}/src/feedarchiver/tests/archives/end-to-end
+NGINX_ROOT=$${__}{FEED_ARCHIVE}
+NGINX_PORT=${NGINX_PORT}
 
-# Release variables
-DOCKER_USER=${DOCKER_USER}
+# Release Secrets:
 # Best to create and use a token.  Note that the token must have the `admin`/"Read,
 # Write, Delete" scope, aka "ACCESS PERMISSIONS":
 # https://hub.docker.com/settings/security?generateToken=true
 DOCKER_PASS=${DOCKER_PASS}
 # Project host credentials used here and in CI/CD to support local testing/debugging:
 CI_REGISTRY_PASSWORD=${CI_REGISTRY_PASSWORD}
 PROJECT_GITHUB_PAT=${PROJECT_GITHUB_PAT}
 
-# Define common, shared values in one location
-FEED_ARCHIVE=$${__}{CHECKOUT_DIR}/src/feedarchiver/tests/archives/end-to-end
-NGINX_ROOT=$${__}{FEED_ARCHIVE}
-NGINX_PORT=${NGINX_PORT}
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
+COMPOSE_FILE=./docker-compose.yml:./gitlab-runner/docker-compose.yml:./docker-compose-servarr.yml:./server/docker-compose.yml:./docker-compose.override.yml
+# Build host variables, used only for reproducing CI/CD locally:
+DOCKER_GID=${DOCKER_GID}
```

### Comparing `feed-archiver-2.0.4/.github/workflows/build-test.yml` & `feed-archiver-2.0.6b1/.github/workflows/build-test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,38 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 name: "Build and Test"
 
+env:
+  PUID: "1001"
+  PGID: "123"
+  # Project specific values:
+  PROJECT_NAMESPACE: "rpatterson"
+  PROJECT_NAME: "feed-archiver"
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
@@ -14,35 +43,15 @@
 jobs:
 
   build-test:
     runs-on: "ubuntu-latest"
     container:
       image: "ghcr.io/rpatterson/feed-archiver:build-host"
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
           - "3.11"
@@ -74,32 +83,35 @@
       # Upload build artifacts:
       # https://github.com/actions/upload-artifact#usage
       - name: "Archive test suite reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "test-suite-reports"
           path: |
-            ./build/*/pytest*
+            ./build/*test*
       # https://github.com/marketplace/actions/test-reporter#example
       - name: "Publish test suite report"
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
-          name: "PyTest Test Suite (python${{ matrix.PYTHON_MINORS }})"
+          name: "Test Suite Reports"
           path: >-
-            ./build/*/pytest-junit.xml,
+            ./build/*/*test-junit.xml,
             ./build/*/prospector-xunit.xml
           reporter: "java-junit"
       - name: "Archive code coverage reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "code-coverage-reports"
           path: |
@@ -107,9 +119,9 @@
             ./build/*/coverage*
             ./build/*/htmlcov*
       - name: "Archive linter reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "linter-reports"
           path: |
+            ./build/*/*lint*
             ./build/*/prospector*
-            ./build/*/pylint*
```

### Comparing `feed-archiver-2.0.4/.gitignore` & `feed-archiver-2.0.6b1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Backup files
 *~
 **/*~
 *.rej
 **/*.rej
 
 # Byte-compiled / optimized / DLL files
@@ -12,27 +16,37 @@
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
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
-var/
+/var
+/var-docker
+/README.md
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
 
@@ -93,15 +107,15 @@
 # pyenv
 .python-version
 
 # celery beat schedule file
 celerybeat-schedule
 
 # dotenv
-.env
+/.env
 
 # virtualenv
 venv/
 ENV/
 
 # Spyder project settings
 .spyderproject
```

### Comparing `feed-archiver-2.0.4/.gitlab-ci.yml` & `feed-archiver-2.0.6b1/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,33 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # https://gitlab.com/gitlab-org/gitlab/-/blob/master/lib/gitlab/ci/templates/Docker.gitlab-ci.yml
 
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
@@ -96,18 +102,18 @@
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
-      entrypoint make -e release-python test-clean
+      entrypoint make -e release-pkgs test-clean
   artifacts:
     paths:
       - "./dist/feed?archiver-*"
 
 merge-upgrade:
   stage: "merge-upgrade"
   needs: ["build-test"]
```

### Comparing `feed-archiver-2.0.4/.pre-commit-config.yaml` & `feed-archiver-2.0.6b1/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Run all test, linters and other code checks before committing and pushing.
 fail_fast: true
 repos:
 # Check commit message format and style before pushing to a remote
   - repo: "https://github.com/commitizen-tools/commitizen"
-    rev: "3.1.1"
+    rev: "3.2.1"
     hooks:
       - id: "commitizen"
 # Checks defined in the `./Makefile`
   - repo: "local"
     hooks:
 # Fail fast, run quicker checks first
     - id: "test-push"
       name: "test-push"
       stages: ["push"]
       entry: "make -e test-push"
-      language: "python"
+      language: "system"
       pass_filenames: false
 # Only run the longer running test check after everything else
     - id: "test"
       name: "test"
       stages: ["commit", "merge-commit", "push", "manual"]
       entry: "make -e test"
-      language: "python"
+      language: "system"
       pass_filenames: false
```

### Comparing `feed-archiver-2.0.4/.prospector.yaml` & `feed-archiver-2.0.6b1/.prospector.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # https://prospector.landscape.io/en/master/profiles.html#global-configuration-options
 strictness: "veryhigh"
 test-warnings: true
 doc-warnings: true
 member-warnings: true
 autodetect: false
 inherits:
@@ -21,15 +25,15 @@
   run: false
 # Deprecated in favor of PyFlakes:
 # https://github.com/timothycrosley/deprecated.frosted#important-note-frosted-is-deprecated-long-live-flake8
 # frosted:
 #   run: true
 # FIXME: I confirmed the package is installed but couldn't get to work:
 #     Cannot run tool pyroma as support was not installed.
-#     Please install by running 'pip install prospector[with_pyroma]'
+#     Please install by running 'pip3 install prospector[with_pyroma]'
 # pyroma:
 #   run: true
 
 pyflakes:
   disable:
     # Redundant with `pylint - unused-import`.
     # If a line disables that error with a `  # pylint: disable=unused-import` comment,
```

### Comparing `feed-archiver-2.0.4/CONTRIBUTING.rst` & `feed-archiver-2.0.6b1/CONTRIBUTING.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
+
 ########################################################################################
 Contributing
 ########################################################################################
 
 Development requires fairly standard development tools, but ``git`` and ``make`` to
 bootstrap the local development environment.  Once installed, clone the repository::
 
@@ -12,15 +16,15 @@
 
   $ make
 
 If there's not already `an issue/ticket`_ for the changes you'll be making, create one.
 Regardless, take note of the issue/ticket number, e.g. ``#123``.  Then create a
 branch/fork off of the ``develop`` branch::
 
-  $ git switch -c feat-123-foo-bar origin/develop
+  $ git switch -c feat-123-foo-bar --track origin/develop
 
 This project uses `towncrier`_ to manage it's release notes, AKA changelog and thus
 requires at least one `news fragment`_ before merging back into ``develop``.  The VCS
 hooks enforce this when pushing to ``develop`` or ``main``::
 
   $ towncrier create 123.feature
 
@@ -37,16 +41,32 @@
   $ make test-local
 
 You can also inspect test failures and errors in `Python's post-mortem debugger`_.  This
 also runs locally directly on your development host::
 
   $ make test-debug
 
-The ``$ make test`` target also runs the ``$ make format`` target to format code
-according to this project's guidelines and rules.
+The linters make various decisions on style, formatting, and conventions for you so you
+don't have to think about them and no one has to debate them.  They're enforced by ``$
+make test`` and the VCS hooks.  You may also use the same tools to apply all fixes and
+formatting that can be automated to format code according to this project's guidelines
+and rules::
+
+  $ make devel-format
+
+This project also uses `Reuse`_ to manage licenses and copyright.  If you add files,
+you'll need to put an `SPDX header comment`_ in each added file.  For those file types
+recognized by the `reuse-tool`_, you can use ``$ make devel-format`` to add such headers
+automatically.  Otherwise you may have to use ``$ reuse addheader`` manually specifying
+the appropriate ``--style`` option.  See ``$ reuse addheader --help`` for the available
+``${COMMENT_STYLE}`` values.  You can use ``--style "python"`` for unrecognized file
+types that support the common ``#`` comment style::
+
+  $ tox exec -e build -- reuse addheader --style "${COMMENT_STYLE:?}" \
+  --copyright "Ross Patterson <me@rpatterson.net>" --license "MIT" "${PATH:?}"
 
 Contributions should be pushed to feature branches or forks off of the upstream
 ``develop`` branch.  Once work is finished and all the tests are passing locally, open a
 merge/pull request (MR) against the upstream ``develop`` branch.  Address any issues
 revealed by any failed CI/CD jobs for your MR.  Once all CI/CD checks are green, project
 maintainers can merge your work where CI/CD will publish a pre-release for your changes
 including container images and PyPI packages.  Contributors should then test the
@@ -74,13 +94,17 @@
 the `Makefile`_ for guidance on making contributions there.
 
 
 .. _`Python's post-mortem debugger`:
    https://docs.python.org/3/library/pdb.html#pdb.post_mortem
 
 .. _`towncrier`: https://towncrier.readthedocs.io/en/stable/#philosophy
-.. _`news fragment`: https://towncrier.readthedocs.io/en/stable/quickstart.html#creating-news-fragments
+.. _`news fragment`:
+   https://towncrier.readthedocs.io/en/stable/quickstart.html#creating-news-fragments
+.. _`Reuse`: https://reuse.software/tutorial/#step-2
+.. _`SPDX header comment`: https://spdx.dev/specifications/#current-version
+.. _`reuse-tool`: https://github.com/fsfe/reuse-tool#usage
 
 .. _`an issue/ticket`: https://gitlab.com/rpatterson/feed-archiver/-/issues
 
 .. _Makefile: ./Makefile
 .. _`the ./TODO.rst file`: ./TODO.rst
```

### Comparing `feed-archiver-2.0.4/LICENSE` & `feed-archiver-2.0.6b1/LICENSES/MIT.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-The MIT License (MIT)
+MIT License
 
 Copyright (c) 2020 Ross Patterson
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `feed-archiver-2.0.4/Makefile` & `feed-archiver-2.0.6b1/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Development, build and maintenance tasks:
 #
 # To ease discovery for new contributors, variables that act as options affecting
 # behavior are at the top.  Then skip to `## Top-level targets:` below to find targets
 # intended for use by developers.  The real work, however, is in the recipes for real
 # targets that follow.  If making changes here, please start by reading the philosophy
 # commentary at the bottom of this file.
 
+# Project specific values:
+export PROJECT_NAMESPACE=rpatterson
+export PROJECT_NAME=feed-archiver
+
 # Variables used as options to control behavior:
 export TEMPLATE_IGNORE_EXISTING=false
 # https://devguide.python.org/versions/#supported-versions
-PYTHON_SUPPORTED_MINORS=3.11 3.10 3.9 3.8 3.7
-# Project-specific variables
+PYTHON_SUPPORTED_MINORS=3.10 3.11 3.9 3.8 3.7
 export DOCKER_USER=merpatterson
 GPG_SIGNING_KEYID=2EFF7CCE6828E359
-CI_UPSTREAM_NAMESPACE=rpatterson
-CI_PROJECT_NAME=feed-archiver
 
 # Project-specific options:
 DEBUG=
 POST_MORTEM=
 
 
 ## "Private" Variables:
@@ -65,15 +70,15 @@
 export TZ
 export DOCKER_GID=$(shell getent group "docker" | cut -d ":" -f 3)
 
 # Values concerning supported Python versions:
 # Use the same Python version tox would as a default.
 # https://tox.wiki/en/latest/config.html#base_python
 PYTHON_HOST_MINOR:=$(shell \
-    pip --version | sed -nE 's|.* \(python ([0-9]+.[0-9]+)\)$$|\1|p;q')
+    pip3 --version | sed -nE 's|.* \(python ([0-9]+.[0-9]+)\)$$|\1|p;q')
 export PYTHON_HOST_ENV=py$(subst .,,$(PYTHON_HOST_MINOR))
 # Determine the latest installed Python version of the supported versions
 PYTHON_BASENAMES=$(PYTHON_SUPPORTED_MINORS:%=python%)
 PYTHON_AVAIL_EXECS:=$(foreach \
     PYTHON_BASENAME,$(PYTHON_BASENAMES),$(shell which $(PYTHON_BASENAME)))
 PYTHON_LATEST_EXEC=$(firstword $(PYTHON_AVAIL_EXECS))
 PYTHON_LATEST_BASENAME=$(notdir $(PYTHON_LATEST_EXEC))
@@ -82,23 +87,26 @@
 # Fallback to the latest installed supported Python version
 PYTHON_MINOR=$(PYTHON_LATEST_BASENAME:python%=%)
 endif
 PYTHON_LATEST_MINOR=$(firstword $(PYTHON_SUPPORTED_MINORS))
 PYTHON_LATEST_ENV=py$(subst .,,$(PYTHON_LATEST_MINOR))
 PYTHON_MINORS=$(PYTHON_SUPPORTED_MINORS)
 ifeq ($(PYTHON_MINOR),)
-export PYTHON_MINOR=$(firstword $(PYTHON_MINORS))
+PYTHON_MINOR=$(firstword $(PYTHON_MINORS))
 else ifeq ($(findstring $(PYTHON_MINOR),$(PYTHON_MINORS)),)
-export PYTHON_MINOR=$(firstword $(PYTHON_MINORS))
+PYTHON_MINOR=$(firstword $(PYTHON_MINORS))
 endif
 export PYTHON_MINOR
 export PYTHON_ENV=py$(subst .,,$(PYTHON_MINOR))
 PYTHON_SHORT_MINORS=$(subst .,,$(PYTHON_MINORS))
 PYTHON_ENVS=$(PYTHON_SHORT_MINORS:%=py%)
 PYTHON_ALL_ENVS=$(PYTHON_ENVS) build
+PYTHON_EXTRAS=test devel
+PYTHON_PROJECT_PACKAGE=$(subst -,,$(PROJECT_NAME))
+PYTHON_PROJECT_GLOB=$(subst -,?,$(PROJECT_NAME))
 export PYTHON_WHEEL=
 
 # Values derived from VCS/git:
 VCS_LOCAL_BRANCH:=$(shell git branch --show-current)
 CI_COMMIT_BRANCH=
 GITHUB_REF_TYPE=
 GITHUB_REF_NAME=
@@ -200,28 +208,28 @@
 VCS_BRANCHES+=develop
 endif
 VCS_BRANCHES+=main
 endif
 
 # Values used to run Tox:
 TOX_ENV_LIST=$(subst $(EMPTY) ,$(COMMA),$(PYTHON_ENVS))
+TOX_RUN_ARGS=run-parallel --parallel auto --parallel-live
 ifeq ($(words $(PYTHON_MINORS)),1)
 TOX_RUN_ARGS=run
-else
-TOX_RUN_ARGS=run-parallel --parallel auto --parallel-live
 endif
 ifneq ($(PYTHON_WHEEL),)
 TOX_RUN_ARGS+= --installpkg "$(PYTHON_WHEEL)"
 endif
 export TOX_RUN_ARGS
 # The options that allow for rapid execution of arbitrary commands in the venvs managed
 # by tox
 TOX_EXEC_OPTS=--no-recreate-pkg --skip-pkg-install
 TOX_EXEC_ARGS=tox exec $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)"
 TOX_EXEC_BUILD_ARGS=tox exec $(TOX_EXEC_OPTS) -e "build"
+PIP_COMPILE_EXTRA=
 
 # Values used to build Docker images:
 DOCKER_FILE=./Dockerfile
 export DOCKER_BUILD_ARGS=
 export DOCKER_BUILD_PULL=false
 # Values used to tag built images:
 export DOCKER_VARIANT=
@@ -253,26 +261,27 @@
 DOCKER_IMAGES+=$(DOCKER_IMAGE_GITLAB)
 else ifeq ($(GITHUB_ACTIONS),true)
 DOCKER_IMAGES+=$(DOCKER_IMAGE_GITHUB)
 else
 DOCKER_IMAGES+=$(DOCKER_IMAGE_DOCKER)
 endif
 # Values used to run built images in containers:
-DOCKER_VOLUMES=\
-./var/docker/$(PYTHON_ENV)/ \
-./src/feed_archiver.egg-info/ \
-./var/docker/$(PYTHON_ENV)/feed_archiver.egg-info/ \
-./.tox/ ./var/docker/$(PYTHON_ENV)/.tox/
 DOCKER_COMPOSE_RUN_ARGS=
 DOCKER_COMPOSE_RUN_ARGS+= --rm
 ifeq ($(shell tty),not a tty)
 DOCKER_COMPOSE_RUN_ARGS+= -T
 endif
+export DOCKER_PASS
 
 # Values derived from or overridden by CI environments:
+CI_UPSTREAM_NAMESPACE=$(PROJECT_NAMESPACE)
+CI_PROJECT_NAME=$(PROJECT_NAME)
+ifeq ($(CI),true)
+TEMPLATE_IGNORE_EXISTING=true
+endif
 GITHUB_REPOSITORY_OWNER=$(CI_UPSTREAM_NAMESPACE)
 # Determine if this checkout is a fork of the upstream project:
 CI_IS_FORK=false
 ifeq ($(GITLAB_CI),true)
 USER_EMAIL=$(USER_NAME)@runners-manager.gitlab.com
 ifneq ($(VCS_BRANCH),develop)
 ifneq ($(VCS_BRANCH),main)
@@ -324,14 +333,15 @@
 # external changes, such as new PyPI releases, don't turn CI/CD red spuriously and
 # unrelated to the contributor's actual changes.
 PIP_COMPILE_ARGS=
 endif
 GITHUB_RELEASE_ARGS=--prerelease
 # Only publish releases from the `main` or `develop` branches and only under the
 # canonical CI/CD platform:
+DOCKER_PLATFORMS=
 ifeq ($(GITLAB_CI),true)
 ifeq ($(VCS_BRANCH),main)
 RELEASE_PUBLISH=true
 GITHUB_RELEASE_ARGS=
 else ifeq ($(VCS_BRANCH),develop)
 # Publish pre-releases from the `develop` branch:
 RELEASE_PUBLISH=true
@@ -364,141 +374,145 @@
 GH_TOKEN=
 
 # Defaults specific to this project:
 export NGINX_PORT=80
 DEBUG=
 POST_MORTEM=
 
+# Override variable values if present in `./.env` and if not overridden on the CLI:
+include $(wildcard .env)
+
 # Done with `$(shell ...)`, echo recipe commands going forward
 .SHELLFLAGS+= -x
 
 
-## Makefile "functions":
-#
-# Snippets whose output is frequently used including across recipes.  Used for output
-# only, not actually making any changes.
-# https://www.gnu.org/software/make/manual/html_node/Call-Function.html
-
-# Return the most recently built package:
-current_pkg = $(shell ls -t ./dist/*$(1) | head -n 1)
-
-
 ## Top-level targets:
 
 .PHONY: all
 ### The default target.
 all: build
 
 .PHONY: start
 ### Run the local development end-to-end stack services in the background as daemons.
-start: build-docker-volumes-$(PYTHON_ENV) build-docker-$(PYTHON_MINOR) ./.env
+start: build-docker-$(PYTHON_MINOR) ./.env.~out~
 	docker compose down
 	docker compose up -d
 
 .PHONY: run
 ### Run the local development end-to-end stack services in the foreground for debugging.
-run: build-docker-volumes-$(PYTHON_ENV) build-docker-$(PYTHON_MINOR) ./.env
+run: build-docker-$(PYTHON_MINOR) ./.env.~out~
 	docker compose down
 	docker compose up
 
 .PHONY: run-debug
 ### Run the update sub-command in the container via the interactive debugger
 run-debug: build
 	docker compose run --rm -e DEBUG="$(DEBUG)" -e POST_MORTEM="$(POST_MORTEM)" \
-	    --entrypoint="python" "feed-archiver" -m "pdb" \
-	    "/usr/local/bin/feed-archiver" "update"
+	    --entrypoint="python" "$(PROJECT_NAME)" -m "pdb" \
+	    "/usr/local/bin/$(PROJECT_NAME)" "update"
 
 
 ## Build Targets:
 #
 # Recipes that make artifacts needed for by end-users, development tasks, other recipes.
 
 .PHONY: build
 ### Set up everything for development from a checkout, local and in containers.
-build: ./.git/hooks/pre-commit \
-		$(HOME)/.local/var/log/feed-archiver-host-install.log \
+build: ./.git/hooks/pre-commit ./.env.~out~ \
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
 		build-docker ./server/.htpasswd \
-		./src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml
+		./src/$(PYTHON_PROJECT_PACKAGE)/tests/archives/end-to-end/.$(PROJECT_NAME).yml.~out~
+
+.PHONY: $(PYTHON_ENVS:%=build-requirements-%)
+### Compile fixed/pinned dependency versions if necessary.
+$(PYTHON_ENVS:%=build-requirements-%):
+# Avoid parallel tox recreations stomping on each other
+	$(MAKE) -e "$(@:build-requirements-%=./.tox/%/bin/pip-compile)"
+	targets="./requirements/$(@:build-requirements-%=%)/user.txt \
+	    $(PYTHON_EXTRAS:%=./requirements/$(@:build-requirements-%=%)/%.txt) \
+	    ./requirements/$(@:build-requirements-%=%)/build.txt \
+	    ./build-host/requirements-$(@:build-requirements-%=%).txt"
+# Workaround race conditions in pip's HTTP file cache:
+# https://github.com/pypa/pip/issues/6970#issuecomment-527678672
+	$(MAKE) -e -j $${targets} ||
+	    $(MAKE) -e -j $${targets} ||
+	    $(MAKE) -e -j $${targets}
+
+.PHONY: build-requirements-compile
+### Compile the requirements for one Python version and one type/extra.
+build-requirements-compile:
+	$(MAKE) -e "./.tox/$(PYTHON_ENV)/bin/pip-compile"
+	pip_compile_opts="--resolver backtracking --upgrade"
+ifneq ($(PIP_COMPILE_EXTRA),)
+	pip_compile_opts+=" --extra $(PIP_COMPILE_EXTRA)"
+endif
+	./.tox/$(PYTHON_ENV)/bin/pip-compile $${pip_compile_opts} \
+	    --output-file "$(PIP_COMPILE_OUT)" "$(PIP_COMPILE_SRC)"
 
 .PHONY: build-pkgs
 ### Ensure the built package is current when used outside of tox.
 build-pkgs: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log build-docker-volumes-$(PYTHON_ENV)
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log
 # Defined as a .PHONY recipe so that multiple targets can depend on this as a
 # pre-requisite and it will only be run once per invocation.
 	rm -vf ./dist/*
 # Build Python packages/distributions from the development Docker container for
 # consistency/reproducibility.
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) feed-archiver-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    tox run -e "$(PYTHON_ENV)" --pkg-only
 # Copy the wheel to a location accessible to all containers:
 	cp -lfv "$$(
-	    ls -t ./var/docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.whl | head -n 1
+	    ls -t ./var-docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.whl | head -n 1
 	)" "./dist/"
 # Also build the source distribution:
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) feed-archiver-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    tox run -e "$(PYTHON_ENV)" --override "testenv.package=sdist" --pkg-only
 	cp -lfv "$$(
-	    ls -t ./var/docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.tar.gz | head -n 1
+	    ls -t ./var-docker/$(PYTHON_ENV)/.tox/.pkg/dist/*.tar.gz | head -n 1
 	)" "./dist/"
 
-.PHONY: $(PYTHON_ENVS:%=build-requirements-%)
-### Compile fixed/pinned dependency versions if necessary.
-$(PYTHON_ENVS:%=build-requirements-%):
-# Avoid parallel tox recreations stomping on each other
-	$(MAKE) -e "$(@:build-requirements-%=./var/log/tox/%/build.log)"
-	targets="./requirements/$(@:build-requirements-%=%)/user.txt \
-	    ./requirements/$(@:build-requirements-%=%)/devel.txt \
-	    ./requirements/$(@:build-requirements-%=%)/build.txt \
-	    ./build-host/requirements-$(@:build-requirements-%=%).txt"
-# Workaround race conditions in pip's HTTP file cache:
-# https://github.com/pypa/pip/issues/6970#issuecomment-527678672
-	$(MAKE) -e -j $${targets} ||
-	    $(MAKE) -e -j $${targets} ||
-	    $(MAKE) -e -j $${targets}
-
 ## Docker Build Targets:
 #
 # Strive for as much consistency as possible in development tasks between the local host
 # and inside containers.  To that end, most of the `*-docker` container target recipes
 # should run the corresponding `*-local` local host target recipes inside the
 # development container.  Top level targets, like `test`, should run as much as possible
 # inside the development container.
 
 .PHONY: build-docker
 ### Set up for development in Docker containers.
-build-docker: build-pkgs ./var/log/tox/build/build.log
+build-docker: build-pkgs ./var-docker/$(PYTHON_ENV)/log/build-user.log
+	tox run $(TOX_EXEC_OPTS) --notest -e "build"
 	$(MAKE) -e -j PYTHON_WHEEL="$(call current_pkg,.whl)" \
 	    DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --progress plain" \
 	    $(PYTHON_MINORS:%=build-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=build-docker-%)
 ### Set up for development in a Docker container for one Python version.
 $(PYTHON_MINORS:%=build-docker-%):
 	$(MAKE) -e \
 	    PYTHON_MINORS="$(@:build-docker-%=%)" \
 	    PYTHON_MINOR="$(@:build-docker-%=%)" \
 	    PYTHON_ENV="py$(subst .,,$(@:build-docker-%=%))" \
-	    "./var/docker/py$(subst .,,$(@:build-docker-%=%))/log/build-user.log"
+	    "./var-docker/py$(subst .,,$(@:build-docker-%=%))/log/build-user.log"
 
 .PHONY: build-docker-tags
 ### Print the list of image tags for the current registry and variant.
 build-docker-tags:
 	$(MAKE) -e $(DOCKER_REGISTRIES:%=build-docker-tags-%)
 
 .PHONY: $(DOCKER_REGISTRIES:%=build-docker-tags-%)
 ### Print the list of image tags for the current registry and variant.
 $(DOCKER_REGISTRIES:%=build-docker-tags-%): \
-		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		./var/log/tox/build/build.log
+		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH)
 	docker_image=$(DOCKER_IMAGE_$(@:build-docker-tags-%=%))
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)
 ifeq ($(VCS_BRANCH),main)
 # Only update tags end users may depend on to be stable from the `main` branch
-	VERSION=$$(./.tox/build/bin/cz version --project)
+	VERSION=$$($(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project)
 	major_version=$$(echo $${VERSION} | sed -nE 's|([0-9]+).*|\1|p')
 	minor_version=$$(
 	    echo $${VERSION} | sed -nE 's|([0-9]+\.[0-9]+).*|\1|p'
 	)
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-v$${minor_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-v$${major_version}
 	echo $${docker_image}:$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)
@@ -515,16 +529,16 @@
 	echo $${docker_image}:$(DOCKER_VARIANT)
 endif
 endif
 endif
 
 .PHONY: build-docker-build
 ### Run the actual commands used to build the Docker container image.
-build-docker-build: $(HOME)/.local/var/log/docker-multi-platform-host-install.log \
-		./var/log/tox/build/build.log \
+build-docker-build: ./Dockerfile \
+		$(HOME)/.local/var/log/docker-multi-platform-host-install.log \
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/log/docker-login-DOCKER.log
 # Workaround broken interactive session detection:
 	docker pull "python:$(PYTHON_MINOR)"
 	docker_build_caches=""
 ifeq ($(GITLAB_CI),true)
 # Don't cache when building final releases on `main`
@@ -543,73 +557,77 @@
 	if $(MAKE) -e pull-docker
 	then
 	    docker_build_caches+=" --cache-from $(DOCKER_IMAGE_GITHUB):\
 	$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$(DOCKER_BRANCH_TAG)"
 	fi
 endif
 endif
-	docker_image_tags=""
+	docker_build_args=""
 	for image_tag in $$(
 	    $(MAKE) -e --no-print-directory build-docker-tags
 	)
 	do
-	    docker_image_tags+="--tag $${image_tag} "
+	    docker_build_args+=" --tag $${image_tag}"
 	done
+ifeq ($(DOCKER_VARIANT),)
+	docker_build_args+=" --target user"
+else
+	docker_build_args+=" --target $(DOCKER_VARIANT)"
+endif
 # https://github.com/moby/moby/issues/39003#issuecomment-879441675
 	docker buildx build $(DOCKER_BUILD_ARGS) \
 	    --build-arg BUILDKIT_INLINE_CACHE="1" \
 	    --build-arg PYTHON_MINOR="$(PYTHON_MINOR)" \
 	    --build-arg PYTHON_ENV="$(PYTHON_ENV)" \
-	    --build-arg VERSION="$$(./.tox/build/bin/cz version --project)" \
-	    $${docker_image_tags} $${docker_build_caches} --file "$(DOCKER_FILE)" "./"
+	    --build-arg VERSION="$$(
+	        $(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project
+	    )" \
+	    $${docker_build_args} $${docker_build_caches} --file "$(<)" "./"
 
 .PHONY: $(PYTHON_MINORS:%=build-docker-requirements-%)
 ### Pull container images and compile fixed/pinned dependency versions if necessary.
-$(PYTHON_MINORS:%=build-docker-requirements-%): ./.env
+$(PYTHON_MINORS:%=build-docker-requirements-%): ./.env.~out~
 	export PYTHON_MINOR="$(@:build-docker-requirements-%=%)"
 	export PYTHON_ENV="py$(subst .,,$(@:build-docker-requirements-%=%))"
-	$(MAKE) -e build-docker-volumes-$${PYTHON_ENV} \
-	    "./var/docker/$${PYTHON_ENV}/log/build-devel.log"
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) feed-archiver-devel \
+	$(MAKE) -e "./var-docker/$${PYTHON_ENV}/log/build-devel.log"
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    make -e PYTHON_MINORS="$(@:build-docker-requirements-%=%)" \
 	    PIP_COMPILE_ARGS="$(PIP_COMPILE_ARGS)" \
 	    build-requirements-py$(subst .,,$(@:build-docker-requirements-%=%))
 
-.PHONY: $(PYTHON_ENVS:%=build-docker-volumes-%)
-### Ensure access permissions to build artifacts in Python version container volumes.
-# If created by `# dockerd`, they end up owned by `root`.
-$(PYTHON_ENVS:%=build-docker-volumes-%): \
-		./src/feed_archiver.egg-info/ ./.tox/
-	$(MAKE) -e \
-	    $(@:build-docker-volumes-%=./var/docker/%/) \
-	    $(@:build-docker-volumes-%=./var/docker/%/feed_archiver.egg-info/) \
-	    $(@:build-docker-volumes-%=./var/docker/%/.tox/)
-
 
 ## Test Targets:
 #
 # Recipes that run the test suite.
 
 .PHONY: test
 ### Format the code and run the full suite of tests, coverage checks, and linters.
 test: test-docker-lint test-docker
 
 .PHONY: test-local
-### Run the full suite of tests on the local host.
+### Run the full suite of tests, coverage checks, and linters on the local host.
 test-local:
 	tox $(TOX_RUN_ARGS) -e "$(TOX_ENV_LIST)"
 
+.PHONY: test-lint
+### Perform any linter or style checks, including non-code checks.
+test-lint: $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log
+# Run non-code checks, e.g. documentation:
+	tox run -e "build"
+
 .PHONY: test-debug
-### Run tests in the host environment and invoke the debugger on errors/failures.
-test-debug: ./var/log/tox/$(PYTHON_ENV)/editable.log
+### Run tests directly on the host and invoke the debugger on errors/failures.
+test-debug: ./.tox/$(PYTHON_ENV)/log/editable.log
 	$(TOX_EXEC_ARGS) -- pytest --pdb
 
 .PHONY: test-docker
 ### Run the full suite of tests, coverage checks, and code linters in containers.
-test-docker: build-pkgs ./var/log/tox/build/build.log ./var/log/codecov-install.log
+test-docker: build-pkgs $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
+		build-docker
+	tox run $(TOX_EXEC_OPTS) --notest -e "build"
 	$(MAKE) -e -j PYTHON_WHEEL="$(call current_pkg,.whl)" \
 	    DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --progress plain" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=test-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=test-docker-%)
 ### Run the full suite of tests inside a docker container for one Python version.
@@ -618,62 +636,59 @@
 	    PYTHON_MINORS="$(@:test-docker-%=%)" \
 	    PYTHON_MINOR="$(@:test-docker-%=%)" \
 	    PYTHON_ENV="py$(subst .,,$(@:test-docker-%=%))" \
 	    test-docker-pyminor
 
 .PHONY: test-docker-pyminor
 ### Run the full suite of tests inside a docker container for this Python version.
-test-docker-pyminor: build-docker-volumes-$(PYTHON_ENV) build-docker-$(PYTHON_MINOR) \
-		./var/log/codecov-install.log
+test-docker-pyminor: build-docker-$(PYTHON_MINOR) \
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log
 	docker_run_args="--rm"
 	if [ ! -t 0 ]
 	then
 # No fancy output when running in parallel
 	    docker_run_args+=" -T"
 	fi
 # Ensure the dist/package has been correctly installed in the image
-	docker compose run --no-deps $${docker_run_args} feed-archiver \
-	    python -m feedarchiver --help
-	docker compose run --no-deps $${docker_run_args} feed-archiver \
-	    feed-archiver --help
+	docker compose run --no-deps $${docker_run_args} $(PROJECT_NAME) \
+	    python -m "$(PYTHON_PROJECT_PACKAGE)" --help
+	docker compose run --no-deps $${docker_run_args} $(PROJECT_NAME) \
+	    $(PROJECT_NAME) --help
 # Run from the development Docker container for consistency
-	docker compose run $${docker_run_args} feed-archiver-devel \
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
 endif
 endif
 
 .PHONY: test-docker-lint
 ### Check the style and content of the `./Dockerfile*` files.
-test-docker-lint: ./.env build-docker-volumes-$(PYTHON_ENV) \
-		./var/log/docker-login-DOCKER.log
+test-docker-lint: ./.env.~out~ ./var/log/docker-login-DOCKER.log
 	docker compose pull --quiet hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint
 	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
-	    hadolint "./Dockerfile.devel"
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) hadolint \
 	    hadolint "./build-host/Dockerfile"
 
 .PHONY: test-push
 ### Perform any checks that should only be run before pushing.
 test-push: $(VCS_FETCH_TARGETS) \
-		$(HOME)/.local/var/log/feed-archiver-host-install.log \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
-		build-docker-volumes-$(PYTHON_ENV) ./.env
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env.~out~
 	vcs_compare_rev="$(VCS_COMPARE_REMOTE)/$(VCS_COMPARE_BRANCH)"
 ifeq ($(CI),true)
 ifneq ($(PYTHON_MINOR),$(PYTHON_HOST_MINOR))
 # Don't waste CI time, only check for the canonical version:
 	exit
 endif
 ifeq ($(VCS_COMPARE_BRANCH),main)
@@ -697,15 +712,15 @@
 	then
 	    exit
 	elif (( $$exit_code != 0 ))
 	then
 	    exit $$exit_code
 	else
 	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
-	        feed-archiver-devel $(TOX_EXEC_ARGS) -- \
+	        $(PROJECT_NAME)-devel $(TOX_EXEC_ARGS) -- \
 	        towncrier check --compare-with "$${vcs_compare_rev}"
 	fi
 
 .PHONY: test-clean
 ### Confirm that the checkout is free of uncommitted VCS changes.
 test-clean:
 	if [ -n "$$(git status --porcelain)" ]
@@ -719,70 +734,70 @@
 ## Release Targets:
 #
 # Recipes that make an changes needed for releases and publish built artifacts to
 # end-users.
 
 .PHONY: release
 ### Publish installable Python packages and container images as required by commits.
-release: release-python release-docker
+release: release-pkgs release-docker
 
-.PHONY: release-python
-### Publish installable Python packages to PyPI.
-release-python: ./var/log/tox/build/build.log ./var/log/git-remotes.log \
-		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		~/.pypirc ./.env build-docker-volumes-$(PYTHON_ENV)
+.PHONY: release-pkgs
+### Publish installable Python packages to PyPI if conventional commits require.
+release-pkgs: $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
+		./var/log/git-remotes.log \
+		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) ~/.pypirc.~out~ \
+		./.env.~out~
 # Only release from the `main` or `develop` branches:
 ifeq ($(RELEASE_PUBLISH),true)
 # Import the private signing key from CI secrets
 	$(MAKE) -e ./var/log/gpg-import.log
 # Bump the version and build the final release packages:
 	$(MAKE) -e build-pkgs
 # https://twine.readthedocs.io/en/latest/#using-twine
-	./.tox/build/bin/twine check ./dist/feed?archiver-*
+	$(TOX_EXEC_BUILD_ARGS) -- twine check ./dist/$(PYTHON_PROJECT_GLOB)-*
 # The VCS remote should reflect the release before the release is published to ensure
 # that a published release is never *not* reflected in VCS.  Also ensure the tag is in
 # place on any mirrors, using multiple `pushurl` remotes, for those project hosts as
 # well:
 	$(MAKE) -e test-clean
-	./.tox/build/bin/twine upload -s -r "$(PYPI_REPO)" \
-	    ./dist/feed?archiver-*
-	export VERSION=$$(./.tox/build/bin/cz version --project)
+	$(TOX_EXEC_BUILD_ARGS) -- twine upload -s -r "$(PYPI_REPO)" \
+	    ./dist/$(PYTHON_PROJECT_GLOB)-*
+	export VERSION=$$($(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project)
 # Create a GitLab release
 	./.tox/build/bin/twine upload -s -r "gitlab" \
-	    ./dist/feed?archiver-*
+	    ./dist/$(PYTHON_PROJECT_GLOB)-*
 	release_cli_args="--description ./NEWS-VERSION.rst"
 	release_cli_args+=" --tag-name v$${VERSION}"
 	release_cli_args+=" --assets-link {\
 	\"name\":\"PyPI\",\
 	\"url\":\"https://$(PYPI_HOSTNAME)/project/$(CI_PROJECT_NAME)/$${VERSION}/\",\
 	\"link_type\":\"package\"\
 	}"
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
 	gh release create "v$${VERSION}" $(GITHUB_RELEASE_ARGS) \
-	    --notes-file "./NEWS-VERSION.rst" ./dist/feed?archiver-*
+	    --notes-file "./NEWS-VERSION.rst" ./dist/$(PYTHON_PROJECT_GLOB)-*
 endif
 
 .PHONY: release-docker
 ### Publish all container images to all container registries.
-release-docker: build-docker-volumes-$(PYTHON_ENV) build-docker \
-		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
+release-docker: build-docker $(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log)
 	$(MAKE) -e -j DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=release-docker-%)
 
 .PHONY: $(PYTHON_MINORS:%=release-docker-%)
 ### Publish the container images for one Python version to all container registries.
 $(PYTHON_MINORS:%=release-docker-%): \
 		$(DOCKER_REGISTRIES:%=./var/log/docker-login-%.log) \
@@ -792,58 +807,58 @@
 # previously built native images into the manifests.
 	DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --push"
 ifneq ($(DOCKER_PLATFORMS),)
 	DOCKER_BUILD_ARGS+=" --platform $(subst $(EMPTY) ,$(COMMA),$(DOCKER_PLATFORMS))"
 else
 endif
 	export DOCKER_BUILD_ARGS
-# Push the development manifest and images:
-	$(MAKE) -e DOCKER_FILE="./Dockerfile.devel" DOCKER_VARIANT="devel" \
-	    build-docker-build
 # Push the end-user manifest and images:
 	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
 	$(MAKE) -e DOCKER_BUILD_ARGS="$${DOCKER_BUILD_ARGS}\
 	    --build-arg PYTHON_WHEEL=$${PYTHON_WHEEL}" build-docker-build
-# Update Docker Hub `README.md` from the official/canonical Python version:
+# Push the development manifest and images:
+	$(MAKE) -e DOCKER_VARIANT="devel" build-docker-build
+# Update Docker Hub `README.md` using the `./README.rst` reStructuredText version using
+# the official/canonical Python version:
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
-		./var/log/git-remotes.log ./var/log/tox/build/build.log \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
-		./.env build-docker-volumes-$(PYTHON_ENV)
+		./var/log/git-remotes.log \
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./.env.~out~
 	if ! git diff --cached --exit-code
 	then
 	    set +x
 	    echo "CRITICAL: Cannot bump version with staged changes"
 	    false
 	fi
 # Ensure the local branch is updated to the forthcoming version bump commit:
-	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)" --
+	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)"
 # Check if a release is required:
 	exit_code=0
 	if [ "$(VCS_BRANCH)" = "main" ] &&
-	    ./.tox/build/bin/python ./bin/get-base-version $$(
-	        ./.tox/build/bin/cz version --project
+	    $(TOX_EXEC_BUILD_ARGS) -qq -- python ./bin/get-base-version $$(
+	        $(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project
 	    )
 	then
 # Release a previous pre-release as final regardless of whether commits since then
 # require a release:
 	    true
 	else
 # Is a release required by conventional commits:
-	    ./.tox/build/bin/python ./bin/cz-check-bump || exit_code=$$?
+	    $(TOX_EXEC_BUILD_ARGS) -qq -- python ./bin/cz-check-bump || exit_code=$$?
 	    if (( $$exit_code == 3 || $$exit_code == 21 ))
 	    then
 # No commits require a release:
 	        exit
 	    elif (( $$exit_code != 0 ))
 	    then
 	        exit $$exit_code
@@ -862,75 +877,77 @@
 # Capture the release notes for *just this* release for creating the GitHub release.
 # Have to run before the real `$ towncrier build` run without the `--draft` option
 # because after that the `newsfragments` will have been deleted.
 	next_version=$$(
 	    $(TOX_EXEC_BUILD_ARGS) -qq -- cz bump $${cz_bump_args} --yes --dry-run |
 	    sed -nE 's|.* ([^ ]+) *→ *([^ ]+).*|\2|p;q'
 	) || true
-# Build and stage the release notes to be commited by `$ cz bump`
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) feed-archiver-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    $(TOX_EXEC_ARGS) -qq -- \
 	    towncrier build --version "$${next_version}" --draft --yes \
 	    >"./NEWS-VERSION.rst"
 	git add -- "./NEWS-VERSION.rst"
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) feed-archiver-devel \
+# Build and stage the release notes to be commited by `$ cz bump`:
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    $(TOX_EXEC_ARGS) -- towncrier build --version "$${next_version}" --yes
 # Increment the version in VCS
 	$(TOX_EXEC_BUILD_ARGS) -- cz bump $${cz_bump_args}
 # Ensure the container image reflects the version bump but we don't need to update the
 # requirements again.
 	touch \
 	    $(PYTHON_ENVS:%=./requirements/%/user.txt) \
 	    $(PYTHON_ENVS:%=./requirements/%/devel.txt) \
 	    $(PYTHON_ENVS:%=./build-host/requirements-%.txt)
 ifeq ($(VCS_BRANCH),main)
 # Merge the bumped version back into `develop`:
-	bump_rev="$$(git rev-parse HEAD)"
-	git switch -C "develop" --track "$(VCS_COMPARE_REMOTE)/develop" --
-	git merge --ff --gpg-sign \
-	    -m "Merge branch 'main' release back into develop" "$${bump_rev}"
+	$(MAKE) VCS_BRANCH="main" VCS_MERGE_BRANCH="develop" \
+	    VCS_REMOTE="$(VCS_COMPARE_REMOTE)" VCS_MERGE_BRANCH="develop" devel-merge
 ifeq ($(CI),true)
-	git push --no-verify --tags "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
+	git push --no-verify "$(VCS_COMPARE_REMOTE)" "HEAD:develop"
 endif
-	git switch -C "$(VCS_BRANCH)" "$${bump_rev}" --
+	git switch -C "$(VCS_BRANCH)" "$$(git rev-parse HEAD)"
 endif
 ifneq ($(GITHUB_ACTIONS),true)
 ifneq ($(PROJECT_GITHUB_PAT),)
 # Ensure the tag is available for creating the GitHub release below but push *before* to
 # GitLab to avoid a race with repository mirrorying:
-	git push --no-verify --tags "github" "HEAD:$(VCS_BRANCH)"
+	git push --no-verify "github" tag "v$${next_version}"
 endif
 endif
 ifeq ($(CI),true)
-	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
+# Push just this tag to avoid clashes with any previously failed release:
+	git push --no-verify "$(VCS_REMOTE)" tag "v$${next_version}"
+# Also push the branch:
+	git push --no-verify "$(VCS_REMOTE)" "HEAD:$(VCS_BRANCH)"
 endif
 
 
 ## Development Targets:
 #
 # Recipes used by developers to make changes to the code.
 
 .PHONY: devel-format
 ### Automatically correct code in this checkout according to linters and style checkers.
-devel-format: $(HOME)/.local/var/log/feed-archiver-host-install.log
+devel-format: $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log
 	$(TOX_EXEC_ARGS) -- autoflake -r -i --remove-all-unused-imports \
 		--remove-duplicate-keys --remove-unused-variables \
-		--remove-unused-variables "./src/feedarchiver/"
-	$(TOX_EXEC_ARGS) -- autopep8 -v -i -r "./src/feedarchiver/"
-	$(TOX_EXEC_ARGS) -- black "./src/feedarchiver/"
+		--remove-unused-variables "./src/$(PYTHON_PROJECT_PACKAGE)/"
+	$(TOX_EXEC_ARGS) -- autopep8 -v -i -r "./src/$(PYTHON_PROJECT_PACKAGE)/"
+	$(TOX_EXEC_ARGS) -- black "./src/$(PYTHON_PROJECT_PACKAGE)/"
+	$(TOX_EXEC_ARGS) -- reuse addheader -r --skip-unrecognised \
+	    --copyright "Ross Patterson <me@rpatterson.net>" --license "MIT" "./"
 
 .PHONY: devel-upgrade
 ### Update all fixed/pinned dependencies to their latest available versions.
-devel-upgrade: ./.env build-docker-volumes-$(PYTHON_ENV) \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log \
-		./var/log/tox/build/build.log
+devel-upgrade: ./.env.~out~ $(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log \
+		build-docker
 	touch "./setup.cfg" "./requirements/build.txt.in" \
 	    "./build-host/requirements.txt.in"
 # Ensure the network is create first to avoid race conditions
-	docker compose create feed-archiver-devel
+	docker compose create $(PROJECT_NAME)-devel
 	$(MAKE) -e -j PIP_COMPILE_ARGS="--upgrade" \
 	    DOCKER_COMPOSE_RUN_ARGS="$(DOCKER_COMPOSE_RUN_ARGS) -T" \
 	    $(PYTHON_MINORS:%=build-docker-requirements-%)
 # Update VCS hooks from remotes to the latest tag.
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit autoupdate
 
 .PHONY: devel-upgrade-branch
@@ -939,28 +956,28 @@
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
 		./var/log/git-remotes.log
 	remote_branch_exists=false
 	if git fetch "$(VCS_REMOTE)" "$(VCS_BRANCH)-upgrade"
 	then
 	    remote_branch_exists=true
 	fi
-	git switch -C "$(VCS_BRANCH)-upgrade" --track "$(VCS_BRANCH)" --
+	git switch -C "$(VCS_BRANCH)-upgrade"
 	now=$$(date -u)
 	$(MAKE) -e devel-upgrade
 	if $(MAKE) -e "test-clean"
 	then
 # No changes from upgrade, exit successfully but push nothing
 	    exit
 	fi
 # Commit the upgrade changes
 	echo "Upgrade all requirements to the latest versions as of $${now}." \
-	    >"./src/feedarchiver/newsfragments/+upgrade-requirements.bugfix.rst"
+	    >"./newsfragments/+upgrade-requirements.bugfix.rst"
 	git add --update './build-host/requirements-*.txt' './requirements/*/*.txt' \
 	    "./.pre-commit-config.yaml"
-	git add "./src/feedarchiver/newsfragments/+upgrade-requirements.bugfix.rst"
+	git add "./newsfragments/+upgrade-requirements.bugfix.rst"
 	git_commit_args="--all --gpg-sign"
 ifeq ($(CI),true)
 # Don't duplicate the CI run from the push below:
 	git_push_args+=" --no-verify"
 endif
 	git commit $${git_commit_args} -m \
 	    "fix(deps): Upgrade requirements latest versions"
@@ -985,15 +1002,15 @@
 		./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_MERGE_BRANCH)
 	merge_rev="$$(git rev-parse HEAD)"
 	git switch -C "$(VCS_MERGE_BRANCH)" --track "$(VCS_REMOTE)/$(VCS_MERGE_BRANCH)"
 	git merge --ff --gpg-sign -m \
 	    $$'Merge branch \'$(VCS_BRANCH)\' into $(VCS_MERGE_BRANCH)\n\n[ci merge]' \
 	    "$${merge_rev}"
 ifeq ($(CI),true)
-	git push --no-verify --tags "$(VCS_REMOTE)" "HEAD:$(VCS_MERGE_BRANCH)"
+	git push --no-verify "$(VCS_REMOTE)" "HEAD:$(VCS_MERGE_BRANCH)"
 endif
 
 
 ## Clean Targets:
 #
 # Recipes used to restore the checkout to initial conditions.
 
@@ -1001,217 +1018,164 @@
 ### Restore the checkout to a state as close to an initial clone as possible.
 clean:
 	docker compose down --remove-orphans --rmi "all" -v || true
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit uninstall \
 	    --hook-type "pre-commit" --hook-type "commit-msg" --hook-type "pre-push" \
 	    || true
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit clean || true
-	git clean -dfx -e "var/" -e ".env"
-	rm -rfv "./var/log/"
-	rm -rf "./var/docker/"
+	git clean -dfx -e "/var" -e "var-docker/" -e "/.env" -e "*~"
+	git clean -dfx "./var-docker/py*/.tox/" \
+	    "./var-docker/py*/feed_archiver.egg-info/"
+	rm -rfv "./var/log/" ./var-docker/py*/log/
 
 
 ## Real Targets:
 #
 # Recipes that make actual changes and create and update files for the target.
 
 # Manage fixed/pinned versions in `./requirements/**.txt` files.  Has to be run for each
 # python version in the virtual environment for that Python version:
 # https://github.com/jazzband/pip-tools#cross-environment-usage-of-requirementsinrequirementstxt-and-pip-compile
-$(PYTHON_ENVS:%=./requirements/%/devel.txt): ./pyproject.toml ./setup.cfg ./tox.ini
+python_combine_requirements=$(PYTHON_ENVS:%=./requirements/%/$(1).txt)
+$(foreach extra,$(PYTHON_EXTRAS),$(call python_combine_requirements,$(extra))): \
+		./pyproject.toml ./setup.cfg ./tox.ini
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "$(@:requirements/%/devel.txt=./var/log/tox/%/build.log)"
-	./.tox/$(@:requirements/%/devel.txt=%)/bin/pip-compile \
-	    --resolver "backtracking" $(PIP_COMPILE_ARGS) --extra "devel" \
-	    --output-file "$(@)" "$(<)"
+	extra_basename="$$(basename "$(@)")"
+	$(MAKE) -e PYTHON_ENV="$$(basename "$$(dirname "$(@)")")" \
+	    PIP_COMPILE_EXTRA="$${extra_basename%.txt}" \
+	    PIP_COMPILE_SRC="$(<)" PIP_COMPILE_OUT="$(@)" \
+	    build-requirements-compile
 	mkdir -pv "./var/log/"
 	touch "./var/log/rebuild.log"
 $(PYTHON_ENVS:%=./requirements/%/user.txt): ./pyproject.toml ./setup.cfg ./tox.ini
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "$(@:requirements/%/user.txt=./var/log/tox/%/build.log)"
-	./.tox/$(@:requirements/%/user.txt=%)/bin/pip-compile \
-	    --resolver "backtracking" $(PIP_COMPILE_ARGS) --output-file "$(@)" "$(<)"
+	$(MAKE) -e PYTHON_ENV="$(@:requirements/%/user.txt=%)" PIP_COMPILE_SRC="$(<)" \
+	    PIP_COMPILE_OUT="$(@)" build-requirements-compile
 	mkdir -pv "./var/log/"
 	touch "./var/log/rebuild.log"
 $(PYTHON_ENVS:%=./build-host/requirements-%.txt): ./build-host/requirements.txt.in
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "$(@:build-host/requirements-%.txt=./var/log/tox/%/build.log)"
-	./.tox/$(@:build-host/requirements-%.txt=%)/bin/pip-compile \
-	    --resolver "backtracking" $(PIP_COMPILE_ARGS) --output-file "$(@)" "$(<)"
+	$(MAKE) -e PYTHON_ENV="$(@:build-host/requirements-%.txt=%)" \
+	    PIP_COMPILE_SRC="$(<)" PIP_COMPILE_OUT="$(@)" build-requirements-compile
 # Only update the installed tox version for the latest/host/main/default Python version
 	if [ "$(@:build-host/requirements-%.txt=%)" = "$(PYTHON_ENV)" ]
 	then
 # Don't install tox into one of it's own virtual environments
 	    if [ -n "$${VIRTUAL_ENV:-}" ]
 	    then
-	        pip_bin="$$(which -a pip | grep -v "^$${VIRTUAL_ENV}/bin/" | head -n 1)"
+	        pip_bin="$$(which -a pip3 | grep -v "^$${VIRTUAL_ENV}/bin/" | head -n 1)"
 	    else
-	        pip_bin="pip"
+	        pip_bin="pip3"
 	    fi
 	    "$${pip_bin}" install -r "$(@)"
 	fi
 	mkdir -pv "./var/log/"
 	touch "./var/log/rebuild.log"
 $(PYTHON_ENVS:%=./requirements/%/build.txt): ./requirements/build.txt.in
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e "$(@:requirements/%/build.txt=./var/log/tox/%/build.log)"
-	./.tox/$(@:requirements/%/build.txt=%)/bin/pip-compile \
-	    --resolver "backtracking" $(PIP_COMPILE_ARGS) --output-file "$(@)" "$(<)"
+	$(MAKE) -e PYTHON_ENV="$(@:requirements/%/build.txt=%)" PIP_COMPILE_SRC="$(<)" \
+	    PIP_COMPILE_OUT="$(@)" build-requirements-compile
 
 # Targets used as pre-requisites to ensure virtual environments managed by tox have been
 # created and can be used directly to save time on Tox's overhead when we don't need
 # Tox's logic about when to update/recreate them, e.g.:
 #     $ ./.tox/build/bin/cz --help
 # Mostly useful for build/release tools.
-$(PYTHON_ALL_ENVS:%=./var/log/tox/%/build.log):
-	$(MAKE) -e "$(HOME)/.local/var/log/feed-archiver-host-install.log"
-	mkdir -pv "$(dir $(@))"
-	tox run $(TOX_EXEC_OPTS) -e "$(@:var/log/tox/%/build.log=%)" --notest |&
-	    tee -a "$(@)"
+$(PYTHON_ALL_ENVS:%=./.tox/%/bin/pip-compile):
+	$(MAKE) -e "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
+	tox run $(TOX_EXEC_OPTS) -e "$(@:.tox/%/bin/pip-compile=%)" --notest
 # Workaround tox's `usedevelop = true` not working with `./pyproject.toml`.  Use as a
 # prerequisite when using Tox-managed virtual environments directly and changes to code
 # need to take effect immediately.
-$(PYTHON_ENVS:%=./var/log/tox/%/editable.log):
-	$(MAKE) -e "$(HOME)/.local/var/log/feed-archiver-host-install.log"
+$(PYTHON_ENVS:%=./.tox/%/log/editable.log):
+	$(MAKE) -e "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
 	mkdir -pv "$(dir $(@))"
-	tox exec $(TOX_EXEC_OPTS) -e "$(@:var/log/tox/%/editable.log=%)" -- \
-	    pip install -e "./" |& tee -a "$(@)"
+	tox exec $(TOX_EXEC_OPTS) -e "$(@:./.tox/%/log/editable.log=%)" -- \
+	    pip3 install -e "./" |& tee -a "$(@)"
 
 ## Docker real targets:
 
 # Build the development image:
-./var/docker/$(PYTHON_ENV)/log/build-devel.log: \
-		./Dockerfile.devel ./.dockerignore ./bin/entrypoint \
+./var-docker/$(PYTHON_ENV)/log/build-devel.log: ./Dockerfile ./.dockerignore \
+		./bin/entrypoint ./build-host/requirements.txt.in \
+		./var-docker/$(PYTHON_ENV)/log/rebuild.log \
 		./pyproject.toml ./setup.cfg ./tox.ini \
-		./build-host/requirements.txt.in ./docker-compose.yml \
-		./docker-compose.override.yml ./.env \
-		./var/docker/$(PYTHON_ENV)/log/rebuild.log
+		./docker-compose.yml ./docker-compose.override.yml ./.env.~out~ \
+		./bin/host-install
 	true DEBUG Updated prereqs: $(?)
-	$(MAKE) -e build-docker-volumes-$(PYTHON_ENV)
 	mkdir -pv "$(dir $(@))"
 ifeq ($(DOCKER_BUILD_PULL),true)
 # Pull the development image and simulate as if it had been built here.
 	if $(MAKE) -e DOCKER_VARIANT="devel" pull-docker
 	then
-	    touch "$(@)" "./var/docker/$(PYTHON_ENV)/log/rebuild.log"
+	    touch "$(@)" "./var-docker/$(PYTHON_ENV)/log/rebuild.log"
 # Ensure the virtualenv in the volume is also current:
-	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) \
-	        feed-archiver-devel make -e PYTHON_MINORS="$(PYTHON_MINOR)" \
-	        "./var/log/tox/$(PYTHON_ENV)/build.log"
+	    docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
+	        tox run $(TOX_EXEC_OPTS) -e "$(PYTHON_ENV)" --notest
 	    exit
 	fi
 endif
-	$(MAKE) -e DOCKER_FILE="./Dockerfile.devel" DOCKER_VARIANT="devel" \
-	    DOCKER_BUILD_ARGS="--load" build-docker-build >>"$(@)"
+	$(MAKE) -e DOCKER_VARIANT="devel" DOCKER_BUILD_ARGS="--load" \
+	    build-docker-build | tee -a "$(@)"
+# Represent that host install is baked into the image in the `${HOME}` bind volume:
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
-	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) feed-archiver-devel \
+	docker compose run $(DOCKER_COMPOSE_RUN_ARGS) $(PROJECT_NAME)-devel \
 	    make -e PYTHON_MINORS="$(PYTHON_MINOR)" build-requirements-$(PYTHON_ENV)
 ifeq ($(CI),true)
 # On CI, any changes from compiling requirements is a failure so no need to waste time
 # rebuilding images:
 	touch "$(@)"
 else
 	$(MAKE) -e "$(@)"
 endif
 
 # Build the end-user image:
-./var/docker/$(PYTHON_ENV)/log/build-user.log: \
-		./var/docker/$(PYTHON_ENV)/log/build-devel.log ./Dockerfile \
-		./var/docker/$(PYTHON_ENV)/log/rebuild.log
+./var-docker/$(PYTHON_ENV)/log/build-user.log: \
+		./var-docker/$(PYTHON_ENV)/log/build-devel.log ./Dockerfile \
+		./.dockerignore ./bin/entrypoint ./build-host/requirements.txt.in \
+		./var-docker/$(PYTHON_ENV)/log/rebuild.log
 	true DEBUG Updated prereqs: $(?)
 ifeq ($(PYTHON_WHEEL),)
 	$(MAKE) -e "build-pkgs"
 	PYTHON_WHEEL="$$(ls -t ./dist/*.whl | head -n 1)"
 endif
 # Build the end-user image now that all required artifacts are built"
 	mkdir -pv "$(dir $(@))"
 	$(MAKE) -e DOCKER_BUILD_ARGS="$(DOCKER_BUILD_ARGS) --load \
 	--build-arg PYTHON_WHEEL=$${PYTHON_WHEEL}" build-docker-build >>"$(@)"
 # The image installs the host requirements, reflect that in the bind mount volumes
 	date >>"$(@:%/build-user.log=%/host-install.log)"
 
-./var/ $(PYTHON_ENVS:%=./var/docker/%/) \
-./src/feed_archiver.egg-info/ \
-$(PYTHON_ENVS:%=./var/docker/%/feed_archiver.egg-info/) \
-./.tox/ $(PYTHON_ENVS:%=./var/docker/%/.tox/):
-	mkdir -pv "$(@)"
-
 # Marker file used to trigger the rebuild of the image for just one Python version.
 # Useful to workaround async timestamp issues when running jobs in parallel:
-./var/docker/$(PYTHON_ENV)/log/rebuild.log:
+./var-docker/$(PYTHON_ENV)/log/rebuild.log:
 	mkdir -pv "$(dir $(@))"
 	date >>"$(@)"
 
-# Local environment variables from a template:
-./.env: ./.env.in
-	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
-
-# Static site server set up
-./server/.htpasswd: .SHELLFLAGS = -eu -o pipefail -c
-./server/.htpasswd:
-	echo "Enter a HTTP Basic authentication password for the static site server."
-	if ! which htpasswd
-	then
-	    sudo apt-get update
-	    sudo apt-get install -y apache2-utils
-	fi
-	htpasswd -c "$(@)" "feed-archiver"
-
-# Extract the Sonarr API key
-./sonarr/config/config.xml: ./var/docker/$(PYTHON_ENV)/log/build.log
-	mkdir -pv "$(dir $(@))"
-	docker compose rm -sf sonarr
-	docker compose up -d sonarr
-	sleep 1
-	until [ -e "$(@)" ]
-	do
-	    sleep 0.1
-	done
-
-./src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml: \
-		./src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in \
-		./sonarr/config/config.xml
-	export SONARR_API_KEY=$$(
-	    sed -nE 's|.*<ApiKey>(.+)</ApiKey>.*|\1|p' "./sonarr/config/config.xml"
-	)
-	$(MAKE) "template=$(<)" "target=$(@)" expand-template
+# Local environment variables and secrets from a template:
+./.env.~out~: ./.env.in
+	$(call expand_template,$(<),$(@))
 
 # Install all tools required by recipes that have to be installed externally on the
 # host.  Use a target file outside this checkout to support multiple checkouts.  Use a
 # target specific to this project so that other projects can use the same approach but
 # with different requirements.
-$(HOME)/.local/var/log/feed-archiver-host-install.log:
+$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log: ./bin/host-install \
+		./build-host/requirements.txt.in
 	mkdir -pv "$(dir $(@))"
-# Bootstrap the minimum Python environment
-	(
-	    if ! which pip
-	    then
-	        if which apk
-	        then
-	            sudo apk update
-	            sudo apk add "gettext" "py3-pip" "gnupg" "github-cli" "curl"
-	        elif which apt-get
-	        then
-	            sudo apt-get update
-	            sudo apt-get install -y \
-	                "gettext-base" "python3-pip" "gnupg" "gh" "curl"
-	        else
-	            set +x
-	            echo "ERROR: OS not supported for installing host dependencies"
-	            false
-	        fi
-	    fi
-	    if [ -e ./build-host/requirements-$(PYTHON_HOST_ENV).txt ]
-	    then
-	        pip install -r "./build-host/requirements-$(PYTHON_HOST_ENV).txt"
-	    else
-	        pip install -r "./build-host/requirements.txt.in"
-	    fi
-	) |& tee -a "$(@)"
+	"$(<)" |& tee -a "$(@)"
 
 # https://docs.docker.com/build/building/multi-platform/#building-multi-platform-images
 $(HOME)/.local/var/log/docker-multi-platform-host-install.log:
 	mkdir -pv "$(dir $(@))"
 	if ! docker context inspect "multi-platform" |& tee -a "$(@)"
 	then
 	    docker context create "multi-platform" |& tee -a "$(@)"
@@ -1271,26 +1235,26 @@
 	then
 # If the local branch doesn't exist, fall back to the pre-release branch:
 	    git fetch $${git_fetch_args} "$${branch_path%%/*}" "develop" |&
 	        tee -a "$(@)"
 	fi
 
 ./.git/hooks/pre-commit:
-	$(MAKE) -e "$(HOME)/.local/var/log/feed-archiver-host-install.log"
+	$(MAKE) -e "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
 	$(TOX_EXEC_BUILD_ARGS) -- pre-commit install \
 	    --hook-type "pre-commit" --hook-type "commit-msg" --hook-type "pre-push"
 
 # Capture any project initialization tasks for reference.  Not actually usable.
 ./pyproject.toml:
-	$(MAKE) -e "$(HOME)/.local/var/log/feed-archiver-host-install.log"
+	$(MAKE) -e "$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log"
 	$(TOX_EXEC_BUILD_ARGS) -- cz init
 
 # Tell Emacs where to find checkout-local tools needed to check the code.
-./.dir-locals.el: ./.dir-locals.el.in
-	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
+./.dir-locals.el.~out~: ./.dir-locals.el.in
+	$(call expand_template,$(<),$(@))
 
 # Ensure minimal VCS configuration, mostly useful in automation such as CI.
 ~/.gitconfig:
 	git config --global user.name "$(USER_FULL_NAME)"
 	git config --global user.email "$(USER_EMAIL)"
 
 ./var/log/git-remotes.log:
@@ -1319,59 +1283,50 @@
 	set +x
 	echo "ERROR: PROJECT_GITHUB_PAT missing from ./.env or CI secrets"
 	false
 endif
 endif
 	set -x
 # Fail fast if there's still no push access
-	git push --no-verify --tags "origin" | tee -a "$(@)"
+	git push --no-verify "origin" "HEAD:$(VCS_BRANCH)" | tee -a "$(@)"
 
 # Ensure release publishing authentication, mostly useful in automation such as CI.
-~/.pypirc: ./home/.pypirc.in
-	$(MAKE) -e "template=$(<)" "target=$(@)" expand-template
+~/.pypirc.~out~: ./home/.pypirc.in
+	$(call expand_template,$(<),$(@))
 
-./var/log/docker-login-DOCKER.log: ./.env
+./var/log/docker-login-DOCKER.log:
+	$(MAKE) "./.env.~out~"
 	mkdir -pv "$(dir $(@))"
-	set +x
-	source "./.env"
-	export DOCKER_PASS
 	if [ -n "$${DOCKER_PASS}" ]
 	then
-	    set -x
-	    printenv "DOCKER_PASS" | docker login -u "merpatterson" --password-stdin
+	    printenv "DOCKER_PASS" | docker login -u "$(DOCKER_USER)" --password-stdin
 	elif [ "$(CI_IS_FORK)" != "true" ]
 	then
 	    echo "ERROR: DOCKER_PASS missing from ./.env or CI secrets"
 	    false
 	fi
 	date | tee -a "$(@)"
-./var/log/docker-login-GITLAB.log: ./.env
+./var/log/docker-login-GITLAB.log:
+	$(MAKE) "./.env.~out~"
 	mkdir -pv "$(dir $(@))"
-	set +x
-	source "./.env"
-	export CI_REGISTRY_PASSWORD
 	if [ -n "$${CI_REGISTRY_PASSWORD}" ]
 	then
-	    set -x
 	    printenv "CI_REGISTRY_PASSWORD" |
 	        docker login -u "$(CI_REGISTRY_USER)" --password-stdin "$(CI_REGISTRY)"
 	elif [ "$(CI_IS_FORK)" != "true" ]
 	then
 	    echo "ERROR: CI_REGISTRY_PASSWORD missing from ./.env or CI secrets"
 	    false
 	fi
 	date | tee -a "$(@)"
-./var/log/docker-login-GITHUB.log: ./.env
+./var/log/docker-login-GITHUB.log:
+	$(MAKE) "./.env.~out~"
 	mkdir -pv "$(dir $(@))"
-	set +x
-	source "./.env"
-	export PROJECT_GITHUB_PAT
 	if [ -n "$${PROJECT_GITHUB_PAT}" ]
 	then
-	    set -x
 	    printenv "PROJECT_GITHUB_PAT" |
 	        docker login -u "$(GITHUB_REPOSITORY_OWNER)" --password-stdin "ghcr.io"
 	elif [ "$(CI_IS_FORK)" != "true" ]
 	then
 	    echo "ERROR: PROJECT_GITHUB_PAT missing from ./.env or CI secrets"
 	    false
 	fi
@@ -1382,31 +1337,34 @@
 ./server/.htpasswd:
 	echo "Enter a HTTP Basic authentication password for the static site server."
 	if ! which htpasswd
 	then
 	    sudo apt-get update
 	    sudo apt-get install -y apache2-utils
 	fi
-	htpasswd -c "$(@)" "feed-archiver"
+	htpasswd -c "$(@)" "$(PROJECT_NAME)"
 
 # Extract the Sonarr API key
-./sonarr/config/config.xml: ./var/log/docker-build.log
+./sonarr/config/config.xml: ./var/docker/$(PYTHON_ENV)/log/build.log
+	mkdir -pv "$(dir $(@))"
+	docker compose rm -sf sonarr
 	docker compose up -d sonarr
 	sleep 1
 	until [ -e "$(@)" ]
 	do
 	    sleep 0.1
 	done
-./src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml: \
-		./src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in \
+
+./src/$(PYTHON_PROJECT_PACKAGE)/tests/archives/end-to-end/.$(PROJECT_NAME).yml.~out~: \
+		./src/$(PYTHON_PROJECT_PACKAGE)/tests/archives/end-to-end/.$(PROJECT_NAME).yml.in \
 		./sonarr/config/config.xml
 	export SONARR_API_KEY=$$(
 	    sed -nE 's|.*<ApiKey>(.+)</ApiKey>.*|\1|p' "./sonarr/config/config.xml"
 	)
-	$(MAKE) "template=$(<)" "target=$(@)" expand-template
+	$(call expand_template,$(<),$(@))
 
 # GPG signing key creation and management in CI
 export GPG_PASSPHRASE=
 GPG_SIGNING_PRIVATE_KEY=
 ./var/ci-cd-signing-subkey.asc:
 # We need a private key in the CI/CD environment for signing release commits and
 # artifacts.  Use a subkey so that it can be revoked without affecting your main key.
@@ -1461,70 +1419,65 @@
 endif
 
 ./var/gitlab-runner/config/config.toml: ./gitlab-runner/config/config.toml.in
 	docker compose run --rm gitlab-runner register \
 	    --url "https://gitlab.com/" --docker-image "docker" --executor "docker"
 
 
-## Utility Targets:
+## Makefile "functions":
 #
-# Recipes used to make similar changes across targets where using Make's basic syntax
-# can't be used.
-
-.PHONY: expand-template
-## Create a file from a template replacing environment variables
-expand-template:
-	$(MAKE) -e "$(HOME)/.local/var/log/feed-archiver-host-install.log"
-	set +x
-	if [ -e "$(target)" ]
-	then
-ifeq ($(TEMPLATE_IGNORE_EXISTING),true)
-	    exit
-else
-	    envsubst <"$(template)" | diff -u "$(target)" "-" || true
-	    echo "ERROR: Template $(template) has been updated:"
-	    echo "       Reconcile changes and \`$$ touch $(target)\`:"
-	    false
-endif
-	fi
-	envsubst <"$(template)" >"$(target)"
-
-.PHONY: pull-docker
-### Pull an existing image best to use as a cache for building new images
-pull-docker: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
-		./var/log/tox/build/build.log
-	export VERSION=$$(./.tox/build/bin/cz version --project)
-	for vcs_branch in $(VCS_BRANCHES)
-	do
-	    docker_tag="$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${vcs_branch}"
-	    for docker_image in $(DOCKER_IMAGES)
-	    do
-	        if docker pull "$${docker_image}:$${docker_tag}"
-	        then
-	            docker tag "$${docker_image}:$${docker_tag}" \
-	                "$(DOCKER_IMAGE_DOCKER):$${docker_tag}"
-	            exit
-	        fi
-	    done
-	done
-	set +x
-	echo "ERROR: Could not pull any existing docker image"
-	false
+# Snippets whose output is frequently used including across recipes:
+# https://www.gnu.org/software/make/manual/html_node/Call-Function.html
 
-.PHONY: bootstrap-project
-### Run any tasks needed to be run once for a given project by a maintainer
-bootstrap-project: \
-		./var/log/docker-login-GITLAB.log \
-		./var/log/docker-login-GITHUB.log
-# Initially seed the build host Docker image to bootstrap CI/CD environments
-# GitLab CI/CD:
-	$(MAKE) -e -C "./build-host/" DOCKER_IMAGE="$(DOCKER_IMAGE_GITLAB)" release
-# GitHub Actions:
-	$(MAKE) -e -C "./build-host/" DOCKER_IMAGE="$(DOCKER_IMAGE_GITHUB)" release
+# Return the most recently built package:
+current_pkg=$(shell ls -t ./dist/*$(1) | head -n 1)
 
+# Have to use a placeholder `*.~out~` as the target instead of the real expanded
+# template because we can't disable `.DELETE_ON_ERROR` on a per-target basis.
+#
+# Short-circuit/repeat the host-install recipe here because expanded templates should
+# *not* be updated when `./bin/host-install` is, so we can't use it as a prerequisite,
+# *but* it is required to expand templates.  We can't use a sub-make because any
+# expanded templates we use in `include ...` directives, such as `./.env`, are updated
+# as targets when reading the `./Makefile` leading to endless recursion.
+define expand_template=
+if ! which envsubst
+then
+    mkdir -pv "$(HOME)/.local/var/log/"
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
+fi
+if [ "$(CI)" != "true" ]
+then
+    envsubst <"$(1)" | diff -u "$(2:%.~out~=%)" "-" || true
+fi
+set +x
+echo "WARNING:Template $(1) has been updated."
+echo "        Reconcile changes and \`$$ touch $(2:%.~out~=%)\`."
+set -x
+if [ ! -s "$(2:%.~out~=%)" ]
+then
+    envsubst <"$(1)" >"$(2:%.~out~=%)"
+    touch -d "@0" "$(2:%.~out~=%)"
+fi
+if [ "$(TEMPLATE_IGNORE_EXISTING)" == "true" ]
+then
+    envsubst <"$(1)" >"$(2)"
+    exit
+fi
+exit 1
+endef
 
 ## Makefile Development:
 #
 # Development primarily requires a balance of 2 priorities:
 #
 # - Ensure the correctness of the code and build artifacts
 # - Minimize iteration time overhead in the inner loop of development
@@ -1595,7 +1548,45 @@
 #   Overriding variables on the command-line when invoking make as "options"
 #
 # We want to avoid, however, using many more features of Make, particularly the more
 # "magical" features, to keep it readable, discover-able, and otherwise accessible to
 # developers who may not have significant familiarity with Make.  If there's a good,
 # pragmatic reason to add use of further features feel free to make the case but avoid
 # them if possible.
+
+
+## Maintainer targets:
+#
+# Recipes not used during the normal course of development.
+
+.PHONY: pull-docker
+### Pull an existing image best to use as a cache for building new images
+pull-docker: ./var/git/refs/remotes/$(VCS_REMOTE)/$(VCS_BRANCH) \
+		$(HOME)/.local/var/log/$(PROJECT_NAME)-host-install.log
+	export VERSION=$$($(TOX_EXEC_BUILD_ARGS) -qq -- cz version --project)
+	for vcs_branch in $(VCS_BRANCHES)
+	do
+	    docker_tag="$(DOCKER_VARIANT_PREFIX)$(PYTHON_ENV)-$${vcs_branch}"
+	    for docker_image in $(DOCKER_IMAGES)
+	    do
+	        if docker pull "$${docker_image}:$${docker_tag}"
+	        then
+	            docker tag "$${docker_image}:$${docker_tag}" \
+	                "$(DOCKER_IMAGE_DOCKER):$${docker_tag}"
+	            exit
+	        fi
+	    done
+	done
+	set +x
+	echo "ERROR: Could not pull any existing docker image"
+	false
+
+.PHONY: bootstrap-project
+### Run any tasks needed to be run once for a given project by a maintainer
+bootstrap-project: \
+		./var/log/docker-login-GITLAB.log \
+		./var/log/docker-login-GITHUB.log
+# Initially seed the build host Docker image to bootstrap CI/CD environments
+# GitLab CI/CD:
+	$(MAKE) -e -C "./build-host/" DOCKER_IMAGE="$(DOCKER_IMAGE_GITLAB)" release
+# GitHub Actions:
+	$(MAKE) -e -C "./build-host/" DOCKER_IMAGE="$(DOCKER_IMAGE_GITHUB)" release
```

### Comparing `feed-archiver-2.0.4/NEWS.rst` & `feed-archiver-2.0.6b1/NEWS.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+feed-archiver 2.0.6b1 (2023-05-10)
+==================================
+
+Bugfixes
+--------
+
+- Restore Python 3.7 compatibility following a dependency upgrade in v2.0.1b0.
+- Upgrade all requirements to the latest versions as of Tue May  9 09:31:01 PM UTC 2023.
+
+
+feed-archiver 2.0.6b0 (2023-05-09)
+==================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Sun May  7 09:27:36 AM UTC 2023.
+
+
+feed-archiver 2.0.5 (2023-05-07)
+================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Sun May  7 16:01:06 UTC 2023.
+
+
 feed-archiver 2.0.4 (2023-04-29)
 ================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Sat Apr 29 16:01:07 UTC 2023.
@@ -79,14 +107,16 @@
 
 Feedarchiver 1.0.0b10 (2023-03-15)
 ==================================
 
 Features
 --------
 
+- Add support for a fallback link configurations that take effect if no other
+  configurations link the enclosure.
 - Address a Bandit warning about requests without timeouts.
 - Write an ``./index.html`` file listing links to archived feeds.
 - Rename the ``link-paths`` plugin system to a more accurate name, ``enclosures``.  Note
   that this requires an update to existing archive configurations using ``link-paths``
   plugins.
 - Replace ``content`` term with more correct ``enclosure`` term.  Requires running the ``$
   feed-archiver relink`` sub-command to update existing archives.
```

### Comparing `feed-archiver-2.0.4/PKG-INFO` & `feed-archiver-2.0.6b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.4
+Version: 2.0.6b1
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: devel
-License-File: LICENSE
+
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
 
 ########################################################################################
 Feed Archiver
 ########################################################################################
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/feed-archiver.svg?logo=pypi&label=PyPI&logoColor=gold
-	  :alt: PyPI latest release version
-	  :target: https://pypi.org/project/feed-archiver/
-       .. figure:: https://img.shields.io/pypi/dm/feed-archiver.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-	  :alt: PyPI downloads per month
-	  :target: https://pypi.org/project/feed-archiver/
+          :alt: PyPI latest release version
+          :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/pyversions/feed-archiver.svg?logo=python&label=Python&logoColor=gold
-	  :alt: PyPI Python versions
-	  :target: https://pypi.org/project/feed-archiver/
+          :alt: PyPI Python versions
+          :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
-	  :alt: Python code style
-	  :target: https://github.com/psf/black
+          :alt: Python code style
+          :target: https://github.com/psf/black
+       .. figure:: https://api.reuse.software/badge/gitlab.com/rpatterson/feed-archiver
+          :alt: REUSE license status
+          :target: https://api.reuse.software/info/gitlab.com/rpatterson/feed-archiver
 
      - .. figure:: https://gitlab.com/rpatterson/feed-archiver/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/feed-archiver/-/releases
        .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
           :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
@@ -78,18 +82,18 @@
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/feed-archiver?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
-	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
+          :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
-	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
+          :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
      - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
           :alt: KeyBase PGP key ID
           :target: https://keybase.io/rpatterson
        .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
           :alt: GitHub followers count
           :target: https://github.com/rpatterson
@@ -186,16 +190,14 @@
 re-using example configurations known to work by others.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
-Install and use either via a local, native installation or a Docker container image:
-
 Local/Native Installation
 ========================================================================================
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ pip3 install --user feed-archiver
 
@@ -208,30 +210,30 @@
 `the example ./docker-compose.yml file`_ for an example configuration.  Once you have
 your configuration, you can create and run the container::
 
   $ docker compose up
 
 Alternatively, you make use the image directly.  Pull `the Docker image`_::
 
-  $ docker pull "registry.gitlab.org/rpatterson/feed-archiver"
+  $ docker pull "registry.gitlab.com/rpatterson/feed-archiver"
 
 And then use the image to create and run a container::
 
-  $ docker run --rm -it "registry.gitlab.org/rpatterson/feed-archiver" ...
+  $ docker run --rm -it "registry.gitlab.com/rpatterson/feed-archiver" ...
 
 Images variant tags are published for the Python version, branch, and major/minor
 versions so that users can control when they get new images over time,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-main``.  The canonical
-Python version is 3.10 which is the version used in tags without ``py###``,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:main``.  Pre-releases are from
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310-main``.  The canonical Python
+version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:main``.  Pre-releases are from
 ``develop`` and final releases are from ``main`` which is also the default for tags
-without a branch, e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310``. The
+without a branch, e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310``. The
 major/minor version tags are only applied to the final release images and without the
 corresponding ``main`` branch tag,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-v0.8``.
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310-v0.8``.
 
 Multi-platform Docker images are published containing images for the following
 platforms or architectures in the Python 3.10 ``py310`` variant:
 
 - ``linux/amd64``
 - ``linux/arm64``
 - ``linux/arm/v7``
```

### Comparing `feed-archiver-2.0.4/README.rst` & `feed-archiver-2.0.6b1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
+
 ########################################################################################
 Feed Archiver
 ########################################################################################
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/feed-archiver.svg?logo=pypi&label=PyPI&logoColor=gold
-	  :alt: PyPI latest release version
-	  :target: https://pypi.org/project/feed-archiver/
-       .. figure:: https://img.shields.io/pypi/dm/feed-archiver.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-	  :alt: PyPI downloads per month
-	  :target: https://pypi.org/project/feed-archiver/
+          :alt: PyPI latest release version
+          :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/pyversions/feed-archiver.svg?logo=python&label=Python&logoColor=gold
-	  :alt: PyPI Python versions
-	  :target: https://pypi.org/project/feed-archiver/
+          :alt: PyPI Python versions
+          :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
-	  :alt: Python code style
-	  :target: https://github.com/psf/black
+          :alt: Python code style
+          :target: https://github.com/psf/black
+       .. figure:: https://api.reuse.software/badge/gitlab.com/rpatterson/feed-archiver
+          :alt: REUSE license status
+          :target: https://api.reuse.software/info/gitlab.com/rpatterson/feed-archiver
 
      - .. figure:: https://gitlab.com/rpatterson/feed-archiver/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/feed-archiver/-/releases
        .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
           :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
@@ -50,18 +54,18 @@
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/feed-archiver?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
-	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
+          :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
-	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
+          :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
      - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
           :alt: KeyBase PGP key ID
           :target: https://keybase.io/rpatterson
        .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
           :alt: GitHub followers count
           :target: https://github.com/rpatterson
@@ -158,16 +162,14 @@
 re-using example configurations known to work by others.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
-Install and use either via a local, native installation or a Docker container image:
-
 Local/Native Installation
 ========================================================================================
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ pip3 install --user feed-archiver
 
@@ -180,30 +182,30 @@
 `the example ./docker-compose.yml file`_ for an example configuration.  Once you have
 your configuration, you can create and run the container::
 
   $ docker compose up
 
 Alternatively, you make use the image directly.  Pull `the Docker image`_::
 
-  $ docker pull "registry.gitlab.org/rpatterson/feed-archiver"
+  $ docker pull "registry.gitlab.com/rpatterson/feed-archiver"
 
 And then use the image to create and run a container::
 
-  $ docker run --rm -it "registry.gitlab.org/rpatterson/feed-archiver" ...
+  $ docker run --rm -it "registry.gitlab.com/rpatterson/feed-archiver" ...
 
 Images variant tags are published for the Python version, branch, and major/minor
 versions so that users can control when they get new images over time,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-main``.  The canonical
-Python version is 3.10 which is the version used in tags without ``py###``,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:main``.  Pre-releases are from
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310-main``.  The canonical Python
+version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:main``.  Pre-releases are from
 ``develop`` and final releases are from ``main`` which is also the default for tags
-without a branch, e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310``. The
+without a branch, e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310``. The
 major/minor version tags are only applied to the final release images and without the
 corresponding ``main`` branch tag,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-v0.8``.
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310-v0.8``.
 
 Multi-platform Docker images are published containing images for the following
 platforms or architectures in the Python 3.10 ``py310`` variant:
 
 - ``linux/amd64``
 - ``linux/arm64``
 - ``linux/arm/v7``
```

### Comparing `feed-archiver-2.0.4/TODO.rst` & `feed-archiver-2.0.6b1/TODO.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
+
 ########################################################################################
 Seeking Contributions
 ########################################################################################
 
 Known bugs and desirable features for which contributions are most welcome.
```

### Comparing `feed-archiver-2.0.4/bin/cz-check-bump` & `feed-archiver-2.0.6b1/bin/cz-check-bump`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python3
+
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Check if the conventional commits since the last release require a new release.
 
 Works around Commitizen's version handling when bumping from a pre-release:
 
 https://github.com/commitizen-tools/commitizen/issues/688#issue-1628052526
 """
```

### Comparing `feed-archiver-2.0.4/bin/entrypoint` & `feed-archiver-2.0.6b1/bin/entrypoint`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/bin/bash
+
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 #
 # Perform any required volatile run-time initialization
 
 set -eu -o pipefail
 shopt -s inherit_errexit
 if [ "${DEBUG:=false}" = "true" ]
 then
@@ -21,16 +26,16 @@
 	    echo "ERROR: Can't create a user when not run as root" 1>&2
 	    false
 	fi
 	if ! id "${PUID}" >"/dev/null" 2>&1
 	then
 	    # Add a user to the `passwd` DB so that the `~feed-archiver/`
 	    # HOME directory can be looked up.
-	    adduser --uid "${PUID}" --disabled-password --gecos \
-		    "Feed Archiver,,," "feed-archiver" >"/dev/null"
+	    adduser --uid "${PUID}" --disabled-password \
+	        --gecos "Feed Archiver,,," "feed-archiver" >"/dev/null"
 	fi
 	# Fix the TTY ownership if the session is interactive
 	if tty_dev=$(tty)
 	then
 	    chown "${PUID}" "${tty_dev}"
 	fi
 	# Delegate the rest to the `CMD`
```

### Comparing `feed-archiver-2.0.4/bin/get-base-version` & `feed-archiver-2.0.6b1/bin/get-base-version`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python
+
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Return the current version minus any pre-release suffix along with it's type.
 
 Useful to get the final/stable version when the previous pre-release has been blessed as
 ready for publishing as final.
 """  # pylint: disable=invalid-name
```

### Comparing `feed-archiver-2.0.4/build-host/Dockerfile` & `feed-archiver-2.0.6b1/build-host/Dockerfile`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Container image in which to build, test, and release the project
 
 # I *want* something to break to let me know if something changes in the latest version
 # of the base image changes something:
 # hadolint ignore=DL3007
 FROM docker:latest
 
@@ -18,32 +22,36 @@
     "py3-pip" \
     "gnupg" \
     "curl" \
     "tar" \
     "github-cli" \
     && rm -rf /var/cache/apk/*
 
+# Project contstants:
+ARG PROJECT_NAMESPACE=rpatterson
+ARG PROJECT_NAME=feed-archiver
+
 # Find the same home directory even when run as another user, e.g. `root`.
 ENV HOME="/home/runner"
 # Add user installs to PATH
 ENV PATH="${HOME}/.local/bin:${PATH}"
 
 COPY [ "./requirements-py310.txt", "${HOME}/.local/lib/" ]
 RUN mkdir -pv "${HOME}/.local/var/log/" && \
-    pip install --no-cache-dir --user -r "${HOME}/.local/lib/requirements-py310.txt" \
-    >"${HOME}/.local/var/log/feed-archiver-host-install.log"
+    pip3 install --no-cache-dir --user -r "${HOME}/.local/lib/requirements-py310.txt" \
+    >"${HOME}/.local/var/log/${PROJECT_NAME}-host-install.log"
 
 COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
 ENTRYPOINT [ "docker-entrypoint.sh", "entrypoint" ]
 CMD [ "make", "-e", "build-docker" ]
 
 # https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
-LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/feed-archiver"
-LABEL org.opencontainers.image.documentation="https://gitlab.com/rpatterson/feed-archiver"
-LABEL org.opencontainers.image.source="https://gitlab.com/rpatterson/feed-archiver"
+LABEL org.opencontainers.image.url="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECT_NAME}"
+LABEL org.opencontainers.image.documentation="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECT_NAME}"
+LABEL org.opencontainers.image.source="https://gitlab.com/${PROJECT_NAMESPACE}/${PROJECT_NAME}"
 LABEL org.opencontainers.image.title="Feed Archiver Build Host"
 LABEL org.opencontainers.image.description="Feed Archiver build host"
 LABEL org.opencontainers.image.licenses="MIT"
 LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
 LABEL org.opencontainers.image.vendor="rpatterson.net"
 LABEL org.opencontainers.image.base.name="docker.io/library/docker:latest"
 # Build-time `LABEL`s
```

### Comparing `feed-archiver-2.0.4/build-host/Makefile` & `feed-archiver-2.0.6b1/build-host/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 ## Build and publish an image in which to build, test, and release the project
 
 ### Defensive settings for make:
 #     https://tech.davis-hansson.com/p/make/
 SHELL:=bash
 .ONESHELL:
 .SHELLFLAGS:=-eu -o pipefail -c
```

### Comparing `feed-archiver-2.0.4/build-host/bin/entrypoint` & `feed-archiver-2.0.6b1/build-host/bin/entrypoint`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/bin/ash
+
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 #
 # Shared set up for local testing of CI/CD
 
 set -eu -o pipefail
 CHOWN_ARGS="-R"
 if [ "${DEBUG:=false}" = "true" ]
 then
```

### Comparing `feed-archiver-2.0.4/build-host/requirements-py310.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py310.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/build-host/requirements-py311.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py311.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/build-host/requirements-py37.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py37.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/build-host/requirements-py38.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py38.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/build-host/requirements-py39.txt` & `feed-archiver-2.0.6b1/build-host/requirements-py39.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/docker-compose-servarr.yml` & `feed-archiver-2.0.6b1/docker-compose-servarr.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Example Sonarr service to demonstrate the integration with Prunerr.
 #
 # In a separate file because integrating with Sonarr is optional.  See the comment above
 # `COMPOSE_FILE` in `./.env.in` for an example of how to add this file.
 version: "3.8"
 
 services:
```

### Comparing `feed-archiver-2.0.4/docker-compose.override.yml` & `feed-archiver-2.0.6b1/docker-compose.override.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,174 +1,182 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Override `$ docker compose ...` configuration for development or testing here in this
 # repo checkout.  Everything that may be used outside this checkout should be in
 # `./docker-compose.yml`.
 version: "3.8"
 
 services:
 
   # Configuration specific to development:
   feed-archiver:
     image: "\
-      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/feed-archiver\
-      :${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
-    container_name: "feed-archiver-checkout"
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/${PROJECT_NAMESPACE:?}\
+      /${PROJECT_NAME:?}:${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
+    container_name: "${PROJECT_NAME:?}-checkout"
     build:
-      context: "${CHECKOUT_DIR}/"
+      context: "${CHECKOUT_DIR:-.}/"
+      target: "user"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
     depends_on:
       # Don't force service dependencies on other deployments that extend the base
       - "ofelia"
     volumes:
       # Preserve caches caches between container runs
-      - "${CHECKOUT_DIR}/home/:/home/feed-archiver/"
+      - "${CHECKOUT_DIR:-.}/home/:/home/${PROJECT_NAME:?}/"
       # Specify the default archive within your media library
       - "${FEED_ARCHIVE:-/media/Library/feeds/}:${FEED_ARCHIVE:-/media/Library/feeds/}"
   # Allow use in development checkout alongside a real deployment, avoid name clash
   sonarr:
-    container_name: "feed-archiver-devel-sonarr"
+    container_name: "${PROJECT_NAME:-}-devel-sonarr"
     # Choose a port prefix unlikely to be in use from the ephemeral port range
     # https://en.wikipedia.org/wiki/Ephemeral_port#Range
     #     $ shuf -i 49-65 -n 1
     #     54
     ports:
       - "8989:54989"
   traefik:
-    container_name: "feed-archiver-devel-traefik"
+    container_name: "${PROJECT_NAME:-}-devel-traefik"
   nginx:
-    container_name: "feed-archiver-devel-nginx"
+    container_name: "${PROJECT_NAME:-}-devel-nginx"
     volumes:
       - "./nginx/templates/:/etc/nginx/templates/"
   ofelia:
-    container_name: "feed-archiver-devel-ofelia"
+    container_name: "${PROJECT_NAME:-}-devel-ofelia"
 
   ## Contianers used for development and release:
 
   # Container for use by developers:
   feed-archiver-devel:
     image: "\
-      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/feed-archiver\
-      :devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
-    container_name: "feed-archiver-devel"
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/${PROJECT_NAMESPACE:?}\
+      /${PROJECT_NAME:?}:devel-${PYTHON_ENV:-py310}-${DOCKER_BRANCH_TAG:-develop}"
+    container_name: "${PROJECT_NAME:?}-devel"
     profiles:
       - "test"
     build:
-      context: "${CHECKOUT_DIR}/"
-      dockerfile: "${CHECKOUT_DIR}/Dockerfile.devel"
+      context: "${CHECKOUT_DIR:-.}/"
+      target: "devel"
       args:
         PYTHON_MINOR: "${PYTHON_MINOR:-3.10}"
         PYTHON_ENV: "${PYTHON_ENV:-py310}"
         VERSION: "${VERSION:-}"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       # Make the run-time user configurable in `./.env`
       PUID: "${PUID:-1000}"
       PGID: "${PGID:-${PUID:-1000}}"
       # Variables from the environment we want to be passed through into the container:
       CI: "${CI:-false}"
       # DEBUG: "true"
     volumes:
       # Ensure local changes are reflected inside the container.
-      - "${CHECKOUT_DIR}/bin/entrypoint:/usr/local/bin/entrypoint"
-      - "${CHECKOUT_DIR}/:/usr/local/src/feed-archiver/"
+      - "${CHECKOUT_DIR:-.}/bin/entrypoint:/usr/local/bin/entrypoint"
+      - "${CHECKOUT_DIR:-.}/:/usr/local/src/${PROJECT_NAME:?}/"
       # Preserve caches caches between container runs
-      - "${CHECKOUT_DIR}/home/:/home/feed-archiver/"
+      - "${CHECKOUT_DIR:-.}/home/:/home/${PROJECT_NAME:?}/"
       # Avoid any clashes between image variants and/or the local host at both build and
       # run-time.
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/\
-        :/usr/local/src/feed-archiver/var/"
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}/.tox/\
-        :/usr/local/src/feed-archiver/.tox/"
-      - "${CHECKOUT_DIR}/var/docker/${PYTHON_ENV:-py310}\
+      - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}/\
+        :/usr/local/src/${PROJECT_NAME:?}/var/"
+      - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}/.tox/\
+        :/usr/local/src/${PROJECT_NAME:?}/.tox/"
+      - "${CHECKOUT_DIR:-.}/var-docker/${PYTHON_ENV:-py310}\
         /feed_archiver.egg-info/\
-        :/usr/local/src/feed-archiver/src/feed_archiver.egg-info/"
+        :/usr/local/src/${PROJECT_NAME:?}/src/feed_archiver.egg-info/"
 
   # https://github.com/hadolint/hadolint#how-to-use
   hadolint:
     image: "ghcr.io/hadolint/hadolint"
     profiles:
       - "test"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
-      - "${CHECKOUT_DIR}/:/usr/local/src/feed-archiver/"
-    working_dir: "/usr/local/src/feed-archiver/"
+      - "${CHECKOUT_DIR:-.}/:/usr/local/src/${PROJECT_NAME:-}/"
+    working_dir: "/usr/local/src/${PROJECT_NAME:-}/"
     command: >-
       hadolint "./Dockerfile"
 
   pandoc:
     image: "pandoc/core"
     profiles:
       - "release"
     user: "${PUID:-1000}:${PGID:-${PUID:-1000}}"
     environment:
       TZ: "${TZ:-Etc/UTC}"
     volumes:
-      - "${CHECKOUT_DIR}/:/data/"
+      - "${CHECKOUT_DIR:-.}/:/data/"
     entrypoint: "ash"
-    # Strip reStructuredText directives unsupported in Markdown:
+    # Strip reStructuredText directives unsupported in Markdown before converting and
+    # converted Markdown that isn't widely supported, e.g. table of contents and tables
+    # respectively:
     command: >-
       -xeu -c '
         grep -Ev "^ *\.\. +(contents)::.*" "./README.rst" |
-        pandoc -f "rst" -t "markdown" -o "./var/README.md"
+        pandoc -f "rst" -t "gfm" | grep -Ev "^(\+-+\+|\|.*\|)$" >"./README.md"
       '
 
   docker-pushrm:
     image: "chko/docker-pushrm"
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
-      - "${CHECKOUT_DIR}/:/data/"
+      - "${CHECKOUT_DIR:-.}/:/data/"
     command: >-
-      --file "/data/var/README.md"
-      --short "feed archiver foundation or template"
-      --debug "merpatterson/feed-archiver"
+      --file "/data/README.md"
+      --short "Archive the full contents of RSS/Atom syndication feeds including
+      enclosures and assets."
+      --debug "${DOCKER_USER:-}/${PROJECT_NAME:-}"
 
   gitlab-release-cli:
     image: "${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/gitlab-org/release-cli:latest"
     profiles:
       - "release"
     environment:
       CI_JOB_TOKEN: "${CI_JOB_TOKEN:-}"
     volumes:
-      - "./:/usr/local/src/feed-archiver/"
-    working_dir: "/usr/local/src/feed-archiver/"
+      - "./:/usr/local/src/${PROJECT_NAME:-}/"
+    working_dir: "/usr/local/src/${PROJECT_NAME:-}/"
 
   ## Containers related to CI/CD:
 
   # The container in which CI/CD is run:
   build-host:
     image: "\
-      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/rpatterson/feed-archiver\
+      ${DOCKER_REGISTRY_HOST:-registry.gitlab.com}/${DOCKER_USER:-}/${PROJECT_NAME:-}\
       :build-host"
     profiles:
       - "ci"
-    build: "${CHECKOUT_DIR}/build-host/"
+    build: "${CHECKOUT_DIR:-.}/build-host/"
     privileged: true
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
-      - "${CHECKOUT_DIR}/:${CHECKOUT_DIR}"
-      - "${CHECKOUT_DIR}/build-host/bin/entrypoint:/usr/local/bin/entrypoint"
+      - "${CHECKOUT_DIR:-.}/:${CHECKOUT_DIR:-.}"
+      - "${CHECKOUT_DIR:-.}/build-host/bin/entrypoint:/usr/local/bin/entrypoint"
       # Share local SSH authentication to repository remotes
       - "~/.ssh/:/home/runner/.ssh/"
     env_file: "./.env"
     environment:
       TZ: "${TZ:-Etc/UTC}"
       PUID: "${PUID:-1000}"
       PGID: "${DOCKER_GID:-${PGID:-${PUID:-1000}}}"
       # DEBUG: "true"
-    working_dir: "${CHECKOUT_DIR}"
+    working_dir: "${CHECKOUT_DIR:-.}"
     command: >-
       make -e build-docker test-docker release
 
   gitlab-runner:
     profiles:
       - "ci"
```

### Comparing `feed-archiver-2.0.4/docker-compose.yml` & `feed-archiver-2.0.6b1/docker-compose.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
+# Minimal `$ docker compose ...` configuration to demonstrate the requirements for
+# running feed-archiver in containers.
 version: "3.8"
 
 services:
 
   ## Container for use by end users:
   feed-archiver:
     image: "registry.gitlab.com/rpatterson/feed-archiver"
```

### Comparing `feed-archiver-2.0.4/gitlab-runner/config/config.toml.in` & `feed-archiver-2.0.6b1/gitlab-runner/config/config.toml.in`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Set to 2 times the number of parallel matrix jobs as a default.
 # Alternatively, set to the number of CPUs/cores or some multiple:
 concurrent = 10
 # Pick up jobs as soon as possible:
 check_interval = 1
 shutdown_timeout = 0
```

### Comparing `feed-archiver-2.0.4/nginx/templates/default.conf.template` & `feed-archiver-2.0.6b1/nginx/templates/default.conf.template`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 server {
     # FIXME: Should we find a way to switch to HTTPS so we can use HTTP/2
     listen ${NGINX_PORT} default_server;
     listen [::]:${NGINX_PORT} default_server;
     server_name ${NGINX_HOST};
 
     # Make browsing/discovery easier, serve indexes of directories:
```

### Comparing `feed-archiver-2.0.4/pyproject.toml` & `feed-archiver-2.0.6b1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,23 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 [build-system]
 # https://setuptools.pypa.io/en/latest/build_meta.html#how-to-use-it
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 # Use VCS tags as the sole authority on versions.  Dynamically determine the current
 # version from VCS tags:
 # https://github.com/pypa/setuptools_scm#pyprojecttoml-usage
 write_to = "src/feedarchiver/version.py"
 # Uncomment to test uploading to PyPI locally
 # local_scheme = "no-local-version"
-[tool.commitizen]
-# Parse commit messages according to conventional commits to decide wether the next
-# versin tag should be a major, minor or patch bump and create the VCS tag.  Also
-# provides VCS hooks to enforce that commit messages comply with conventional commits:
-# https://commitizen-tools.github.io/commitizen/
-name = "cz_conventional_commits"
-changelog_start_rev = "v0.0.0"
-version = "2.0.4"
-tag_format = "v$version"
-annotated_tag = true
-gpg_sign = true
-bump_message = """\
-build(release): Version $current_version → $new_version
-
-[actions skip]
-[ci release]
-"""
-[tool.towncrier]
-# https://towncrier.readthedocs.io/en/stable/#quick-start
-package = "feedarchiver"
-package_dir = "src"
-name = "feed-archiver"
 
 [tool.pylint.MASTER]
 # Ensure `duplicate-code` and any other errors that depend on not runnining in parallel
 # are reported:
 jobs = 1
 enable-all-extensions = true
 output-format = "colorized"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `feed-archiver-2.0.4/requirements/py310/build.txt` & `feed-archiver-2.0.6b1/requirements/py39/build.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.1
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
     #   commitizen
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
@@ -58,22 +58,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==3.3.1
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -83,41 +81,35 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
-typing-extensions==4.5.0
-    # via setuptools-scm
-urllib3==1.26.15
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
```

### Comparing `feed-archiver-2.0.4/requirements/py310/devel.txt` & `feed-archiver-2.0.6b1/requirements/py310/devel.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,71 +12,69 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==23.1.0
-    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via feed-archiver (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
-    #   pip-tools
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
-cfgv==3.3.1
-    # via pre-commit
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.4
+coverage==7.2.5
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
-distlib==0.3.6
-    # via virtualenv
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.12.0
-    # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -88,34 +86,32 @@
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
 httpcore==0.17.0
     # via httpx
 httpx==0.24.0
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   respx
-identify==2.5.23
-    # via pre-commit
+    # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
+license-expression==30.1.0
+    # via reuse
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 lxml-stubs==0.4.0
     # via feed-archiver (pyproject.toml)
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
@@ -127,43 +123,33 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-nodeenv==1.7.0
-    # via pre-commit
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via feed-archiver (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-    #   virtualenv
-pluggy==1.0.0
-    # via pytest
-pre-commit==3.2.2
-    # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -175,15 +161,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -198,40 +184,33 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   pytest-subtests
-pytest-subtests==0.10.0
-    # via feed-archiver (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   feed-archiver (pyproject.toml)
-    #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
-    #   requests-mock
+    #   reuse
     #   xenon
-requests-mock==1.10.0
-    # via feed-archiver (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
-respx==0.20.1
+reuse==1.0.0
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
@@ -244,15 +223,14 @@
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
-    #   requests-mock
     #   user-agent
 smmap==5.0.0
     # via gitdb
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
@@ -273,48 +251,42 @@
     #   autoflake
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
-    #   pytest
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.29
+trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.8
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.29.0.0
+types-requests==2.30.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.11
+types-urllib3==1.26.25.12
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
     #   mypy
     #   pydantic
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.23.0
-    # via pre-commit
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via feed-archiver (pyproject.toml)
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `feed-archiver-2.0.4/requirements/py310/user.txt` & `feed-archiver-2.0.6b1/requirements/py39/user.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py310/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py39/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
 argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
@@ -26,28 +26,32 @@
 httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
+importlib-metadata==6.6.0 ; python_version < "3.10"
+    # via feed-archiver (pyproject.toml)
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
     #   httpx
 tenacity==8.2.2
     # via feed-archiver (pyproject.toml)
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `feed-archiver-2.0.4/requirements/py311/build.txt` & `feed-archiver-2.0.6b1/requirements/py310/build.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.1
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
     #   commitizen
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
@@ -58,22 +58,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==3.3.1
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -83,39 +81,35 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
-typing-extensions==4.5.0
-    # via setuptools-scm
-urllib3==1.26.15
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
```

### Comparing `feed-archiver-2.0.4/requirements/py311/devel.txt` & `feed-archiver-2.0.6b1/requirements/py311/devel.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,69 +12,69 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==23.1.0
-    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via feed-archiver (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
-    #   pip-tools
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
-cfgv==3.3.1
-    # via pre-commit
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.4
+coverage==7.2.5
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
-distlib==0.3.6
-    # via virtualenv
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.12.0
-    # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -86,34 +86,32 @@
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
 httpcore==0.17.0
     # via httpx
 httpx==0.24.0
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   respx
-identify==2.5.23
-    # via pre-commit
+    # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
+license-expression==30.1.0
+    # via reuse
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 lxml-stubs==0.4.0
     # via feed-archiver (pyproject.toml)
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
@@ -125,43 +123,33 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-nodeenv==1.7.0
-    # via pre-commit
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via feed-archiver (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-    #   virtualenv
-pluggy==1.0.0
-    # via pytest
-pre-commit==3.2.2
-    # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -173,15 +161,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -196,40 +184,33 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   pytest-subtests
-pytest-subtests==0.10.0
-    # via feed-archiver (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   feed-archiver (pyproject.toml)
-    #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
-    #   requests-mock
+    #   reuse
     #   xenon
-requests-mock==1.10.0
-    # via feed-archiver (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
-respx==0.20.1
+reuse==1.0.0
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
@@ -242,15 +223,14 @@
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
-    #   requests-mock
     #   user-agent
 smmap==5.0.0
     # via gitdb
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
@@ -266,41 +246,36 @@
     #   prospector
     #   requirements-detector
     #   vulture
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.29
+trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.8
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.29.0.0
+types-requests==2.30.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.11
+types-urllib3==1.26.25.12
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   mypy
     #   pydantic
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.23.0
-    # via pre-commit
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via feed-archiver (pyproject.toml)
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `feed-archiver-2.0.4/requirements/py311/user.txt` & `feed-archiver-2.0.6b1/requirements/py38/user.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py311/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py38/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
 argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
@@ -26,28 +26,32 @@
 httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
+importlib-metadata==6.6.0 ; python_version < "3.10"
+    # via feed-archiver (pyproject.toml)
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
     #   httpx
 tenacity==8.2.2
     # via feed-archiver (pyproject.toml)
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `feed-archiver-2.0.4/requirements/py37/build.txt` & `feed-archiver-2.0.6b1/requirements/py38/build.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,50 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.1
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
-    #   argcomplete
     #   commitizen
     #   keyring
-    #   pre-commit
-    #   setuptools-scm
     #   twine
-    #   virtualenv
 importlib-resources==5.12.0
     # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
@@ -64,22 +60,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==2.21.0
+pre-commit==3.3.1
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -89,51 +83,41 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via
-    #   commitizen
-    #   importlib-metadata
-    #   markdown-it-py
-    #   platformdirs
-    #   rich
-    #   setuptools-scm
-urllib3==1.26.15
+    # via rich
+urllib3==2.0.2
     # via
     #   requests
     #   twine
-virtualenv==20.21.1
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via
```

### Comparing `feed-archiver-2.0.4/requirements/py37/devel.txt` & `feed-archiver-2.0.6b1/requirements/py37/devel.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,73 +12,71 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==23.1.0
-    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 backports-cached-property==1.0.2 ; python_version < "3.8"
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via feed-archiver (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
-    #   pip-tools
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
-cfgv==3.3.1
-    # via pre-commit
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.4
+coverage==7.2.5
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
-distlib==0.3.6
-    # via virtualenv
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.12.0
-    # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -90,49 +88,42 @@
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
 httpcore==0.17.0
     # via httpx
 httpx==0.24.0
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   respx
-identify==2.5.23
-    # via pre-commit
+    # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
-importlib-metadata==4.13.0 ; python_version < "3.8"
+importlib-metadata==4.13.0 ; python_version < "3.10"
     # via
     #   argcomplete
-    #   attrs
     #   build
     #   click
     #   feed-archiver (pyproject.toml)
-    #   pluggy
-    #   pre-commit
     #   pydocstyle
-    #   pytest
     #   rstcheck
     #   rstcheck-core
     #   stevedore
-    #   virtualenv
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
 isort==5.11.5
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
+license-expression==30.1.0
+    # via reuse
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 lxml-stubs==0.4.0
     # via feed-archiver (pyproject.toml)
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
@@ -144,43 +135,33 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-nodeenv==1.7.0
-    # via pre-commit
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via feed-archiver (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-    #   virtualenv
-pluggy==1.0.0
-    # via pytest
-pre-commit==2.21.0
-    # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -192,15 +173,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -215,40 +196,33 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   pytest-subtests
-pytest-subtests==0.10.0
-    # via feed-archiver (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   feed-archiver (pyproject.toml)
-    #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
-    #   requests-mock
+    #   reuse
     #   xenon
-requests-mock==1.10.0
-    # via feed-archiver (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
-respx==0.20.1
+reuse==1.0.0
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
@@ -261,15 +235,14 @@
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
-    #   requests-mock
     #   user-agent
 smmap==5.0.0
     # via gitdb
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
@@ -290,36 +263,35 @@
     #   autoflake
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
-    #   pytest
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.29
+trove-classifiers==2023.5.2
     # via pyroma
 typed-ast==1.5.4
     # via
     #   astroid
     #   black
     #   mypy
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.8
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.29.0.0
+types-requests==2.30.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.11
+types-urllib3==1.26.25.12
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   anyio
     #   astroid
     #   black
     #   gitpython
@@ -328,27 +300,22 @@
     #   mypy
     #   platformdirs
     #   pydantic
     #   pylint
     #   rich
     #   rstcheck
     #   rstcheck-core
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.21.1
-    # via pre-commit
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via feed-archiver (pyproject.toml)
 zipp==3.15.0
     # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `feed-archiver-2.0.4/requirements/py37/user.txt` & `feed-archiver-2.0.6b1/requirements/py37/user.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via httpcore
 argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
 backports-cached-property==1.0.2 ; python_version < "3.8"
     # via feed-archiver (pyproject.toml)
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
@@ -28,23 +28,23 @@
 httpx==0.24.0
     # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
-importlib-metadata==6.6.0 ; python_version < "3.8"
+importlib-metadata==6.6.0 ; python_version < "3.10"
     # via
     #   argcomplete
     #   feed-archiver (pyproject.toml)
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
@@ -54,13 +54,13 @@
 tenacity==8.2.2
     # via feed-archiver (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   anyio
     #   h11
     #   importlib-metadata
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `feed-archiver-2.0.4/requirements/py38/build.txt` & `feed-archiver-2.0.6b1/requirements/py311/build.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.1
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
     #   commitizen
     #   keyring
     #   twine
-importlib-resources==5.12.0
-    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -60,22 +58,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==3.3.1
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -85,52 +81,42 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
-typing-extensions==4.5.0
-    # via
-    #   rich
-    #   setuptools-scm
-urllib3==1.26.15
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `feed-archiver-2.0.4/requirements/py38/devel.txt` & `feed-archiver-2.0.6b1/requirements/py38/devel.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,71 +12,69 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==23.1.0
-    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via feed-archiver (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
-    #   pip-tools
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
-cfgv==3.3.1
-    # via pre-commit
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.4
+coverage==7.2.5
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
-distlib==0.3.6
-    # via virtualenv
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.12.0
-    # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -88,34 +86,34 @@
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
 httpcore==0.17.0
     # via httpx
 httpx==0.24.0
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   respx
-identify==2.5.23
-    # via pre-commit
+    # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
+importlib-metadata==6.6.0 ; python_version < "3.10"
+    # via feed-archiver (pyproject.toml)
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
+license-expression==30.1.0
+    # via reuse
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 lxml-stubs==0.4.0
     # via feed-archiver (pyproject.toml)
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
@@ -127,43 +125,33 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-nodeenv==1.7.0
-    # via pre-commit
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via feed-archiver (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-    #   virtualenv
-pluggy==1.0.0
-    # via pytest
-pre-commit==3.2.2
-    # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -175,15 +163,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -198,40 +186,33 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   pytest-subtests
-pytest-subtests==0.10.0
-    # via feed-archiver (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   feed-archiver (pyproject.toml)
-    #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
-    #   requests-mock
+    #   reuse
     #   xenon
-requests-mock==1.10.0
-    # via feed-archiver (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
-respx==0.20.1
+reuse==1.0.0
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
@@ -244,15 +225,14 @@
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
-    #   requests-mock
     #   user-agent
 smmap==5.0.0
     # via gitdb
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
@@ -273,51 +253,47 @@
     #   autoflake
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
-    #   pytest
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.29
+trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.8
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.29.0.0
+types-requests==2.30.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.11
+types-urllib3==1.26.25.12
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
     #   rich
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.23.0
-    # via pre-commit
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via feed-archiver (pyproject.toml)
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `feed-archiver-2.0.4/requirements/py38/user.txt` & `feed-archiver-2.0.6b1/requirements/py311/user.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py38/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --output-file=requirements/py311/user.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
 argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
 feedparser==6.0.10
@@ -30,24 +30,24 @@
     #   anyio
     #   httpx
     #   requests
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.29.0
+requests==2.30.0
     # via arrapi
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
     # via user-agent
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
     #   httpx
 tenacity==8.2.2
     # via feed-archiver (pyproject.toml)
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
```

### Comparing `feed-archiver-2.0.4/requirements/py39/build.txt` & `feed-archiver-2.0.6b1/requirements/py37/build.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
+#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
 argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.1
+commitizen==3.2.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
-decli==0.5.2
+decli==0.6.0
     # via commitizen
 distlib==0.3.6
     # via virtualenv
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 filelock==3.12.0
     # via virtualenv
-identify==2.5.23
+identify==2.5.24
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==4.13.0
+importlib-metadata==6.6.0
     # via
+    #   argcomplete
     #   commitizen
     #   keyring
+    #   pre-commit
     #   twine
+    #   virtualenv
+importlib-resources==5.12.0
+    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
@@ -58,22 +63,20 @@
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.1
-    # via
-    #   commitizen
-    #   setuptools-scm
+    # via commitizen
 pkginfo==1.9.6
     # via twine
 platformdirs==3.5.0
     # via virtualenv
-pre-commit==3.2.2
+pre-commit==2.21.0
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
@@ -83,48 +86,51 @@
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.29.0
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
 rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
-setuptools-scm==7.1.0
-    # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomli==2.0.1
-    # via setuptools-scm
 tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
-    # via setuptools-scm
-urllib3==1.26.15
+    # via
+    #   commitizen
+    #   importlib-metadata
+    #   markdown-it-py
+    #   platformdirs
+    #   rich
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `feed-archiver-2.0.4/requirements/py39/devel.txt` & `feed-archiver-2.0.6b1/requirements/py39/devel.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,71 +12,69 @@
     # via feed-archiver (pyproject.toml)
 astroid==2.15.4
     # via
     #   pylint
     #   pylint-celery
     #   pylint-flask
     #   requirements-detector
-attrs==23.1.0
-    # via pytest-subtests
 autoflake==1.7.8
     # via feed-archiver (pyproject.toml)
 autopep8==2.0.2
     # via feed-archiver (pyproject.toml)
 bandit==1.7.5
     # via prospector
+binaryornot==0.4.4
+    # via reuse
 black==23.3.0
     # via feed-archiver (pyproject.toml)
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==0.10.0
     # via
     #   feed-archiver (pyproject.toml)
-    #   pip-tools
     #   pyroma
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
-cfgv==3.3.1
-    # via pre-commit
+chardet==5.1.0
+    # via
+    #   binaryornot
+    #   python-debian
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
     #   click-default-group
-    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.4
+coverage==7.2.5
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
-distlib==0.3.6
-    # via virtualenv
 docutils==0.19
     # via
     #   pyroma
     #   rstcheck-core
 dodgy==0.2.1
     # via prospector
-exceptiongroup==1.1.1
-    # via pytest
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
-filelock==3.12.0
-    # via virtualenv
 flake8==2.3.0
     # via
     #   flake8-polyfill
     #   prospector
 flake8-polyfill==1.0.2
     # via pep8-naming
 future==0.18.3
@@ -88,34 +86,34 @@
     #   bandit
     #   prospector
 h11==0.14.0
     # via httpcore
 httpcore==0.17.0
     # via httpx
 httpx==0.24.0
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   respx
-identify==2.5.23
-    # via pre-commit
+    # via feed-archiver (pyproject.toml)
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
+importlib-metadata==6.6.0 ; python_version < "3.10"
+    # via feed-archiver (pyproject.toml)
 incremental==22.10.0
     # via towncrier
-iniconfig==2.0.0
-    # via pytest
 isort==5.12.0
     # via pylint
 jinja2==3.1.2
-    # via towncrier
+    # via
+    #   reuse
+    #   towncrier
 lazy-object-proxy==1.9.0
     # via astroid
+license-expression==30.1.0
+    # via reuse
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
 lxml-stubs==0.4.0
     # via feed-archiver (pyproject.toml)
 mando==0.6.4
     # via radon
 markupsafe==2.1.2
@@ -127,43 +125,33 @@
     #   pylint
 mypy==1.2.0
     # via prospector
 mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-nodeenv==1.7.0
-    # via pre-commit
 packaging==23.1
     # via
     #   black
     #   build
     #   prospector
     #   pyroma
-    #   pytest
     #   requirements-detector
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
-pip-tools==6.13.0
-    # via feed-archiver (pyproject.toml)
 platformdirs==3.5.0
     # via
     #   black
     #   pylint
-    #   virtualenv
-pluggy==1.0.0
-    # via pytest
-pre-commit==3.2.2
-    # via feed-archiver (pyproject.toml)
 prospector[with_everything]==1.9.0
     # via feed-archiver (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
     #   prospector
 pydantic==1.10.7
@@ -175,15 +163,15 @@
     #   autoflake
     #   flake8
     #   prospector
 pygments==2.15.1
     # via
     #   pyroma
     #   rich
-pylint==2.17.3
+pylint==2.17.4
     # via
     #   prospector
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
     #   pylint-plugin-utils
 pylint-celery==0.3
@@ -198,40 +186,33 @@
     #   pylint-celery
     #   pylint-django
     #   pylint-flask
 pyproject-hooks==1.0.0
     # via build
 pyroma==4.2
     # via prospector
-pytest==7.3.1
-    # via
-    #   feed-archiver (pyproject.toml)
-    #   pytest-subtests
-pytest-subtests==0.10.0
-    # via feed-archiver (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyyaml==6.0
     # via
     #   bandit
     #   feed-archiver (pyproject.toml)
-    #   pre-commit
     #   prospector
     #   xenon
 radon==5.1.0
     # via xenon
-requests==2.29.0
+requests==2.30.0
     # via
     #   arrapi
     #   pyroma
-    #   requests-mock
+    #   reuse
     #   xenon
-requests-mock==1.10.0
-    # via feed-archiver (pyproject.toml)
 requirements-detector==1.2.1
     # via prospector
-respx==0.20.1
+reuse==1.0.0
     # via feed-archiver (pyproject.toml)
 rich==12.6.0
     # via
     #   bandit
     #   typer
 rstcheck==6.1.2
     # via feed-archiver (pyproject.toml)
@@ -244,15 +225,14 @@
 sgmllib3k==1.0.0
     # via feedparser
 shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   mando
-    #   requests-mock
     #   user-agent
 smmap==5.0.0
     # via gitdb
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
@@ -273,50 +253,46 @@
     #   autoflake
     #   autopep8
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
-    #   pytest
     #   towncrier
 tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.29
+trove-classifiers==2023.5.2
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.8
+types-docutils==0.19.1.9
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.29.0.0
+types-requests==2.30.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.11
+types-urllib3==1.26.25.12
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.23.0
-    # via pre-commit
 vulture==2.7
     # via prospector
-wheel==0.40.0
-    # via pip-tools
 wrapt==1.15.0
     # via astroid
 xenon==0.9.0
     # via feed-archiver (pyproject.toml)
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `feed-archiver-2.0.4/requirements/py39/user.txt` & `feed-archiver-2.0.6b1/requirements/py311/test.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,93 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/py39/user.txt --resolver=backtracking pyproject.toml
+#    pip-compile --extra=test --output-file=requirements/py311/test.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
 argcomplete==3.0.8
     # via feed-archiver (pyproject.toml)
 arrapi==1.4.2
     # via feed-archiver (pyproject.toml)
-certifi==2022.12.7
+attrs==23.1.0
+    # via pytest-subtests
+build==0.10.0
+    # via pip-tools
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
     #   requests
 charset-normalizer==3.1.0
     # via requests
+click==8.1.3
+    # via pip-tools
 feedparser==6.0.10
     # via feed-archiver (pyproject.toml)
 h11==0.14.0
     # via httpcore
 httpcore==0.17.0
     # via httpx
 httpx==0.24.0
-    # via feed-archiver (pyproject.toml)
+    # via
+    #   feed-archiver (pyproject.toml)
+    #   respx
 idna==3.4
     # via
     #   anyio
     #   httpx
     #   requests
+iniconfig==2.0.0
+    # via pytest
 lxml==4.9.2
     # via feed-archiver (pyproject.toml)
+packaging==23.1
+    # via
+    #   build
+    #   pytest
+pip-tools==6.13.0
+    # via feed-archiver (pyproject.toml)
+pluggy==1.0.0
+    # via pytest
+pyproject-hooks==1.0.0
+    # via build
+pytest==7.3.1
+    # via
+    #   feed-archiver (pyproject.toml)
+    #   pytest-subtests
+pytest-subtests==0.10.0
+    # via feed-archiver (pyproject.toml)
 pyyaml==6.0
     # via feed-archiver (pyproject.toml)
-requests==2.29.0
-    # via arrapi
+requests==2.30.0
+    # via
+    #   arrapi
+    #   requests-mock
+requests-mock==1.10.0
+    # via feed-archiver (pyproject.toml)
+respx==0.20.1
+    # via feed-archiver (pyproject.toml)
 sgmllib3k==1.0.0
     # via feedparser
 six==1.16.0
-    # via user-agent
+    # via
+    #   requests-mock
+    #   user-agent
 sniffio==1.3.0
     # via
     #   anyio
     #   httpcore
     #   httpx
 tenacity==8.2.2
     # via feed-archiver (pyproject.toml)
-urllib3==1.26.15
+urllib3==2.0.2
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
+wheel==0.40.0
+    # via pip-tools
+
+# The following packages are considered to be unsafe in a requirements file:
+# pip
+# setuptools
```

### Comparing `feed-archiver-2.0.4/server/docker-compose.yml` & `feed-archiver-2.0.6b1/server/docker-compose.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # Example `$ docker compose ...` configuration to demonstrate the requirements for
 # serving a feeds archive via a static site server.
 version: "3.8"
 
 services:
 
   # Container-native, outward-facing proxy to stitch together service in this stack,
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-# Example `$ docker compose ...` configuration to demonstrate the requirements
-for # serving a feeds archive via a static site server. version: "3.8"
-services: # Container-native, outward-facing proxy to stitch together service
-in this stack, # manage TLS/SSL certs, require HTTP `Basic` authentication,
-etc.. traefik: # I prefer to use the latest and have things break so I keep up
-to date. Override # to pin a version if you prefer otherwise. image: "traefik"
-container_name: "traefik" restart: "unless-stopped" command: # https://
-doc.traefik.io/traefik/user-guides/docker-compose/acme-tls/#setup - "--
-log.level=INFO" # - "--log.level=DEBUG" # https://doc.traefik.io/traefik/
-observability/access-logs/#configuration - "--accesslog=true" # Enables the web
-UI and tells Traefik to listen to docker # https://doc.traefik.io/traefik/
-getting-started/quick-start/#launch-traefik-with-the-docker-provider - "--
-api.insecure=true" - "--providers.docker=true" # Be defensive, don't
-accidentally expose internal services - "--
-providers.docker.exposedbydefault=false" # Serve HTTPS - "--
+# SPDX-FileCopyrightText: 2023 Ross Patterson
+rpatterson.net> # # SPDX-License-Identifier: MIT # Example `$ docker compose
+...` configuration to demonstrate the requirements for # serving a feeds
+archive via a static site server. version: "3.8" services: # Container-native,
+outward-facing proxy to stitch together service in this stack, # manage TLS/SSL
+certs, require HTTP `Basic` authentication, etc.. traefik: # I prefer to use
+the latest and have things break so I keep up to date. Override # to pin a
+version if you prefer otherwise. image: "traefik" container_name: "traefik"
+restart: "unless-stopped" command: # https://doc.traefik.io/traefik/user-
+guides/docker-compose/acme-tls/#setup - "--log.level=INFO" # - "--
+log.level=DEBUG" # https://doc.traefik.io/traefik/observability/access-logs/
+#configuration - "--accesslog=true" # Enables the web UI and tells Traefik to
+listen to docker # https://doc.traefik.io/traefik/getting-started/quick-start/
+#launch-traefik-with-the-docker-provider - "--api.insecure=true" - "--
+providers.docker=true" # Be defensive, don't accidentally expose internal
+services - "--providers.docker.exposedbydefault=false" # Serve HTTPS - "--
 entrypoints.websecure.address=:443" - "--
 certificatesresolvers.letsencrypt.acme.tlschallenge=true" #- "--
 certificatesresolvers.letsencrypt.acme.caserver=https://acme-staging-
 v02.api.letsencrypt.org/directory" - "--
 certificatesresolvers.letsencrypt.acme.email=me@rpatterson.net" - "--
 certificatesresolvers.letsencrypt.acme.storage=/letsencrypt/acme.json" # https:
 //doc.traefik.io/traefik/v2.2/routing/entrypoints/#redirection - "--
```

### Comparing `feed-archiver-2.0.4/setup.cfg` & `feed-archiver-2.0.6b1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -14,30 +14,30 @@
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.7
 	Topic :: Utilities
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	argcomplete
 	backports.cached-property; python_version < "3.8"
-	importlib_metadata; python_version < "3.8"
+	importlib_metadata; python_version < "3.10"
 	pyyaml
 	lxml
 	feedparser
 	httpx
 	user-agent
 	arrapi
 	tenacity
@@ -50,28 +50,29 @@
 	feed-archiver = feedarchiver:main
 feedarchiver.enclosures = 
 	default = feedarchiver.enclosures.template:TemplateEnclosurePlugin
 	template = feedarchiver.enclosures.template:TemplateEnclosurePlugin
 	sonarr = feedarchiver.enclosures.servarr:SonarrEnclosurePlugin
 
 [options.extras_require]
-devel = 
+test = 
 	respx
 	requests-mock
 	pytest
 	pytest-subtests
-	pre-commit
+	pip-tools
+devel = 
 	coverage
 	prospector[with_everything]
 	xenon
 	rstcheck
+	reuse<1.1.0
 	black
 	autoflake
 	autopep8
-	pip-tools
 	towncrier
 	build
 	lxml-stubs
 	types-requests
 	types-PyYAML
 
 [tool:pytest]
```

### Comparing `feed-archiver-2.0.4/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-2.0.6b1/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.4
+Version: 2.0.6b1
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: devel
-License-File: LICENSE
+
+.. SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+..
+.. SPDX-License-Identifier: MIT
 
 ########################################################################################
 Feed Archiver
 ########################################################################################
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/feed-archiver.svg?logo=pypi&label=PyPI&logoColor=gold
-	  :alt: PyPI latest release version
-	  :target: https://pypi.org/project/feed-archiver/
-       .. figure:: https://img.shields.io/pypi/dm/feed-archiver.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold
-	  :alt: PyPI downloads per month
-	  :target: https://pypi.org/project/feed-archiver/
+          :alt: PyPI latest release version
+          :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/pypi/pyversions/feed-archiver.svg?logo=python&label=Python&logoColor=gold
-	  :alt: PyPI Python versions
-	  :target: https://pypi.org/project/feed-archiver/
+          :alt: PyPI Python versions
+          :target: https://pypi.org/project/feed-archiver/
        .. figure:: https://img.shields.io/badge/code%20style-black-000000.svg
-	  :alt: Python code style
-	  :target: https://github.com/psf/black
+          :alt: Python code style
+          :target: https://github.com/psf/black
+       .. figure:: https://api.reuse.software/badge/gitlab.com/rpatterson/feed-archiver
+          :alt: REUSE license status
+          :target: https://api.reuse.software/info/gitlab.com/rpatterson/feed-archiver
 
      - .. figure:: https://gitlab.com/rpatterson/feed-archiver/-/badges/release.svg
 	  :alt: GitLab latest release
 	  :target: https://gitlab.com/rpatterson/feed-archiver/-/releases
        .. figure:: https://gitlab.com/rpatterson/feed-archiver/badges/main/pipeline.svg
           :alt: GitLab CI/CD pipeline status
           :target: https://gitlab.com/rpatterson/feed-archiver/-/commits/main
@@ -78,18 +82,18 @@
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/feed-archiver?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/stars/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub stars
-	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
+          :target: https://hub.docker.com/r/merpatterson/feed-archiver
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/feed-archiver?logo=docker
 	  :alt: Docker Hub image size (latest semver)
-	  :target: https://hub.docker.com/r/merpatterson/feed-archiver
+          :target: https://hub.docker.com/r/merpatterson/feed-archiver
 
      - .. figure:: https://img.shields.io/keybase/pgp/rpatterson?logo=keybase
           :alt: KeyBase PGP key ID
           :target: https://keybase.io/rpatterson
        .. figure:: https://img.shields.io/github/followers/rpatterson?style=social
           :alt: GitHub followers count
           :target: https://github.com/rpatterson
@@ -186,16 +190,14 @@
 re-using example configurations known to work by others.
 
 
 ****************************************************************************************
 Installation
 ****************************************************************************************
 
-Install and use either via a local, native installation or a Docker container image:
-
 Local/Native Installation
 ========================================================================================
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ pip3 install --user feed-archiver
 
@@ -208,30 +210,30 @@
 `the example ./docker-compose.yml file`_ for an example configuration.  Once you have
 your configuration, you can create and run the container::
 
   $ docker compose up
 
 Alternatively, you make use the image directly.  Pull `the Docker image`_::
 
-  $ docker pull "registry.gitlab.org/rpatterson/feed-archiver"
+  $ docker pull "registry.gitlab.com/rpatterson/feed-archiver"
 
 And then use the image to create and run a container::
 
-  $ docker run --rm -it "registry.gitlab.org/rpatterson/feed-archiver" ...
+  $ docker run --rm -it "registry.gitlab.com/rpatterson/feed-archiver" ...
 
 Images variant tags are published for the Python version, branch, and major/minor
 versions so that users can control when they get new images over time,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-main``.  The canonical
-Python version is 3.10 which is the version used in tags without ``py###``,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:main``.  Pre-releases are from
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310-main``.  The canonical Python
+version is 3.10 which is the version used in tags without ``py###``,
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:main``.  Pre-releases are from
 ``develop`` and final releases are from ``main`` which is also the default for tags
-without a branch, e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310``. The
+without a branch, e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310``. The
 major/minor version tags are only applied to the final release images and without the
 corresponding ``main`` branch tag,
-e.g. ``registry.gitlab.org/merpatterson/feed-archiver:py310-v0.8``.
+e.g. ``registry.gitlab.com/rpatterson/feed-archiver:py310-v0.8``.
 
 Multi-platform Docker images are published containing images for the following
 platforms or architectures in the Python 3.10 ``py310`` variant:
 
 - ``linux/amd64``
 - ``linux/arm64``
 - ``linux/arm/v7``
```

### Comparing `feed-archiver-2.0.4/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-2.0.6b1/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+.cz.toml
 .dir-locals.el.in
 .dockerignore
 .env.in
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
 .prospector.yaml
 CONTRIBUTING.rst
 Dockerfile
-Dockerfile.devel
-LICENSE
 Makefile
 NEWS-VERSION.rst
 NEWS.rst
 README.rst
 TODO.rst
 docker-compose-servarr.yml
 docker-compose.override.yml
 docker-compose.yml
-link-fallbacks.feature.rst
 pyproject.toml
 setup.cfg
+towncrier.toml
 tox.ini
 .github/workflows/build-test.yml
+.reuse/dep5
+.tox/.gitignore
+LICENSES/MIT.txt
 bin/cz-check-bump
 bin/entrypoint
 bin/get-base-version
 bin/hadolint
+bin/host-install
 build-host/Dockerfile
 build-host/Makefile
 build-host/README.rst
 build-host/requirements-py310.txt
 build-host/requirements-py311.txt
 build-host/requirements-py37.txt
 build-host/requirements-py38.txt
@@ -37,32 +40,39 @@
 build-host/requirements.txt.in
 build-host/bin/entrypoint
 dist/.gitignore
 gitlab-runner/docker-compose.yml
 gitlab-runner/config/config.toml.in
 home/.gitignore
 home/.pypirc.in
+newsfragments/.gitignore
 nginx/templates/default.conf.template
 requirements/build.txt.in
 requirements/py310/build.txt
 requirements/py310/devel.txt
+requirements/py310/test.txt
 requirements/py310/user.txt
 requirements/py311/build.txt
 requirements/py311/devel.txt
+requirements/py311/test.txt
 requirements/py311/user.txt
 requirements/py37/build.txt
 requirements/py37/devel.txt
+requirements/py37/test.txt
 requirements/py37/user.txt
 requirements/py38/build.txt
 requirements/py38/devel.txt
+requirements/py38/test.txt
 requirements/py38/user.txt
 requirements/py39/build.txt
 requirements/py39/devel.txt
+requirements/py39/test.txt
 requirements/py39/user.txt
 server/docker-compose.yml
+src/feed_archiver.egg-info/.gitignore
 src/feed_archiver.egg-info/PKG-INFO
 src/feed_archiver.egg-info/SOURCES.txt
 src/feed_archiver.egg-info/dependency_links.txt
 src/feed_archiver.egg-info/entry_points.txt
 src/feed_archiver.egg-info/requires.txt
 src/feed_archiver.egg-info/top_level.txt
 src/feedarchiver/__init__.py
@@ -71,15 +81,14 @@
 src/feedarchiver/feed.py
 src/feedarchiver/formats.py
 src/feedarchiver/utils.py
 src/feedarchiver/version.py
 src/feedarchiver/enclosures/__init__.py
 src/feedarchiver/enclosures/servarr.py
 src/feedarchiver/enclosures/template.py
-src/feedarchiver/newsfragments/.gitignore
 src/feedarchiver/tests/__init__.py
 src/feedarchiver/tests/test_archive.py
 src/feedarchiver/tests/test_cli.py
 src/feedarchiver/tests/test_download.py
 src/feedarchiver/tests/test_feed.py
 src/feedarchiver/tests/test_linking.py
 src/feedarchiver/tests/test_urls.py
@@ -134,8 +143,25 @@
 src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
 src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
 src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
 src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
 src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
 src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
 src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+var/.gitignore
+var-docker/.gitignore
+var-docker/py310/.gitignore
+var-docker/py310/.tox/.gitignore
+var-docker/py310/feed_archiver.egg-info/.gitignore
+var-docker/py311/.gitignore
+var-docker/py311/.tox/.gitignore
+var-docker/py311/feed_archiver.egg-info/.gitignore
+var-docker/py37/.gitignore
+var-docker/py37/.tox/.gitignore
+var-docker/py37/feed_archiver.egg-info/.gitignore
+var-docker/py38/.gitignore
+var-docker/py38/.tox/.gitignore
+var-docker/py38/feed_archiver.egg-info/.gitignore
+var-docker/py39/.gitignore
+var-docker/py39/.tox/.gitignore
+var-docker/py39/feed_archiver.egg-info/.gitignore
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/__init__.py` & `feed-archiver-2.0.6b1/src/feedarchiver/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 # PYTHON_ARGCOMPLETE_OK
+
 """
 Archive RSS/Atom syndication feeds and their enclosures and assets.
 """
 
 import sys
 import pathlib
 import logging
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/archive.py` & `feed-archiver-2.0.6b1/src/feedarchiver/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 An archive of RSS/Atom syndication feeds.
 """
 
 import os
 import pathlib
 import urllib.parse
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/enclosures/__init__.py` & `feed-archiver-2.0.6b1/src/feedarchiver/enclosures/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,42 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Plugins for linking feed item enclosures into media libraries.
 """
 
 import re
 import pprint
 
 try:
-    from importlib.metadata import entry_points  # type: ignore
-except ImportError:  # pragma: no cover
     from importlib_metadata import entry_points  # type: ignore
+except ImportError:  # pragma: no cover
+    from importlib.metadata import entry_points  # type: ignore
 
 
 def load_plugins(parent, parent_config):
     """
     Pre-process and validate the enclosure plugin configurations.
     """
     archive = getattr(parent, "archive", parent)
     defaults = archive.global_config.get("plugins", {}).get("enclosures", {})
     configs = parent_config.get("enclosures", [])
     if not isinstance(configs, list):  # pragma: no cover
         raise ValueError(
             f"`enclosures` must be a list/array:\n{pprint.pformat(configs)}"
         )
-    entrypoints = {ep.name: ep for ep in entry_points()["feedarchiver.enclosures"]}
+    entrypoints = entry_points(group="feedarchiver.enclosures")
     plugins = []
     fallack_plugins = []
     for config in configs:
         # Perform any validation as early as possible
         name = config.get("plugin", "default")
-        if name not in entrypoints:  # pragma: no cover
+        if name not in entrypoints.names:  # pragma: no cover
             raise ValueError(
                 f"enclosure plugin name not registered: {name}",
             )
         if ("match-pattern" in config and "match-string" not in config) or (
             "match-string" in config and "match-pattern" not in config
         ):  # pragma: no cover
             raise ValueError(
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/enclosures/servarr.py` & `feed-archiver-2.0.6b1/src/feedarchiver/enclosures/servarr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Link enclosures about a TV series episode next to the video file as external audio.
 """
 
 import functools
 import pathlib
 import re
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/enclosures/template.py` & `feed-archiver-2.0.6b1/src/feedarchiver/enclosures/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 The default enclosure plugin, expands a template into the target path.
 """
 
 import pathlib
 
 from .. import utils  # noqa, pylint: disable=unused-import
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/feed.py` & `feed-archiver-2.0.6b1/src/feedarchiver/feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 An RSS/Atom syndication feed in an archive.
 """
 
 import os
 import copy
 import re
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/formats.py` & `feed-archiver-2.0.6b1/src/feedarchiver/formats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Handle different feed XML formats.
 """
 
 import typing
 import logging
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/__init__.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
-Tests for this feed archiver foundation or template.
+Tests for Feed Archiver.
 """
 
 import os
 import datetime
 import pathlib
 import tempfile
 import shutil
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink/.feed-archiver.yml` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/relink/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/test_archive.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_archive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test the feed-archiver representation of an archive of syndication feeeds.
 """
 
 import typing
 import unittest
 from unittest import mock
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/test_cli.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test the feed-archiver Command-Line Interface.
 """
 
 import sys
 import os
 import io
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/test_download.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_download.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test the feed-archiver downloading of enclosures, assets, etc..
 """
 
 import os
 import datetime
 import pathlib
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/test_feed.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test updating the archive from the feed URLs.
 """
 
 import os
 import datetime
 import logging
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/test_linking.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_linking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test the feed-archiver linking of enclosures into media libraries.
 """
 
 import os
 import pathlib
 import logging
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/tests/test_urls.py` & `feed-archiver-2.0.6b1/src/feedarchiver/tests/test_urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Test the feed-archiver URL escaping for file-system paths.
 """
 
 from .. import tests
```

### Comparing `feed-archiver-2.0.4/src/feedarchiver/utils.py` & `feed-archiver-2.0.6b1/src/feedarchiver/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Utility functions or other shared constants and values.
 
 Particularly useful to avoid circular imports.
 """
 
 import os
```

### Comparing `feed-archiver-2.0.4/tox.ini` & `feed-archiver-2.0.6b1/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,42 @@
+; SPDX-FileCopyrightText: 2023 Ross Patterson <me@rpatterson.net>
+;
+; SPDX-License-Identifier: MIT
+
 [tox]
 # https://devguide.python.org/versions/#supported-versions
-envlist = py{37,38,39,310,311}
+envlist = py{310,311,39,38,37}
 # https://tox.wiki/en/latest/example/package.html#setuptools
 isolated_build = True
 
+[project]
+name = feed-archiver
+package = feedarchiver
+
 [testenv]
-description = Run tests and checks for code and content
+description = Run the project test suite
 package = wheel
 wheel_build_env = .pkg
 passenv =
     HOME
     PYTHON_HOST_ENV
     DEBUG
-extras = devel
-deps = -rrequirements/{envname}/devel.txt
+extras = test
+deps = -rrequirements/{envname}/test.txt
+commands =
+    pytest --junit-xml="./build/{envname}/pytest-junit.xml" -s
+
+[testenv:py310]
+description = Run the project test suite with coverage and checks for code and content
+extras =
+    test
+    devel
+deps =
+    -rrequirements/{envname}/test.txt
+    -rrequirements/{envname}/devel.txt
 commands =
 # Create a directory for artifacts not managed by `$ tox`:
     python -c 'import pathlib; \
         pathlib.Path("./build/{envname}").mkdir(parents=True, exist_ok=True)'
 # Fail fast.  Run quick tests and checks first to save time in the inner loop of
 # development iteration.
     pyroma --min="10" "./"
@@ -33,43 +52,41 @@
         --output-format "json:./build/{envname}/prospector.json" \
         --output-format "pylint:./build/{envname}/prospector.pylint" \
         --output-format "text:./build/{envname}/prospector.txt" \
         --output-format "vscode:./build/{envname}/prospector-vscode.txt" \
         --output-format "xunit:./build/{envname}/prospector-xunit.xml" \
         --output-format "yaml:./build/{envname}/prospector.yaml" \
         --output-format "grouped" \
-        "./src/feedarchiver/"
+        "./src/{[project]package}/"
 # https://github.com/PyCQA/prospector/issues/599#issue-1600120419
-    vulture "./src/feedarchiver/"
+    vulture "./src/{[project]package}/"
 # https://xenon.readthedocs.io/en/latest/#an-actual-example
     xenon --max-absolute "C" --max-modules "B" --max-average "A" \
-        "./src/feedarchiver/"
+        "./src/{[project]package}/"
 # Check documentation as much a possible:
     rstcheck -r "./README.rst" "./CONTRIBUTING.rst" "./TODO.rst" \
-        "./src/feedarchiver/" "./build-host/"
+        "./newsfragments/"
+# Check copyright and licensing:
+    reuse lint
 # Ensure this package is correctly installed into this environment.
-    python -m "feedarchiver" --help
-    feed-archiver --help
+    python -m "{[project]package}" --help
+    {[project]name} --help
 # Run more time consuming tests and checks last.
-    coverage run --data-file="./build/{envname}/.coverage" -m pytest \
-        --junit-xml="./build/{envname}/pytest-junit.xml" -s
+    coverage run --data-file="./build/{envname}/.coverage" -m {[testenv]commands}
     coverage json --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -o "./build/{envname}/coverage.json"
     coverage lcov --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -o "./build/{envname}/coverage-lcov.info"
     coverage xml --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -o "./build/{envname}/coverage.xml"
     coverage html --fail-under=0 --data-file="./build/{envname}/.coverage" \
         -d "./build/{envname}/htmlcov"
     coverage report --data-file="./build/{envname}/.coverage"
 
 [testenv:build]
 description = Independent build, release, devel tools (requires PYTHON_HOST_ENV)
 skip_install = true
-# Workaround an issue with `skip_install` and passing in the `--installpkg` CLI option:
-# https://github.com/tox-dev/tox/issues/2442#issuecomment-1347549575
-package_env =
 deps = -rrequirements/{env:PYTHON_HOST_ENV:py310}/build.txt
 commands =
 
 [testenv:.pkg]
-deps = build
+deps = build
```

