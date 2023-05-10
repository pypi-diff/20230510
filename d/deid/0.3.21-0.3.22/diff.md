# Comparing `tmp/deid-0.3.21.tar.gz` & `tmp/deid-0.3.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deid-0.3.21.tar", last modified: Wed Dec  7 19:48:09 2022, max compression
+gzip compressed data, was "deid-0.3.22.tar", last modified: Wed May 10 16:45:21 2023, max compression
```

## Comparing `deid-0.3.21.tar` & `deid-0.3.22.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.194917 deid-0.3.21/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       21 2021-06-30 01:32:24.000000 deid-0.3.21/.dockerignore
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.178916 deid-0.3.21/.github/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       14 2021-06-30 01:32:24.000000 deid-0.3.21/.github/FUNDING.yml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      416 2021-06-30 01:32:24.000000 deid-0.3.21/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       19 2021-09-21 18:35:38.000000 deid-0.3.21/.github/codespell_ignore_words.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       30 2022-11-30 03:11:49.000000 deid-0.3.21/.github/dev-requirements.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.178916 deid-0.3.21/.github/workflows/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      404 2022-11-30 03:11:49.000000 deid-0.3.21/.github/workflows/codespell.yaml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1350 2022-11-30 03:11:49.000000 deid-0.3.21/.github/workflows/docs.yaml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1074 2022-12-07 19:27:51.000000 deid-0.3.21/.github/workflows/main.yaml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      523 2022-11-30 03:11:49.000000 deid-0.3.21/.gitignore
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      673 2022-11-30 03:11:49.000000 deid-0.3.21/.pre-commit-config.yaml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15813 2021-06-30 01:32:24.000000 deid-0.3.21/.pylintrc
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      387 2022-09-28 20:27:41.000000 deid-0.3.21/.travis.yml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      190 2021-06-30 01:32:24.000000 deid-0.3.21/AUTHORS.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7679 2022-12-07 19:48:06.000000 deid-0.3.21/CHANGELOG.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4851 2022-11-30 03:11:49.000000 deid-0.3.21/CONTRIBUTING.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      271 2021-06-30 01:32:24.000000 deid-0.3.21/Dockerfile
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1063 2022-09-10 22:19:04.000000 deid-0.3.21/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      128 2021-06-30 01:32:24.000000 deid-0.3.21/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2237 2022-12-07 19:48:09.194917 deid-0.3.21/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1147 2021-09-21 18:35:38.000000 deid-0.3.21/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.178916 deid-0.3.21/deid/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2021-06-30 01:32:24.000000 deid-0.3.21/deid/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.178916 deid-0.3.21/deid/config/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5894 2022-09-10 22:19:04.000000 deid-0.3.21/deid/config/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2022-09-10 22:19:04.000000 deid-0.3.21/deid/config/standards.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    20685 2022-11-30 03:11:49.000000 deid-0.3.21/deid/config/utils.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.178916 deid-0.3.21/deid/data/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      607 2022-11-30 03:11:49.000000 deid-0.3.21/deid/data/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23819 2022-11-30 03:11:49.000000 deid-0.3.21/deid/data/deid.dicom
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2561 2022-09-28 15:46:53.000000 deid-0.3.21/deid/data/deid.dicom.ultrasound
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      802 2022-11-30 03:11:49.000000 deid-0.3.21/deid/data/deid.dicom.xray.chest
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/deid/dicom/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      221 2022-11-30 03:11:49.000000 deid-0.3.21/deid/dicom/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/deid/dicom/actions/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      381 2022-09-10 22:19:04.000000 deid-0.3.21/deid/dicom/actions/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2738 2022-12-07 19:22:10.000000 deid-0.3.21/deid/dicom/actions/jitter.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2331 2022-12-07 19:22:10.000000 deid-0.3.21/deid/dicom/actions/uids.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      634 2022-11-30 03:11:49.000000 deid-0.3.21/deid/dicom/config.json
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10375 2022-09-26 00:46:56.000000 deid-0.3.21/deid/dicom/fields.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7648 2022-09-10 22:19:04.000000 deid-0.3.21/deid/dicom/filter.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3497 2022-11-30 03:11:49.000000 deid-0.3.21/deid/dicom/groups.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4208 2022-11-30 03:11:49.000000 deid-0.3.21/deid/dicom/header.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    20403 2022-12-07 19:22:10.000000 deid-0.3.21/deid/dicom/parser.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/deid/dicom/pixels/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       88 2022-09-27 22:25:24.000000 deid-0.3.21/deid/dicom/pixels/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15402 2022-12-07 19:22:10.000000 deid-0.3.21/deid/dicom/pixels/clean.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10014 2022-12-07 19:22:10.000000 deid-0.3.21/deid/dicom/pixels/detect.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5968 2022-11-30 03:11:49.000000 deid-0.3.21/deid/dicom/tags.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3739 2022-12-07 19:22:10.000000 deid-0.3.21/deid/dicom/utils.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      999 2022-09-10 22:19:04.000000 deid-0.3.21/deid/dicom/validate.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/deid/logger/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       59 2021-06-30 01:32:24.000000 deid-0.3.21/deid/logger/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9530 2022-11-30 03:11:49.000000 deid-0.3.21/deid/logger/message.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4462 2022-09-10 22:19:04.000000 deid-0.3.21/deid/logger/progress.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/deid/main/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4655 2022-11-30 03:11:49.000000 deid-0.3.21/deid/main/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2141 2022-09-10 22:19:04.000000 deid-0.3.21/deid/main/identifiers.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2540 2022-09-10 22:19:04.000000 deid-0.3.21/deid/main/inspect.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/deid/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      242 2022-09-10 22:19:04.000000 deid-0.3.21/deid/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6162 2022-12-07 19:48:06.000000 deid-0.3.21/deid/utils/actions.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4535 2022-09-10 22:19:04.000000 deid-0.3.21/deid/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      602 2022-12-07 19:48:06.000000 deid-0.3.21/deid/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.178916 deid-0.3.21/deid.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2237 2022-12-07 19:48:09.000000 deid-0.3.21/deid.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4933 2022-12-07 19:48:09.000000 deid-0.3.21/deid.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2022-12-07 19:48:09.000000 deid-0.3.21/deid.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       40 2022-12-07 19:48:09.000000 deid-0.3.21/deid.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       54 2022-12-07 19:48:09.000000 deid-0.3.21/deid.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        5 2022-12-07 19:48:09.000000 deid-0.3.21/deid.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        7 2021-06-30 01:32:24.000000 deid-0.3.21/docs/.gitignore
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2021-06-30 01:32:24.000000 deid-0.3.21/docs/Gemfile
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1215 2022-11-30 03:11:49.000000 deid-0.3.21/docs/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1391 2022-09-10 22:19:04.000000 deid-0.3.21/docs/_config.yml
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_data/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      395 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_data/links.yml
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_docs/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       34 2021-06-30 01:32:24.000000 deid-0.3.21/docs/_docs/_defaults.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_docs/contributing/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2416 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/contributing/code.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2042 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/contributing/docs.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_docs/development/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3784 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/development/image-format.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      589 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/development/index.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      497 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/development/linting-format.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_docs/examples/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9012 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/examples/client.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8794 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/examples/deid-dataset.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9811 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/examples/func-replace.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7577 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/examples/func-sequence-replace.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11886 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/examples/header-expanders.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2064 2021-06-30 01:32:24.000000 deid-0.3.21/docs/_docs/examples/index.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14974 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/examples/recipe.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_docs/getting-started/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3118 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/getting-started/dicom-config.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7162 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/getting-started/dicom-get.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3838 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/getting-started/dicom-loading.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14944 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/getting-started/dicom-pixels.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    19625 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/getting-started/dicom-put.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1565 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/getting-started/index.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_docs/install/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      989 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/install/docker.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      537 2021-06-30 01:32:24.000000 deid-0.3.21/docs/_docs/install/index.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      874 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/install/local.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_docs/user-docs/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    21290 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/user-docs/client.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      921 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/user-docs/index.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7540 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/user-docs/recipe-filters.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4191 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/user-docs/recipe-funcs.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5339 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/user-docs/recipe-groups.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    19875 2022-12-07 19:48:06.000000 deid-0.3.21/docs/_docs/user-docs/recipe-headers.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1389 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/user-docs/recipe-labels.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1485 2022-11-30 03:11:49.000000 deid-0.3.21/docs/_docs/user-docs/tags.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_includes/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1072 2021-06-30 01:32:24.000000 deid-0.3.21/docs/_includes/head.html
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1569 2022-09-10 22:19:04.000000 deid-0.3.21/docs/_includes/navigation.html
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_layouts/
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)     1053 2021-06-30 01:32:24.000000 deid-0.3.21/docs/_layouts/default.html
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/_posts/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1690 2021-06-30 01:32:24.000000 deid-0.3.21/docs/_posts/2018-12-09-docs.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       85 2021-06-30 01:32:24.000000 deid-0.3.21/docs/_posts/_defaults.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/api_docs/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/.nojekyll
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6805 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/Makefile
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.182916 deid-0.3.21/docs/api_docs/_static/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1751 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/_static/theme.css
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.186917 deid-0.3.21/docs/api_docs/_templates/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      290 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/_templates/class.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      229 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/_templates/function.rst
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.186917 deid-0.3.21/docs/api_docs/assets/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1150 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/assets/favicon.ico
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4142 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/assets/logo.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9213 2022-11-30 03:11:49.000000 deid-0.3.21/docs/api_docs/conf.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      125 2022-09-11 02:56:17.000000 deid-0.3.21/docs/api_docs/docs-requirements.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1241 2022-11-30 03:11:49.000000 deid-0.3.21/docs/api_docs/index.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/requirements.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.186917 deid-0.3.21/docs/api_docs/source/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      471 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.config.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      150 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.data.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      522 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.dicom.actions.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      516 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.dicom.pixels.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1392 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.dicom.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      474 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.logger.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      465 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.main.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      423 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3088 2022-09-28 20:27:41.000000 deid-0.3.21/docs/api_docs/source/deid.tests.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      459 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/deid.utils.rst
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       49 2022-09-10 22:19:04.000000 deid-0.3.21/docs/api_docs/source/modules.rst
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      202 2022-09-28 20:27:41.000000 deid-0.3.21/docs/apidoc.sh
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.178916 deid-0.3.21/docs/assets/
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.186917 deid-0.3.21/docs/assets/css/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    26599 2022-11-30 03:11:49.000000 deid-0.3.21/docs/assets/css/deid.css
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.186917 deid-0.3.21/docs/assets/fonts/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    25024 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/fonts/helveticaneueout-webfont.woff
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    20244 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/fonts/helveticaneueout-webfont.woff2
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.186917 deid-0.3.21/docs/assets/img/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      837 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/img/apple-touch-icon.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      224 2022-11-30 03:11:49.000000 deid-0.3.21/docs/assets/img/emblem.svg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1150 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/img/favicon.ico
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      311 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/img/favicon.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    29361 2022-12-07 19:48:06.000000 deid-0.3.21/docs/assets/img/interaction-grid.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4142 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/img/logo.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      216 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/img/menu.svg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    39652 2021-10-07 22:49:57.000000 deid-0.3.21/docs/assets/img/open-source-halloween-2021.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)   104993 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/img/siteicon.png
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      859 2021-06-30 01:32:24.000000 deid-0.3.21/docs/assets/img/touch-icon.png
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.186917 deid-0.3.21/docs/assets/js/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15439 2022-11-30 03:11:49.000000 deid-0.3.21/docs/assets/js/lunr.min.js
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3002 2022-11-30 03:11:49.000000 deid-0.3.21/docs/assets/js/search.js
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/docs/pages/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2021-06-30 01:32:24.000000 deid-0.3.21/docs/pages/404.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      890 2021-06-30 01:32:24.000000 deid-0.3.21/docs/pages/changelog.html
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1478 2022-11-30 03:11:49.000000 deid-0.3.21/docs/pages/index.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      128 2021-06-30 01:32:24.000000 deid-0.3.21/docs/pages/robots.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      991 2021-06-30 01:32:24.000000 deid-0.3.21/docs/pages/search.html
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/examples/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      374 2022-11-30 03:11:49.000000 deid-0.3.21/examples/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/examples/deid/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      277 2021-09-21 18:35:38.000000 deid-0.3.21/examples/deid/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      395 2022-09-26 00:46:56.000000 deid-0.3.21/examples/deid/deid.dicom
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      319 2022-09-26 00:46:56.000000 deid-0.3.21/examples/deid/deid.dicom-groups
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      211 2021-06-30 01:32:24.000000 deid-0.3.21/examples/deid/deid.dicom-pusheen
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/examples/dicom/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      256 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/examples/dicom/dicom-extract/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      191 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/dicom-extract/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5677 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/dicom-extract/create-dicom-csv.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/examples/dicom/header-manipulation/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7579 2021-06-30 01:32:24.000000 deid-0.3.21/examples/dicom/header-manipulation/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      152 2021-06-30 01:32:24.000000 deid-0.3.21/examples/dicom/header-manipulation/deid.dicom
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/examples/dicom/header-manipulation/file-meta/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       65 2021-09-06 23:26:28.000000 deid-0.3.21/examples/dicom/header-manipulation/file-meta/deid.dicom
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      647 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/header-manipulation/file-meta/example.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3895 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/header-manipulation/func-replacement.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/examples/dicom/header-manipulation/func-sequence-replace/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)   854078 2021-06-30 01:32:24.000000 deid-0.3.21/examples/dicom/header-manipulation/func-sequence-replace/MR.dcm
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)   845062 2021-06-30 01:32:24.000000 deid-0.3.21/examples/dicom/header-manipulation/func-sequence-replace/cleaned.dcm
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       71 2021-06-30 01:32:24.000000 deid-0.3.21/examples/dicom/header-manipulation/func-sequence-replace/deid.dicom
--rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)     1308 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/header-manipulation/func-sequence-replace/example.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.190917 deid-0.3.21/examples/dicom/pixels/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1851 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/pixels/run-cleaner-client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      877 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/pixels/run-inspect-pixels.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.194917 deid-0.3.21/examples/dicom/recipe/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8089 2022-11-30 03:11:49.000000 deid-0.3.21/examples/dicom/recipe/deid-dicom-example.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      395 2022-09-26 00:46:56.000000 deid-0.3.21/examples/dicom/recipe/deid.dicom
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2022-11-30 03:11:49.000000 deid-0.3.21/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      646 2022-12-07 19:48:09.194917 deid-0.3.21/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3562 2022-11-30 03:11:49.000000 deid-0.3.21/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2022-12-07 19:48:09.194917 deid-0.3.21/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2250 2022-11-30 03:24:04.000000 deid-0.3.21/test/test.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.867051 deid-0.3.22/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       21 2021-06-30 01:32:24.000000 deid-0.3.22/.dockerignore
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.843051 deid-0.3.22/.github/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       14 2021-06-30 01:32:24.000000 deid-0.3.22/.github/FUNDING.yml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      416 2021-06-30 01:32:24.000000 deid-0.3.22/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       19 2021-09-21 18:35:38.000000 deid-0.3.22/.github/codespell_ignore_words.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       30 2022-11-30 03:11:49.000000 deid-0.3.22/.github/dev-requirements.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.843051 deid-0.3.22/.github/workflows/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      404 2022-11-30 03:11:49.000000 deid-0.3.22/.github/workflows/codespell.yaml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1350 2022-11-30 03:11:49.000000 deid-0.3.22/.github/workflows/docs.yaml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1074 2022-12-07 19:27:51.000000 deid-0.3.22/.github/workflows/main.yaml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      523 2022-11-30 03:11:49.000000 deid-0.3.22/.gitignore
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      673 2022-11-30 03:11:49.000000 deid-0.3.22/.pre-commit-config.yaml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15813 2021-06-30 01:32:24.000000 deid-0.3.22/.pylintrc
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      387 2022-09-28 20:27:41.000000 deid-0.3.22/.travis.yml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      190 2021-06-30 01:32:24.000000 deid-0.3.22/AUTHORS.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7936 2023-05-10 16:45:18.000000 deid-0.3.22/CHANGELOG.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4851 2022-11-30 03:11:49.000000 deid-0.3.22/CONTRIBUTING.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      271 2021-06-30 01:32:24.000000 deid-0.3.22/Dockerfile
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1063 2022-09-10 22:19:04.000000 deid-0.3.22/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      128 2021-06-30 01:32:24.000000 deid-0.3.22/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2257 2023-05-10 16:45:21.867051 deid-0.3.22/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1147 2021-09-21 18:35:38.000000 deid-0.3.22/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.843051 deid-0.3.22/deid/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2021-06-30 01:32:24.000000 deid-0.3.22/deid/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.843051 deid-0.3.22/deid/config/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5892 2023-05-10 16:45:18.000000 deid-0.3.22/deid/config/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-05-10 16:45:18.000000 deid-0.3.22/deid/config/standards.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    20674 2023-05-10 16:45:18.000000 deid-0.3.22/deid/config/utils.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/deid/data/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      607 2023-05-10 16:45:18.000000 deid-0.3.22/deid/data/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23816 2023-01-21 00:40:59.000000 deid-0.3.22/deid/data/deid.dicom
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2561 2022-09-28 15:46:53.000000 deid-0.3.22/deid/data/deid.dicom.ultrasound
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      802 2022-11-30 03:11:49.000000 deid-0.3.22/deid/data/deid.dicom.xray.chest
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/deid/dicom/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      221 2022-11-30 03:11:49.000000 deid-0.3.22/deid/dicom/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/deid/dicom/actions/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      381 2022-09-10 22:19:04.000000 deid-0.3.22/deid/dicom/actions/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2736 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/actions/jitter.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2331 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/actions/uids.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      634 2022-11-30 03:11:49.000000 deid-0.3.22/deid/dicom/config.json
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10370 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/fields.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7779 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/filter.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3494 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/groups.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4206 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/header.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    20398 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/parser.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/deid/dicom/pixels/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       88 2022-09-27 22:25:24.000000 deid-0.3.22/deid/dicom/pixels/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15394 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/pixels/clean.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10009 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/pixels/detect.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5967 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/tags.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3739 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/utils.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      998 2023-05-10 16:45:18.000000 deid-0.3.22/deid/dicom/validate.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/deid/logger/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       59 2021-06-30 01:32:24.000000 deid-0.3.22/deid/logger/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9529 2023-05-10 16:45:18.000000 deid-0.3.22/deid/logger/message.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4462 2022-09-10 22:19:04.000000 deid-0.3.22/deid/logger/progress.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/deid/main/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4654 2023-05-10 16:45:18.000000 deid-0.3.22/deid/main/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2140 2023-05-10 16:45:18.000000 deid-0.3.22/deid/main/identifiers.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2540 2023-05-10 16:45:18.000000 deid-0.3.22/deid/main/inspect.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/deid/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      242 2022-09-10 22:19:04.000000 deid-0.3.22/deid/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6159 2023-05-10 16:45:18.000000 deid-0.3.22/deid/utils/actions.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4535 2023-05-10 16:45:18.000000 deid-0.3.22/deid/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      602 2023-05-10 16:45:18.000000 deid-0.3.22/deid/version.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.843051 deid-0.3.22/deid.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2257 2023-05-10 16:45:21.000000 deid-0.3.22/deid.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4933 2023-05-10 16:45:21.000000 deid-0.3.22/deid.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-10 16:45:21.000000 deid-0.3.22/deid.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       40 2023-05-10 16:45:21.000000 deid-0.3.22/deid.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       54 2023-05-10 16:45:21.000000 deid-0.3.22/deid.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        5 2023-05-10 16:45:21.000000 deid-0.3.22/deid.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/docs/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        7 2021-06-30 01:32:24.000000 deid-0.3.22/docs/.gitignore
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2021-06-30 01:32:24.000000 deid-0.3.22/docs/Gemfile
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1215 2022-11-30 03:11:49.000000 deid-0.3.22/docs/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1391 2022-09-10 22:19:04.000000 deid-0.3.22/docs/_config.yml
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/docs/_data/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      395 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_data/links.yml
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/docs/_docs/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       34 2021-06-30 01:32:24.000000 deid-0.3.22/docs/_docs/_defaults.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.847051 deid-0.3.22/docs/_docs/contributing/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2416 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/contributing/code.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2042 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/contributing/docs.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.851051 deid-0.3.22/docs/_docs/development/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3784 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/development/image-format.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      589 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/development/index.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      497 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/development/linting-format.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.851051 deid-0.3.22/docs/_docs/examples/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9012 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/examples/client.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8794 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/examples/deid-dataset.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9811 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/examples/func-replace.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7577 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/examples/func-sequence-replace.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11886 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/examples/header-expanders.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2064 2021-06-30 01:32:24.000000 deid-0.3.22/docs/_docs/examples/index.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14974 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/examples/recipe.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.851051 deid-0.3.22/docs/_docs/getting-started/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3118 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/getting-started/dicom-config.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7162 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/getting-started/dicom-get.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3838 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/getting-started/dicom-loading.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14944 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/getting-started/dicom-pixels.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    19625 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/getting-started/dicom-put.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1565 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/getting-started/index.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.851051 deid-0.3.22/docs/_docs/install/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      989 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/install/docker.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      537 2021-06-30 01:32:24.000000 deid-0.3.22/docs/_docs/install/index.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      874 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/install/local.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.851051 deid-0.3.22/docs/_docs/user-docs/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    21290 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/user-docs/client.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      921 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/user-docs/index.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7778 2023-05-10 16:45:18.000000 deid-0.3.22/docs/_docs/user-docs/recipe-filters.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4191 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/user-docs/recipe-funcs.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5339 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/user-docs/recipe-groups.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    19875 2022-12-07 19:48:06.000000 deid-0.3.22/docs/_docs/user-docs/recipe-headers.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1389 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/user-docs/recipe-labels.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1485 2022-11-30 03:11:49.000000 deid-0.3.22/docs/_docs/user-docs/tags.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.855051 deid-0.3.22/docs/_includes/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1072 2021-06-30 01:32:24.000000 deid-0.3.22/docs/_includes/head.html
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1569 2022-09-10 22:19:04.000000 deid-0.3.22/docs/_includes/navigation.html
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.855051 deid-0.3.22/docs/_layouts/
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)     1053 2021-06-30 01:32:24.000000 deid-0.3.22/docs/_layouts/default.html
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.855051 deid-0.3.22/docs/_posts/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1690 2021-06-30 01:32:24.000000 deid-0.3.22/docs/_posts/2018-12-09-docs.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       85 2021-06-30 01:32:24.000000 deid-0.3.22/docs/_posts/_defaults.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.855051 deid-0.3.22/docs/api_docs/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/.nojekyll
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6805 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/Makefile
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.855051 deid-0.3.22/docs/api_docs/_static/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1751 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/_static/theme.css
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.855051 deid-0.3.22/docs/api_docs/_templates/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      290 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/_templates/class.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      229 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/_templates/function.rst
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.855051 deid-0.3.22/docs/api_docs/assets/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1150 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/assets/favicon.ico
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4142 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/assets/logo.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     9213 2022-11-30 03:11:49.000000 deid-0.3.22/docs/api_docs/conf.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      125 2022-09-11 02:56:17.000000 deid-0.3.22/docs/api_docs/docs-requirements.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1241 2022-11-30 03:11:49.000000 deid-0.3.22/docs/api_docs/index.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/requirements.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.859051 deid-0.3.22/docs/api_docs/source/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      471 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.config.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      150 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.data.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      522 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.dicom.actions.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      516 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.dicom.pixels.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1392 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.dicom.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      474 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.logger.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      465 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.main.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      423 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3088 2022-09-28 20:27:41.000000 deid-0.3.22/docs/api_docs/source/deid.tests.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      459 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/deid.utils.rst
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       49 2022-09-10 22:19:04.000000 deid-0.3.22/docs/api_docs/source/modules.rst
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      202 2022-09-28 20:27:41.000000 deid-0.3.22/docs/apidoc.sh
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.839050 deid-0.3.22/docs/assets/
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.859051 deid-0.3.22/docs/assets/css/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    26599 2022-11-30 03:11:49.000000 deid-0.3.22/docs/assets/css/deid.css
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.859051 deid-0.3.22/docs/assets/fonts/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    25024 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/fonts/helveticaneueout-webfont.woff
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    20244 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/fonts/helveticaneueout-webfont.woff2
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.859051 deid-0.3.22/docs/assets/img/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      837 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/img/apple-touch-icon.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      224 2022-11-30 03:11:49.000000 deid-0.3.22/docs/assets/img/emblem.svg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1150 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/img/favicon.ico
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      311 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/img/favicon.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    29361 2022-12-07 19:48:06.000000 deid-0.3.22/docs/assets/img/interaction-grid.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4142 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/img/logo.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      216 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/img/menu.svg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    39652 2021-10-07 22:49:57.000000 deid-0.3.22/docs/assets/img/open-source-halloween-2021.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)   104993 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/img/siteicon.png
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      859 2021-06-30 01:32:24.000000 deid-0.3.22/docs/assets/img/touch-icon.png
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.859051 deid-0.3.22/docs/assets/js/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    15439 2022-11-30 03:11:49.000000 deid-0.3.22/docs/assets/js/lunr.min.js
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3002 2022-11-30 03:11:49.000000 deid-0.3.22/docs/assets/js/search.js
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.863051 deid-0.3.22/docs/pages/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2021-06-30 01:32:24.000000 deid-0.3.22/docs/pages/404.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      890 2021-06-30 01:32:24.000000 deid-0.3.22/docs/pages/changelog.html
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1478 2022-11-30 03:11:49.000000 deid-0.3.22/docs/pages/index.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      128 2021-06-30 01:32:24.000000 deid-0.3.22/docs/pages/robots.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      991 2021-06-30 01:32:24.000000 deid-0.3.22/docs/pages/search.html
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.863051 deid-0.3.22/examples/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      374 2022-11-30 03:11:49.000000 deid-0.3.22/examples/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.863051 deid-0.3.22/examples/deid/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      277 2021-09-21 18:35:38.000000 deid-0.3.22/examples/deid/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      395 2022-09-26 00:46:56.000000 deid-0.3.22/examples/deid/deid.dicom
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      319 2022-09-26 00:46:56.000000 deid-0.3.22/examples/deid/deid.dicom-groups
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      211 2021-06-30 01:32:24.000000 deid-0.3.22/examples/deid/deid.dicom-pusheen
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.863051 deid-0.3.22/examples/dicom/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      256 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.863051 deid-0.3.22/examples/dicom/dicom-extract/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      191 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/dicom-extract/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5677 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/dicom-extract/create-dicom-csv.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.863051 deid-0.3.22/examples/dicom/header-manipulation/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7579 2021-06-30 01:32:24.000000 deid-0.3.22/examples/dicom/header-manipulation/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      152 2021-06-30 01:32:24.000000 deid-0.3.22/examples/dicom/header-manipulation/deid.dicom
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.863051 deid-0.3.22/examples/dicom/header-manipulation/file-meta/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       65 2021-09-06 23:26:28.000000 deid-0.3.22/examples/dicom/header-manipulation/file-meta/deid.dicom
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)      647 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/header-manipulation/file-meta/example.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3895 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/header-manipulation/func-replacement.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.867051 deid-0.3.22/examples/dicom/header-manipulation/func-sequence-replace/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)   854078 2021-06-30 01:32:24.000000 deid-0.3.22/examples/dicom/header-manipulation/func-sequence-replace/MR.dcm
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)   845062 2021-06-30 01:32:24.000000 deid-0.3.22/examples/dicom/header-manipulation/func-sequence-replace/cleaned.dcm
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       71 2021-06-30 01:32:24.000000 deid-0.3.22/examples/dicom/header-manipulation/func-sequence-replace/deid.dicom
+-rwxrwxr-x   0 vanessa   (1000) vanessa   (1000)     1308 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/header-manipulation/func-sequence-replace/example.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.867051 deid-0.3.22/examples/dicom/pixels/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1851 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/pixels/run-cleaner-client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      877 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/pixels/run-inspect-pixels.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.867051 deid-0.3.22/examples/dicom/recipe/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8089 2022-11-30 03:11:49.000000 deid-0.3.22/examples/dicom/recipe/deid-dicom-example.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      395 2022-09-26 00:46:56.000000 deid-0.3.22/examples/dicom/recipe/deid.dicom
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2022-11-30 03:11:49.000000 deid-0.3.22/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      646 2023-05-10 16:45:21.867051 deid-0.3.22/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3562 2022-11-30 03:11:49.000000 deid-0.3.22/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-10 16:45:21.867051 deid-0.3.22/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2250 2022-11-30 03:24:04.000000 deid-0.3.22/test/test.py
```

### Comparing `deid-0.3.21/.github/workflows/docs.yaml` & `deid-0.3.22/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/.github/workflows/main.yaml` & `deid-0.3.22/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/.gitignore` & `deid-0.3.22/.gitignore`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/.pre-commit-config.yaml` & `deid-0.3.22/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/.pylintrc` & `deid-0.3.22/.pylintrc`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/CHANGELOG.md` & `deid-0.3.22/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 - backward incompatible changes (recipe file format? image file format?)
 - migration guidance (how to convert images?)
 - changed behaviour (recipe sections work differently)
 
 Referenced versions in headers are tagged on Github, in parentheses are for pypi.
 
 ## [vxx](https://github.com/pydicom/deid/tree/master) (master)
+- Allow filter tag names to be 0x-prefix hex numbers so private tags can be referenced in recipes [#253](https://github.com/pydicom/deid/issues/253) (0.3.22)
+- Fix incorrect coordinate definition for GE CT [#249](https://github.com/pydicom/deid/issues/249)
 - Circular import error [#247](https://github.com/pydicom/deid/issues/247) (0.3.21)
 - Expand BLANK Action to additional VRs [#241](https://github.com/pydicom/deid/issues/241) (0.3.2)
   - Correct issues with REPLACE action on numeric VRs [#244](https://github.com/pydicom/deid/issues/244)
   - Correct issue with actions on fields within sequences [#243](https://github.com/pydicom/deid/issues/243)
 - pre-commit for linting and formatting (0.3.1)
 - Add `ctpcoordinates` and `ctpkeepcoordinates` to handle different formats (0.3.0)
   - Minimum Python required is 3.7, numpy 1.20
```

### Comparing `deid-0.3.21/CONTRIBUTING.md` & `deid-0.3.22/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/LICENSE` & `deid-0.3.22/LICENSE`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/PKG-INFO` & `deid-0.3.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: deid
-Version: 0.3.21
+Version: 0.3.22
 Summary: best effort deidentify dicom with python and pydicom
 Home-page: https://github.com/pydicom/deid
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 License: LICENSE
 Keywords: open source,python,anonymize,dicom
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -62,7 +63,9 @@
 ```bash
 docker build -t pydicom/deid .
 docker run pydicom/deid --help
 ```
 
 ## Issues
 If you have an issue, or want to request a feature, please do so on our [issues board](https://www.github.com/pydicom/deid/issues).
+
+
```

### Comparing `deid-0.3.21/README.md` & `deid-0.3.22/README.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/deid/config/__init__.py` & `deid-0.3.22/deid/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 from deid.config.standards import actions, formats, sections
 from deid.config.utils import get_deid, load_combined_deid, load_deid
 from deid.logger import bot
 
 
@@ -24,15 +24,14 @@
           is provided, should be done in order of preference for load
           (later in the list overrides earlier loaded).
     base: if True, load a default base (default_base) before custom
     default_base: the default base to load if "base" is True
     """
 
     def __init__(self, deid=None, base=False, default_base="dicom"):
-
         # If deid is None, use the default
         if deid is None:
             base = True
 
         self._init_deid(deid, base=base, default_base=default_base)
 
     def __str__(self):
@@ -45,15 +44,14 @@
         """
         Load a deid recipe into the object.
 
         If a deid configuration is already defined, append to that.
         """
         deid = get_deid(deid)
         if deid is not None:
-
             # Update our list of files
             self._files.append(deid)
             self.files = list(set(self.files))
 
             # Priority here goes to additional deid
             self.deid = load_combined_deid([self.deid, deid])
```

### Comparing `deid-0.3.21/deid/config/standards.py` & `deid-0.3.22/deid/config/standards.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 # Supported formats
 formats = ["dicom"]
 
 # Supported Sections
 sections = ["header", "labels", "filter", "values", "fields"]
```

### Comparing `deid-0.3.21/deid/config/utils.py` & `deid-0.3.22/deid/config/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 # pylint: skip-file
 
 import os
 import re
 import sys
@@ -33,35 +33,32 @@
     if not isinstance(deids, list):
         bot.exit("load_combined_deids expects a list.")
 
     found_format = None
     deid = None
 
     for single_deid in deids:
-
         # If not a tag or path, returns None
         next_deid = get_deid(tag=single_deid, exit_on_fail=False, quiet=True, load=True)
 
         if next_deid is not None:
-
             # Formats must match
             if found_format is None:
                 found_format = next_deid["format"]
             else:
                 if found_format != next_deid["format"]:
                     bot.exis(
                         "Mismatch in deid formats, %s and %s"
                         % (found_format, next_deid["format"])
                     )
 
             # If it's the first one, use as starter template
             if deid is None:
                 deid = next_deid
             else:
-
                 # Update filter, appending to end to give first preference
                 if "filter" in next_deid:
                     if "filter" not in deid:
                         deid["filter"] = next_deid["filter"]
                     else:
                         for name, group in next_deid["filter"].items():
                             deid["filter"][name] = (
@@ -108,29 +105,27 @@
     ]
 
     spec = [x for x in spec if x not in ["", None]]
     config = OrderedDict()
     section = None
 
     while spec:
-
         # Clean up white trailing/leading space
         line = spec.pop(0).strip()
 
         # Comment
         if line.startswith("#"):
             continue
 
         # Set format
         elif bool(re.match("^format", line, re.I)):
             config["format"] = parse_format(line)
 
         # A new section?
         elif line.startswith("%"):
-
             # Remove any comments
             line = line.split("#", 1)[0].strip()
 
             # Is there a section name?
             section_name = None
             parts = line.split(" ")
             if len(parts) > 1:
@@ -147,15 +142,14 @@
         elif line.upper().startswith(group_actions) and section in groups:
             config = parse_group_action(
                 section=section, section_name=section_name, line=line, config=config
             )
 
         # An action (ADD, BLANK, JITTER, KEEP, REPLACE, REMOVE, LABEL)
         elif line.upper().startswith(actions):
-
             # Start of a filter group
             if line.upper().startswith("LABEL") and section == "filter":
                 members = parse_filter_group(spec)
 
                 # Add the filter label to the config
                 config = parse_label(
                     config=config,
@@ -351,15 +345,14 @@
         if member.startswith("#"):
             continue
 
         # Now that operators removed, parse member
         if not member.lower().startswith(filters):
             bot.warning("%s filter is not valid, skipping." % member.lower())
         else:
-
             # Returns single member with field, values, operator,
             # Or if multiple or/and in statement, a list
             entry = parse_member(member, operator)
         if entry is not None:
             criteria["filters"].append(entry.copy())
 
     config[section][section_name].append(criteria)
@@ -376,15 +369,14 @@
     actions = []
     values = []
     fields = []
     operators = []
     members = [members]
 
     while len(members) > 0:
-
         operator = None
         value = None
         member = members.pop(0).strip()
 
         # Find the first || or +
         match_or = re.search("\|\|", member)  # noqa
         match_and = re.search("\+", member)  # noqa
@@ -395,15 +387,14 @@
             if match_or is not None:
                 if match_or.start() >= match_and.start():
                     operator = "+"
             else:
                 operator = "+"
 
         if operator is not None:
-
             member, rest = member.split(operator, 1)
 
             # The rest is only valid if contains a filter statement
             if any(word in rest for word in filters):
                 members.append(rest.strip())
 
                 # Split the statement based on found operator
@@ -466,15 +457,14 @@
     if section in ["filter", "values", "fields"] and section_name is None:
         bot.exit("You must provide a name for a filter section.")
 
     if section not in sections:
         bot.exit("%s is not a valid section." % section)
 
     if section not in config:
-
         # If a section is named, we have more one level (dict)
         if section_name is not None:
             config[section] = OrderedDict()
             config[section][section_name] = []
             bot.debug("Adding section %s %s" % (section, section_name))
         else:
             config[section] = []
@@ -527,15 +517,14 @@
 
     # Fields supports one or more fields with expanders (no third arguments)
     if section == "fields":
         config[section][section_name].append({"action": action, "field": field})
 
     # Values supports FIELD or SPLIT
     elif section == "values":
-
         # If we have a third set of arguments
         if parts:
             value = _remove_comments(parts)
             config[section][section_name].append(
                 {"action": action, "field": field, "value": value}
             )
         else:
```

### Comparing `deid-0.3.21/deid/data/__init__.py` & `deid-0.3.22/deid/data/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import os
 
 data_base = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `deid-0.3.21/deid/data/deid.dicom` & `deid-0.3.22/deid/data/deid.dicom`

 * *Files 0% similar despite different names*

```diff
@@ -1245,245 +1245,245 @@
 00004dc0: 202b 2063 6f6e 7461 696e 7320 4d61 6e75   + contains Manu
 00004dd0: 6661 6374 7572 6572 4d6f 6465 6c4e 616d  facturerModelNam
 00004de0: 6520 4745 7c53 7461 6e66 6f72 640a 2020  e GE|Stanford.  
 00004df0: 2b20 636f 6e74 6169 6e73 2053 6572 6965  + contains Serie
 00004e00: 7344 6573 6372 6970 7469 6f6e 2044 6f73  sDescription Dos
 00004e10: 6520 7c7c 2063 6f6e 7461 696e 7320 496d  e || contains Im
 00004e20: 6167 6554 7970 6520 5343 5245 454e 2053  ageType SCREEN S
-00004e30: 4156 450a 2020 6374 7063 6f6f 7264 696e  AVE.  ctpcoordin
-00004e40: 6174 6573 2030 2c30 2c35 3132 2c31 3231  ates 0,0,512,121
-00004e50: 0a0a 4c41 4245 4c20 5374 616e 666f 7264  ..LABEL Stanford
-00004e60: 204d 6564 6963 616c 2043 656e 7465 7220   Medical Center 
-00004e70: 4745 2023 2028 526f 6765 7220 476f 6c64  GE # (Roger Gold
-00004e80: 6d61 6e29 0a20 2063 6f6e 7461 696e 7320  man).  contains 
-00004e90: 4d61 6e75 6661 6374 7572 6572 2047 450a  Manufacturer GE.
-00004ea0: 2020 2b20 636f 6e74 6169 6e73 204d 616e    + contains Man
-00004eb0: 7566 6163 7475 7265 724d 6f64 656c 4e61  ufacturerModelNa
-00004ec0: 6d65 2047 457c 5374 616e 666f 7264 0a20  me GE|Stanford. 
-00004ed0: 202b 2063 6f6e 7461 696e 7320 496d 6167   + contains Imag
-00004ee0: 6554 7970 6520 4445 5249 5645 442b 5345  eType DERIVED+SE
-00004ef0: 434f 4e44 4152 592b 5343 5245 454e 2053  CONDARY+SCREEN S
-00004f00: 4156 450a 2020 636f 6f72 6469 6e61 7465  AVE.  coordinate
-00004f10: 7320 302c 302c 3531 322c 3132 310a 0a4c  s 0,0,512,121..L
-00004f20: 4142 454c 2053 7461 6e66 6f72 6420 4d65  ABEL Stanford Me
-00004f30: 6469 6369 6e65 204f 7574 7061 7469 656e  dicine Outpatien
-00004f40: 7420 6365 6e74 6572 0a20 2063 6f6e 7461  t center.  conta
-00004f50: 696e 7320 4d61 6e75 6661 6374 7572 6572  ins Manufacturer
-00004f60: 2053 6965 6d65 6e73 0a20 202b 2063 6f6e   Siemens.  + con
-00004f70: 7461 696e 7320 4d61 6e75 6661 6374 7572  tains Manufactur
-00004f80: 6572 4d6f 6465 6c4e 616d 6520 534f 4d41  erModelName SOMA
-00004f90: 544f 4d20 4465 6669 6e69 7469 6f6e 2041  TOM Definition A
-00004fa0: 532b 0a20 202b 2063 6f6e 7461 696e 7320  S+.  + contains 
-00004fb0: 496d 6167 6554 7970 6520 4445 5249 5645  ImageType DERIVE
-00004fc0: 447c 5345 434f 4e44 4152 597c 5343 5245  D|SECONDARY|SCRE
-00004fd0: 454e 2053 4156 457c 564f 4c52 454e 7c56  EN SAVE|VOLREN|V
-00004fe0: 5854 4c20 5354 4154 450a 0a25 6669 6c74  XTL STATE..%filt
-00004ff0: 6572 2062 6c61 636b 6c69 7374 0a0a 4c41  er blacklist..LA
-00005000: 4245 4c20 416e 7920 5363 616e 6e65 6420  BEL Any Scanned 
-00005010: 446f 6375 6d65 6e74 206f 7220 5365 636f  Document or Seco
-00005020: 6e64 6172 7920 5361 7665 0a20 2063 6f6e  ndary Save.  con
-00005030: 7461 696e 7320 496d 6167 6554 7970 6520  tains ImageType 
-00005040: 5365 636f 6e64 6172 790a 2020 636f 6e74  Secondary.  cont
-00005050: 6169 6e73 204d 6f64 616c 6974 7920 4f54  ains Modality OT
-00005060: 0a0a 4c41 4245 4c20 416e 7920 5245 504f  ..LABEL Any REPO
-00005070: 5254 4441 5441 0a20 2063 6f6e 7461 696e  RTDATA.  contain
-00005080: 7320 496d 6167 6554 7970 6520 5245 504f  s ImageType REPO
-00005090: 5254 4441 5441 0a0a 4c41 4245 4c20 416e  RTDATA..LABEL An
-000050a0: 7920 4445 4d4f 4752 4150 4849 4344 4154  y DEMOGRAPHICDAT
-000050b0: 412c 2049 4e56 414c 4944 2023 2028 414d  A, INVALID # (AM
-000050c0: 4229 0a20 2063 6f6e 7461 696e 7320 496d  B).  contains Im
-000050d0: 6167 6554 7970 6520 4445 4d4f 4752 4150  ageType DEMOGRAP
-000050e0: 4849 4344 4154 410a 2020 636f 6e74 6169  HICDATA.  contai
-000050f0: 6e73 2049 6d61 6765 5479 7065 2049 4e56  ns ImageType INV
-00005100: 414c 4944 0a0a 4c41 4245 4c20 5374 616e  ALID..LABEL Stan
-00005110: 666f 7264 2042 6c61 636b 6c69 7374 204d  ford Blacklist M
-00005120: 6973 7369 6e67 2049 6d61 6765 5479 7065  issing ImageType
-00005130: 2020 2320 5375 7361 6e20 5765 6265 722c    # Susan Weber,
-00005140: 2056 616e 6573 7361 2053 6f63 6861 740a   Vanessa Sochat.
-00005150: 2020 6d69 7373 696e 6720 496d 6167 6554    missing ImageT
-00005160: 7970 6520 7c7c 2065 6d70 7479 2049 6d61  ype || empty Ima
-00005170: 6765 5479 7065 0a0a 4c41 4245 4c20 5374  geType..LABEL St
-00005180: 616e 666f 7264 2042 6c61 636b 6c69 7374  anford Blacklist
-00005190: 2073 6563 6f6e 6461 7279 206f 7220 6465   secondary or de
-000051a0: 7269 7665 6420 6361 7463 6861 6c6c 2023  rived catchall #
-000051b0: 2056 616e 6573 7361 2053 6f63 6861 740a   Vanessa Sochat.
-000051c0: 2020 636f 6e74 6169 6e73 204d 6f64 616c    contains Modal
-000051d0: 6974 7920 4354 7c4d 520a 2020 2b20 636f  ity CT|MR.  + co
-000051e0: 6e74 6169 6e73 2049 6d61 6765 5479 7065  ntains ImageType
-000051f0: 2044 4552 4956 4544 7c53 4543 4f4e 4441   DERIVED|SECONDA
-00005200: 5259 7c53 4352 4545 4e7c 5341 5645 0a0a  RY|SCREEN|SAVE..
-00005210: 4c41 4245 4c20 5374 616e 666f 7264 2042  LABEL Stanford B
-00005220: 6c61 636b 6c69 7374 2044 6f73 6520 5265  lacklist Dose Re
-00005230: 706f 7274 206f 7220 4578 7465 726e 616c  port or External
-00005240: 2023 2056 616e 6573 7361 2053 6f63 6861   # Vanessa Socha
-00005250: 740a 2020 636f 6e74 6169 6e73 204d 6f64  t.  contains Mod
-00005260: 616c 6974 7920 4354 7c4d 520a 2020 2b20  ality CT|MR.  + 
-00005270: 636f 6e74 6169 6e73 2053 6572 6965 7344  contains SeriesD
-00005280: 6573 6372 6970 7469 6f6e 2050 6174 6965  escription Patie
-00005290: 6e74 2050 726f 746f 636f 6c7c 5041 4353  nt Protocol|PACS
-000052a0: 206e 6f6d 696e 6174 696f 6e20 666f 726d   nomination form
-000052b0: 7c44 6f73 6520 5265 706f 7274 7c53 7475  |Dose Report|Stu
-000052c0: 6479 2061 6371 7569 7265 6420 6f75 7473  dy acquired outs
-000052d0: 6964 6520 686f 7370 6974 616c 0a0a 4c41  ide hospital..LA
-000052e0: 4245 4c20 4275 726e 6564 2049 6e20 416e  BEL Burned In An
-000052f0: 6e6f 7461 7469 6f6e 2023 2028 4354 5029  notation # (CTP)
-00005300: 0a20 2063 6f6e 7461 696e 7320 496d 6167  .  contains Imag
-00005310: 6554 7970 6520 5341 5645 0a20 202b 2063  eType SAVE.  + c
-00005320: 6f6e 7461 696e 7320 4d6f 6461 6c69 7479  ontains Modality
-00005330: 2043 547c 4d52 0a20 207c 7c20 636f 6e74   CT|MR.  || cont
-00005340: 6169 6e73 2053 6572 6965 7344 6573 6372  ains SeriesDescr
-00005350: 6970 7469 6f6e 2053 4156 450a 2020 7c7c  iption SAVE.  ||
-00005360: 2063 6f6e 7461 696e 7320 4275 726e 6564   contains Burned
-00005370: 496e 416e 6e6f 7461 7469 6f6e 2059 4553  InAnnotation YES
-00005380: 0a20 207c 7c20 656d 7074 7920 496d 6167  .  || empty Imag
-00005390: 6554 7970 650a 2020 7c7c 2065 6d70 7479  eType.  || empty
-000053a0: 2044 6174 654f 6653 6563 6f6e 6461 7279   DateOfSecondary
-000053b0: 4361 7074 7572 650a 2020 7c7c 2065 6d70  Capture.  || emp
-000053c0: 7479 2053 6563 6f6e 6461 7279 4361 7074  ty SecondaryCapt
-000053d0: 7572 6544 6576 6963 654d 616e 7566 6163  ureDeviceManufac
-000053e0: 7475 7265 720a 2020 7c7c 2065 6d70 7479  turer.  || empty
-000053f0: 2053 6563 6f6e 6461 7279 4361 7074 7572   SecondaryCaptur
-00005400: 6544 6576 6963 654d 616e 7566 6163 7475  eDeviceManufactu
-00005410: 7265 724d 6f64 656c 4e61 6d65 0a20 207c  rerModelName.  |
-00005420: 7c20 656d 7074 7920 5365 636f 6e64 6172  | empty Secondar
-00005430: 7943 6170 7475 7265 4465 7669 6365 536f  yCaptureDeviceSo
-00005440: 6674 7761 7265 5665 7273 696f 6e73 0a0a  ftwareVersions..
-00005450: 0a25 6865 6164 6572 0a0a 5245 4d4f 5645  .%header..REMOVE
-00005460: 2065 6e64 7377 6974 683a 5469 6d65 0a52   endswith:Time.R
-00005470: 454d 4f56 4520 656e 6473 7769 7468 3a44  EMOVE endswith:D
-00005480: 6174 650a 5245 4d4f 5645 2065 6e64 7377  ate.REMOVE endsw
-00005490: 6974 683a 7469 6d65 0a52 454d 4f56 4520  ith:time.REMOVE 
-000054a0: 4164 6469 7469 6f6e 616c 5061 7469 656e  AdditionalPatien
-000054b0: 7448 6973 746f 7279 0a52 454d 4f56 4520  tHistory.REMOVE 
-000054c0: 4163 6365 7373 696f 6e4e 756d 6265 720a  AccessionNumber.
-000054d0: 5245 4d4f 5645 2050 6174 6965 6e74 4944  REMOVE PatientID
-000054e0: 0a52 454d 4f56 4520 7374 6172 7473 7769  .REMOVE startswi
-000054f0: 7468 3a49 7373 7565 4461 7465 0a52 454d  th:IssueDate.REM
-00005500: 4f56 4520 4973 7375 6572 4f66 5061 7469  OVE IssuerOfPati
-00005510: 656e 7449 440a 5245 4d4f 5645 2046 696c  entID.REMOVE Fil
-00005520: 6c65 724f 7264 6572 4e75 6d62 6572 496d  lerOrderNumberIm
-00005530: 6167 696e 6753 6572 7669 6365 5265 7175  agingServiceRequ
-00005540: 6573 740a 5245 4d4f 5645 204f 7468 6572  est.REMOVE Other
-00005550: 5061 7469 656e 7449 4473 0a52 454d 4f56  PatientIDs.REMOV
-00005560: 4520 4f74 6865 7250 6174 6965 6e74 4e61  E OtherPatientNa
-00005570: 6d65 730a 5245 4d4f 5645 204f 7468 6572  mes.REMOVE Other
-00005580: 5061 7469 656e 7449 4473 5365 7175 656e  PatientIDsSequen
-00005590: 6365 0a52 454d 4f56 4520 5061 7469 656e  ce.REMOVE Patien
-000055a0: 7441 6464 7265 7373 0a52 454d 4f56 4520  tAddress.REMOVE 
-000055b0: 5061 7469 656e 7442 6972 7468 4e61 6d65  PatientBirthName
-000055c0: 0a52 454d 4f56 4520 5061 7469 656e 744d  .REMOVE PatientM
-000055d0: 6f74 6865 7242 6972 7468 4e61 6d65 0a52  otherBirthName.R
-000055e0: 454d 4f56 4520 5061 7469 656e 744e 616d  EMOVE PatientNam
-000055f0: 650a 5245 4d4f 5645 2050 6174 6965 6e74  e.REMOVE Patient
-00005600: 734e 616d 650a 5245 4d4f 5645 2052 6561  sName.REMOVE Rea
-00005610: 736f 6e46 6f72 5374 7564 790a 5245 4d4f  sonForStudy.REMO
-00005620: 5645 2063 6f6e 7461 696e 733a 5472 6961  VE contains:Tria
-00005630: 6c0a 5245 4d4f 5645 2073 7461 7274 7377  l.REMOVE startsw
-00005640: 6974 683a 5061 7469 656e 7454 656c 6570  ith:PatientTelep
-00005650: 686f 6e65 4e75 6d62 6572 0a52 454d 4f56  honeNumber.REMOV
-00005660: 4520 656e 6473 7769 7468 3a49 440a 5245  E endswith:ID.RE
-00005670: 4d4f 5645 2065 6e64 7377 6974 683a 4944  MOVE endswith:ID
-00005680: 730a 5245 4d4f 5645 2052 6566 6572 7269  s.REMOVE Referri
-00005690: 6e67 5068 7973 6963 6961 6e4e 616d 650a  ngPhysicianName.
-000056a0: 5245 4d4f 5645 2043 6f6e 7375 6c74 696e  REMOVE Consultin
-000056b0: 6750 6879 7369 6369 616e 4e61 6d65 0a52  gPhysicianName.R
-000056c0: 454d 4f56 4520 4576 616c 7561 746f 724e  EMOVE EvaluatorN
-000056d0: 616d 650a 5245 4d4f 5645 2050 6572 666f  ame.REMOVE Perfo
-000056e0: 726d 6564 5374 6174 696f 6e4e 616d 650a  rmedStationName.
-000056f0: 5245 4d4f 5645 2053 6563 6f6e 6461 7279  REMOVE Secondary
-00005700: 5265 7669 6577 6572 4e61 6d65 0a52 454d  ReviewerName.REM
-00005710: 4f56 4520 5065 7273 6f6e 4e61 6d65 0a52  OVE PersonName.R
-00005720: 454d 4f56 4520 5065 7273 6f6e 4164 6472  EMOVE PersonAddr
-00005730: 6573 730a 5245 4d4f 5645 2052 6566 6572  ess.REMOVE Refer
-00005740: 7269 6e67 5068 7973 6963 6961 6e41 6464  ringPhysicianAdd
-00005750: 7265 7373 0a52 454d 4f56 4520 5265 6665  ress.REMOVE Refe
-00005760: 7272 696e 6750 6879 7369 6369 616e 5465  rringPhysicianTe
-00005770: 6c65 7068 6f6e 654e 756d 6265 7273 0a52  lephoneNumbers.R
-00005780: 454d 4f56 4520 5265 6665 7272 696e 6750  EMOVE ReferringP
-00005790: 6879 7369 6369 616e 4964 656e 7469 6669  hysicianIdentifi
-000057a0: 6361 7469 6f6e 5365 7175 656e 6365 0a52  cationSequence.R
-000057b0: 454d 4f56 4520 436f 6e73 756c 7469 6e67  EMOVE Consulting
-000057c0: 5068 7973 6963 6961 6e49 6465 6e74 6966  PhysicianIdentif
-000057d0: 6963 6174 696f 6e53 6571 7565 6e63 650a  icationSequence.
-000057e0: 5245 4d4f 5645 2050 6879 7369 6369 616e  REMOVE Physician
-000057f0: 4170 7072 6f76 696e 6749 6e74 6572 7072  ApprovingInterpr
-00005800: 6574 6174 696f 6e0a 5245 4d4f 5645 2050  etation.REMOVE P
-00005810: 6879 7369 6369 616e 734f 6652 6563 6f72  hysiciansOfRecor
-00005820: 640a 5245 4d4f 5645 2050 6879 7369 6369  d.REMOVE Physici
-00005830: 616e 734f 6652 6563 6f72 6449 6465 6e74  ansOfRecordIdent
-00005840: 6966 6963 6174 696f 6e53 6571 7565 6e63  ificationSequenc
-00005850: 650a 5245 4d4f 5645 2050 6572 666f 726d  e.REMOVE Perform
-00005860: 696e 6750 6879 7369 6369 616e 4e61 6d65  ingPhysicianName
-00005870: 0a52 454d 4f56 4520 5065 7266 6f72 6d69  .REMOVE Performi
-00005880: 6e67 5068 7973 6963 6961 6e49 6465 6e74  ngPhysicianIdent
-00005890: 6966 6963 6174 696f 6e53 6571 7565 6e63  ificationSequenc
-000058a0: 650a 5245 4d4f 5645 2050 6879 7369 6369  e.REMOVE Physici
-000058b0: 616e 7352 6561 6469 6e67 5374 7564 7949  ansReadingStudyI
-000058c0: 6465 6e74 6966 6963 6174 696f 6e53 6571  dentificationSeq
-000058d0: 7565 6e63 650a 5245 4d4f 5645 2052 6571  uence.REMOVE Req
-000058e0: 7565 7374 696e 6750 6879 7369 6369 616e  uestingPhysician
-000058f0: 0a52 454d 4f56 4520 5363 6865 6475 6c65  .REMOVE Schedule
-00005900: 6450 6572 666f 726d 696e 6750 6879 7369  dPerformingPhysi
-00005910: 6369 616e 4964 656e 7469 6669 6361 7469  cianIdentificati
-00005920: 6f6e 5365 7175 656e 6365 0a52 454d 4f56  onSequence.REMOV
-00005930: 4520 5265 7175 6573 7469 6e67 5068 7973  E RequestingPhys
-00005940: 6963 6961 6e49 6465 6e74 6966 6963 6174  icianIdentificat
-00005950: 696f 6e53 6571 7565 6e63 650a 5245 4d4f  ionSequence.REMO
-00005960: 5645 2048 756d 616e 5065 7266 6f72 6d65  VE HumanPerforme
-00005970: 724e 616d 650a 5245 4d4f 5645 2043 6f6e  rName.REMOVE Con
-00005980: 7461 6374 4469 7370 6c61 794e 616d 650a  tactDisplayName.
-00005990: 5245 4d4f 5645 2050 6572 666f 726d 696e  REMOVE Performin
-000059a0: 6750 6879 7369 6369 616e 4e61 6d65 0a52  gPhysicianName.R
-000059b0: 454d 4f56 4520 4e61 6d65 4f66 5068 7973  EMOVE NameOfPhys
-000059c0: 6963 6961 6e73 5265 6164 696e 6753 7475  iciansReadingStu
-000059d0: 6479 0a52 454d 4f56 4520 4f70 6572 6174  dy.REMOVE Operat
-000059e0: 6f72 734e 616d 650a 5245 4d4f 5645 2053  orsName.REMOVE S
-000059f0: 6368 6564 756c 6564 5065 7266 6f72 6d69  cheduledPerformi
-00005a00: 6e67 5068 7973 6963 6961 6e4e 616d 650a  ngPhysicianName.
-00005a10: 5245 4d4f 5645 2052 6576 6965 7765 724e  REMOVE ReviewerN
-00005a20: 616d 650a 5245 4d4f 5645 204e 616d 6573  ame.REMOVE Names
-00005a30: 4f66 496e 7465 6e64 6564 5265 6369 7069  OfIntendedRecipi
-00005a40: 656e 7473 4f66 5265 7375 6c74 730a 5245  entsOfResults.RE
-00005a50: 4d4f 5645 2053 6f75 7263 6541 7070 6c69  MOVE SourceAppli
-00005a60: 6361 746f 724e 616d 650a 5245 4d4f 5645  catorName.REMOVE
-00005a70: 2043 6c69 6e69 6361 6c54 7269 616c 5370   ClinicalTrialSp
-00005a80: 6f6e 736f 724e 616d 650a 5245 4d4f 5645  onsorName.REMOVE
-00005a90: 2043 6f6e 7465 6e74 4372 6561 746f 724e   ContentCreatorN
-00005aa0: 616d 650a 5245 4d4f 5645 2043 6c69 6e69  ame.REMOVE Clini
-00005ab0: 6361 6c54 7269 616c 5072 6f74 6f63 6f6c  calTrialProtocol
-00005ac0: 4574 6869 6373 436f 6d6d 6974 7465 654e  EthicsCommitteeN
-00005ad0: 616d 650a 5245 4d4f 5645 2063 6f6e 7461  ame.REMOVE conta
-00005ae0: 696e 733a 5549 440a 5245 4d4f 5645 2052  ins:UID.REMOVE R
-00005af0: 6567 696f 6e4f 6652 6573 6964 656e 6365  egionOfResidence
-00005b00: 0a52 454d 4f56 4520 4375 7272 656e 7450  .REMOVE CurrentP
-00005b10: 6174 6965 6e74 4c6f 6361 7469 6f6e 0a52  atientLocation.R
-00005b20: 454d 4f56 4520 5061 7469 656e 7443 6f6d  EMOVE PatientCom
-00005b30: 6d65 6e74 730a 5245 4d4f 5645 2050 6174  ments.REMOVE Pat
-00005b40: 6965 6e74 5472 616e 7370 6f72 7441 7272  ientTransportArr
-00005b50: 616e 6765 6d65 6e74 730a 5245 4d4f 5645  angements.REMOVE
-00005b60: 2050 6174 6965 6e74 4465 6174 6844 6174   PatientDeathDat
-00005b70: 6549 6e41 6c74 6572 6e61 7469 7665 4361  eInAlternativeCa
-00005b80: 6c65 6e64 6172 0a52 454d 4f56 4520 5061  lendar.REMOVE Pa
-00005b90: 7469 656e 7449 6e73 7469 7475 7469 6f6e  tientInstitution
-00005ba0: 5265 7369 6465 6e63 650a 5245 4d4f 5645  Residence.REMOVE
-00005bb0: 2050 6572 666f 726d 6564 4c6f 6361 7469   PerformedLocati
-00005bc0: 6f6e 0a52 454d 4f56 4520 5363 6865 6475  on.REMOVE Schedu
-00005bd0: 6c65 6453 7475 6479 4c6f 6361 7469 6f6e  ledStudyLocation
-00005be0: 0a52 454d 4f56 4520 5363 6865 6475 6c65  .REMOVE Schedule
-00005bf0: 6453 7475 6479 4c6f 6361 7469 6f6e 4145  dStudyLocationAE
-00005c00: 5469 746c 650a 5245 4d4f 5645 204f 7264  Title.REMOVE Ord
-00005c10: 6572 456e 7465 7265 724c 6f63 6174 696f  erEntererLocatio
-00005c20: 6e0a 5245 4d4f 5645 2041 7373 6967 6e65  n.REMOVE Assigne
-00005c30: 644c 6f63 6174 696f 6e0a 0a41 4444 2049  dLocation..ADD I
-00005c40: 7373 7565 724f 6650 6174 6965 6e74 4944  ssuerOfPatientID
-00005c50: 2053 5441 5252 0a41 4444 2050 6174 6965   STARR.ADD Patie
-00005c60: 6e74 4269 7274 6844 6174 6520 7661 723a  ntBirthDate var:
-00005c70: 656e 7469 7479 5f74 696d 6573 7461 6d70  entity_timestamp
-00005c80: 0a41 4444 2053 7475 6479 4461 7465 2076  .ADD StudyDate v
-00005c90: 6172 3a69 7465 6d5f 7469 6d65 7374 616d  ar:item_timestam
-00005ca0: 700a 4144 4420 5061 7469 656e 7449 4420  p.ADD PatientID 
-00005cb0: 7661 723a 656e 7469 7479 5f69 640a 4144  var:entity_id.AD
-00005cc0: 4420 4163 6365 7373 696f 6e4e 756d 6265  D AccessionNumbe
-00005cd0: 7220 7661 723a 6974 656d 5f69 640a 4144  r var:item_id.AD
-00005ce0: 4420 5061 7469 656e 7449 6465 6e74 6974  D PatientIdentit
-00005cf0: 7952 656d 6f76 6564 2059 4553 0a52 454d  yRemoved YES.REM
-00005d00: 4f56 4520 6a69 7474 6572 0a              OVE jitter.
+00004e30: 4156 450a 2020 636f 6f72 6469 6e61 7465  AVE.  coordinate
+00004e40: 7320 302c 302c 3531 322c 3132 310a 0a4c  s 0,0,512,121..L
+00004e50: 4142 454c 2053 7461 6e66 6f72 6420 4d65  ABEL Stanford Me
+00004e60: 6469 6361 6c20 4365 6e74 6572 2047 4520  dical Center GE 
+00004e70: 2320 2852 6f67 6572 2047 6f6c 646d 616e  # (Roger Goldman
+00004e80: 290a 2020 636f 6e74 6169 6e73 204d 616e  ).  contains Man
+00004e90: 7566 6163 7475 7265 7220 4745 0a20 202b  ufacturer GE.  +
+00004ea0: 2063 6f6e 7461 696e 7320 4d61 6e75 6661   contains Manufa
+00004eb0: 6374 7572 6572 4d6f 6465 6c4e 616d 6520  cturerModelName 
+00004ec0: 4745 7c53 7461 6e66 6f72 640a 2020 2b20  GE|Stanford.  + 
+00004ed0: 636f 6e74 6169 6e73 2049 6d61 6765 5479  contains ImageTy
+00004ee0: 7065 2044 4552 4956 4544 2b53 4543 4f4e  pe DERIVED+SECON
+00004ef0: 4441 5259 2b53 4352 4545 4e20 5341 5645  DARY+SCREEN SAVE
+00004f00: 0a20 2063 6f6f 7264 696e 6174 6573 2030  .  coordinates 0
+00004f10: 2c30 2c35 3132 2c31 3231 0a0a 4c41 4245  ,0,512,121..LABE
+00004f20: 4c20 5374 616e 666f 7264 204d 6564 6963  L Stanford Medic
+00004f30: 696e 6520 4f75 7470 6174 6965 6e74 2063  ine Outpatient c
+00004f40: 656e 7465 720a 2020 636f 6e74 6169 6e73  enter.  contains
+00004f50: 204d 616e 7566 6163 7475 7265 7220 5369   Manufacturer Si
+00004f60: 656d 656e 730a 2020 2b20 636f 6e74 6169  emens.  + contai
+00004f70: 6e73 204d 616e 7566 6163 7475 7265 724d  ns ManufacturerM
+00004f80: 6f64 656c 4e61 6d65 2053 4f4d 4154 4f4d  odelName SOMATOM
+00004f90: 2044 6566 696e 6974 696f 6e20 4153 2b0a   Definition AS+.
+00004fa0: 2020 2b20 636f 6e74 6169 6e73 2049 6d61    + contains Ima
+00004fb0: 6765 5479 7065 2044 4552 4956 4544 7c53  geType DERIVED|S
+00004fc0: 4543 4f4e 4441 5259 7c53 4352 4545 4e20  ECONDARY|SCREEN 
+00004fd0: 5341 5645 7c56 4f4c 5245 4e7c 5658 544c  SAVE|VOLREN|VXTL
+00004fe0: 2053 5441 5445 0a0a 2566 696c 7465 7220   STATE..%filter 
+00004ff0: 626c 6163 6b6c 6973 740a 0a4c 4142 454c  blacklist..LABEL
+00005000: 2041 6e79 2053 6361 6e6e 6564 2044 6f63   Any Scanned Doc
+00005010: 756d 656e 7420 6f72 2053 6563 6f6e 6461  ument or Seconda
+00005020: 7279 2053 6176 650a 2020 636f 6e74 6169  ry Save.  contai
+00005030: 6e73 2049 6d61 6765 5479 7065 2053 6563  ns ImageType Sec
+00005040: 6f6e 6461 7279 0a20 2063 6f6e 7461 696e  ondary.  contain
+00005050: 7320 4d6f 6461 6c69 7479 204f 540a 0a4c  s Modality OT..L
+00005060: 4142 454c 2041 6e79 2052 4550 4f52 5444  ABEL Any REPORTD
+00005070: 4154 410a 2020 636f 6e74 6169 6e73 2049  ATA.  contains I
+00005080: 6d61 6765 5479 7065 2052 4550 4f52 5444  mageType REPORTD
+00005090: 4154 410a 0a4c 4142 454c 2041 6e79 2044  ATA..LABEL Any D
+000050a0: 454d 4f47 5241 5048 4943 4441 5441 2c20  EMOGRAPHICDATA, 
+000050b0: 494e 5641 4c49 4420 2320 2841 4d42 290a  INVALID # (AMB).
+000050c0: 2020 636f 6e74 6169 6e73 2049 6d61 6765    contains Image
+000050d0: 5479 7065 2044 454d 4f47 5241 5048 4943  Type DEMOGRAPHIC
+000050e0: 4441 5441 0a20 2063 6f6e 7461 696e 7320  DATA.  contains 
+000050f0: 496d 6167 6554 7970 6520 494e 5641 4c49  ImageType INVALI
+00005100: 440a 0a4c 4142 454c 2053 7461 6e66 6f72  D..LABEL Stanfor
+00005110: 6420 426c 6163 6b6c 6973 7420 4d69 7373  d Blacklist Miss
+00005120: 696e 6720 496d 6167 6554 7970 6520 2023  ing ImageType  #
+00005130: 2053 7573 616e 2057 6562 6572 2c20 5661   Susan Weber, Va
+00005140: 6e65 7373 6120 536f 6368 6174 0a20 206d  nessa Sochat.  m
+00005150: 6973 7369 6e67 2049 6d61 6765 5479 7065  issing ImageType
+00005160: 207c 7c20 656d 7074 7920 496d 6167 6554   || empty ImageT
+00005170: 7970 650a 0a4c 4142 454c 2053 7461 6e66  ype..LABEL Stanf
+00005180: 6f72 6420 426c 6163 6b6c 6973 7420 7365  ord Blacklist se
+00005190: 636f 6e64 6172 7920 6f72 2064 6572 6976  condary or deriv
+000051a0: 6564 2063 6174 6368 616c 6c20 2320 5661  ed catchall # Va
+000051b0: 6e65 7373 6120 536f 6368 6174 0a20 2063  nessa Sochat.  c
+000051c0: 6f6e 7461 696e 7320 4d6f 6461 6c69 7479  ontains Modality
+000051d0: 2043 547c 4d52 0a20 202b 2063 6f6e 7461   CT|MR.  + conta
+000051e0: 696e 7320 496d 6167 6554 7970 6520 4445  ins ImageType DE
+000051f0: 5249 5645 447c 5345 434f 4e44 4152 597c  RIVED|SECONDARY|
+00005200: 5343 5245 454e 7c53 4156 450a 0a4c 4142  SCREEN|SAVE..LAB
+00005210: 454c 2053 7461 6e66 6f72 6420 426c 6163  EL Stanford Blac
+00005220: 6b6c 6973 7420 446f 7365 2052 6570 6f72  klist Dose Repor
+00005230: 7420 6f72 2045 7874 6572 6e61 6c20 2320  t or External # 
+00005240: 5661 6e65 7373 6120 536f 6368 6174 0a20  Vanessa Sochat. 
+00005250: 2063 6f6e 7461 696e 7320 4d6f 6461 6c69   contains Modali
+00005260: 7479 2043 547c 4d52 0a20 202b 2063 6f6e  ty CT|MR.  + con
+00005270: 7461 696e 7320 5365 7269 6573 4465 7363  tains SeriesDesc
+00005280: 7269 7074 696f 6e20 5061 7469 656e 7420  ription Patient 
+00005290: 5072 6f74 6f63 6f6c 7c50 4143 5320 6e6f  Protocol|PACS no
+000052a0: 6d69 6e61 7469 6f6e 2066 6f72 6d7c 446f  mination form|Do
+000052b0: 7365 2052 6570 6f72 747c 5374 7564 7920  se Report|Study 
+000052c0: 6163 7175 6972 6564 206f 7574 7369 6465  acquired outside
+000052d0: 2068 6f73 7069 7461 6c0a 0a4c 4142 454c   hospital..LABEL
+000052e0: 2042 7572 6e65 6420 496e 2041 6e6e 6f74   Burned In Annot
+000052f0: 6174 696f 6e20 2320 2843 5450 290a 2020  ation # (CTP).  
+00005300: 636f 6e74 6169 6e73 2049 6d61 6765 5479  contains ImageTy
+00005310: 7065 2053 4156 450a 2020 2b20 636f 6e74  pe SAVE.  + cont
+00005320: 6169 6e73 204d 6f64 616c 6974 7920 4354  ains Modality CT
+00005330: 7c4d 520a 2020 7c7c 2063 6f6e 7461 696e  |MR.  || contain
+00005340: 7320 5365 7269 6573 4465 7363 7269 7074  s SeriesDescript
+00005350: 696f 6e20 5341 5645 0a20 207c 7c20 636f  ion SAVE.  || co
+00005360: 6e74 6169 6e73 2042 7572 6e65 6449 6e41  ntains BurnedInA
+00005370: 6e6e 6f74 6174 696f 6e20 5945 530a 2020  nnotation YES.  
+00005380: 7c7c 2065 6d70 7479 2049 6d61 6765 5479  || empty ImageTy
+00005390: 7065 0a20 207c 7c20 656d 7074 7920 4461  pe.  || empty Da
+000053a0: 7465 4f66 5365 636f 6e64 6172 7943 6170  teOfSecondaryCap
+000053b0: 7475 7265 0a20 207c 7c20 656d 7074 7920  ture.  || empty 
+000053c0: 5365 636f 6e64 6172 7943 6170 7475 7265  SecondaryCapture
+000053d0: 4465 7669 6365 4d61 6e75 6661 6374 7572  DeviceManufactur
+000053e0: 6572 0a20 207c 7c20 656d 7074 7920 5365  er.  || empty Se
+000053f0: 636f 6e64 6172 7943 6170 7475 7265 4465  condaryCaptureDe
+00005400: 7669 6365 4d61 6e75 6661 6374 7572 6572  viceManufacturer
+00005410: 4d6f 6465 6c4e 616d 650a 2020 7c7c 2065  ModelName.  || e
+00005420: 6d70 7479 2053 6563 6f6e 6461 7279 4361  mpty SecondaryCa
+00005430: 7074 7572 6544 6576 6963 6553 6f66 7477  ptureDeviceSoftw
+00005440: 6172 6556 6572 7369 6f6e 730a 0a0a 2568  areVersions...%h
+00005450: 6561 6465 720a 0a52 454d 4f56 4520 656e  eader..REMOVE en
+00005460: 6473 7769 7468 3a54 696d 650a 5245 4d4f  dswith:Time.REMO
+00005470: 5645 2065 6e64 7377 6974 683a 4461 7465  VE endswith:Date
+00005480: 0a52 454d 4f56 4520 656e 6473 7769 7468  .REMOVE endswith
+00005490: 3a74 696d 650a 5245 4d4f 5645 2041 6464  :time.REMOVE Add
+000054a0: 6974 696f 6e61 6c50 6174 6965 6e74 4869  itionalPatientHi
+000054b0: 7374 6f72 790a 5245 4d4f 5645 2041 6363  story.REMOVE Acc
+000054c0: 6573 7369 6f6e 4e75 6d62 6572 0a52 454d  essionNumber.REM
+000054d0: 4f56 4520 5061 7469 656e 7449 440a 5245  OVE PatientID.RE
+000054e0: 4d4f 5645 2073 7461 7274 7377 6974 683a  MOVE startswith:
+000054f0: 4973 7375 6544 6174 650a 5245 4d4f 5645  IssueDate.REMOVE
+00005500: 2049 7373 7565 724f 6650 6174 6965 6e74   IssuerOfPatient
+00005510: 4944 0a52 454d 4f56 4520 4669 6c6c 6572  ID.REMOVE Filler
+00005520: 4f72 6465 724e 756d 6265 7249 6d61 6769  OrderNumberImagi
+00005530: 6e67 5365 7276 6963 6552 6571 7565 7374  ngServiceRequest
+00005540: 0a52 454d 4f56 4520 4f74 6865 7250 6174  .REMOVE OtherPat
+00005550: 6965 6e74 4944 730a 5245 4d4f 5645 204f  ientIDs.REMOVE O
+00005560: 7468 6572 5061 7469 656e 744e 616d 6573  therPatientNames
+00005570: 0a52 454d 4f56 4520 4f74 6865 7250 6174  .REMOVE OtherPat
+00005580: 6965 6e74 4944 7353 6571 7565 6e63 650a  ientIDsSequence.
+00005590: 5245 4d4f 5645 2050 6174 6965 6e74 4164  REMOVE PatientAd
+000055a0: 6472 6573 730a 5245 4d4f 5645 2050 6174  dress.REMOVE Pat
+000055b0: 6965 6e74 4269 7274 684e 616d 650a 5245  ientBirthName.RE
+000055c0: 4d4f 5645 2050 6174 6965 6e74 4d6f 7468  MOVE PatientMoth
+000055d0: 6572 4269 7274 684e 616d 650a 5245 4d4f  erBirthName.REMO
+000055e0: 5645 2050 6174 6965 6e74 4e61 6d65 0a52  VE PatientName.R
+000055f0: 454d 4f56 4520 5061 7469 656e 7473 4e61  EMOVE PatientsNa
+00005600: 6d65 0a52 454d 4f56 4520 5265 6173 6f6e  me.REMOVE Reason
+00005610: 466f 7253 7475 6479 0a52 454d 4f56 4520  ForStudy.REMOVE 
+00005620: 636f 6e74 6169 6e73 3a54 7269 616c 0a52  contains:Trial.R
+00005630: 454d 4f56 4520 7374 6172 7473 7769 7468  EMOVE startswith
+00005640: 3a50 6174 6965 6e74 5465 6c65 7068 6f6e  :PatientTelephon
+00005650: 654e 756d 6265 720a 5245 4d4f 5645 2065  eNumber.REMOVE e
+00005660: 6e64 7377 6974 683a 4944 0a52 454d 4f56  ndswith:ID.REMOV
+00005670: 4520 656e 6473 7769 7468 3a49 4473 0a52  E endswith:IDs.R
+00005680: 454d 4f56 4520 5265 6665 7272 696e 6750  EMOVE ReferringP
+00005690: 6879 7369 6369 616e 4e61 6d65 0a52 454d  hysicianName.REM
+000056a0: 4f56 4520 436f 6e73 756c 7469 6e67 5068  OVE ConsultingPh
+000056b0: 7973 6963 6961 6e4e 616d 650a 5245 4d4f  ysicianName.REMO
+000056c0: 5645 2045 7661 6c75 6174 6f72 4e61 6d65  VE EvaluatorName
+000056d0: 0a52 454d 4f56 4520 5065 7266 6f72 6d65  .REMOVE Performe
+000056e0: 6453 7461 7469 6f6e 4e61 6d65 0a52 454d  dStationName.REM
+000056f0: 4f56 4520 5365 636f 6e64 6172 7952 6576  OVE SecondaryRev
+00005700: 6965 7765 724e 616d 650a 5245 4d4f 5645  iewerName.REMOVE
+00005710: 2050 6572 736f 6e4e 616d 650a 5245 4d4f   PersonName.REMO
+00005720: 5645 2050 6572 736f 6e41 6464 7265 7373  VE PersonAddress
+00005730: 0a52 454d 4f56 4520 5265 6665 7272 696e  .REMOVE Referrin
+00005740: 6750 6879 7369 6369 616e 4164 6472 6573  gPhysicianAddres
+00005750: 730a 5245 4d4f 5645 2052 6566 6572 7269  s.REMOVE Referri
+00005760: 6e67 5068 7973 6963 6961 6e54 656c 6570  ngPhysicianTelep
+00005770: 686f 6e65 4e75 6d62 6572 730a 5245 4d4f  honeNumbers.REMO
+00005780: 5645 2052 6566 6572 7269 6e67 5068 7973  VE ReferringPhys
+00005790: 6963 6961 6e49 6465 6e74 6966 6963 6174  icianIdentificat
+000057a0: 696f 6e53 6571 7565 6e63 650a 5245 4d4f  ionSequence.REMO
+000057b0: 5645 2043 6f6e 7375 6c74 696e 6750 6879  VE ConsultingPhy
+000057c0: 7369 6369 616e 4964 656e 7469 6669 6361  sicianIdentifica
+000057d0: 7469 6f6e 5365 7175 656e 6365 0a52 454d  tionSequence.REM
+000057e0: 4f56 4520 5068 7973 6963 6961 6e41 7070  OVE PhysicianApp
+000057f0: 726f 7669 6e67 496e 7465 7270 7265 7461  rovingInterpreta
+00005800: 7469 6f6e 0a52 454d 4f56 4520 5068 7973  tion.REMOVE Phys
+00005810: 6963 6961 6e73 4f66 5265 636f 7264 0a52  iciansOfRecord.R
+00005820: 454d 4f56 4520 5068 7973 6963 6961 6e73  EMOVE Physicians
+00005830: 4f66 5265 636f 7264 4964 656e 7469 6669  OfRecordIdentifi
+00005840: 6361 7469 6f6e 5365 7175 656e 6365 0a52  cationSequence.R
+00005850: 454d 4f56 4520 5065 7266 6f72 6d69 6e67  EMOVE Performing
+00005860: 5068 7973 6963 6961 6e4e 616d 650a 5245  PhysicianName.RE
+00005870: 4d4f 5645 2050 6572 666f 726d 696e 6750  MOVE PerformingP
+00005880: 6879 7369 6369 616e 4964 656e 7469 6669  hysicianIdentifi
+00005890: 6361 7469 6f6e 5365 7175 656e 6365 0a52  cationSequence.R
+000058a0: 454d 4f56 4520 5068 7973 6963 6961 6e73  EMOVE Physicians
+000058b0: 5265 6164 696e 6753 7475 6479 4964 656e  ReadingStudyIden
+000058c0: 7469 6669 6361 7469 6f6e 5365 7175 656e  tificationSequen
+000058d0: 6365 0a52 454d 4f56 4520 5265 7175 6573  ce.REMOVE Reques
+000058e0: 7469 6e67 5068 7973 6963 6961 6e0a 5245  tingPhysician.RE
+000058f0: 4d4f 5645 2053 6368 6564 756c 6564 5065  MOVE ScheduledPe
+00005900: 7266 6f72 6d69 6e67 5068 7973 6963 6961  rformingPhysicia
+00005910: 6e49 6465 6e74 6966 6963 6174 696f 6e53  nIdentificationS
+00005920: 6571 7565 6e63 650a 5245 4d4f 5645 2052  equence.REMOVE R
+00005930: 6571 7565 7374 696e 6750 6879 7369 6369  equestingPhysici
+00005940: 616e 4964 656e 7469 6669 6361 7469 6f6e  anIdentification
+00005950: 5365 7175 656e 6365 0a52 454d 4f56 4520  Sequence.REMOVE 
+00005960: 4875 6d61 6e50 6572 666f 726d 6572 4e61  HumanPerformerNa
+00005970: 6d65 0a52 454d 4f56 4520 436f 6e74 6163  me.REMOVE Contac
+00005980: 7444 6973 706c 6179 4e61 6d65 0a52 454d  tDisplayName.REM
+00005990: 4f56 4520 5065 7266 6f72 6d69 6e67 5068  OVE PerformingPh
+000059a0: 7973 6963 6961 6e4e 616d 650a 5245 4d4f  ysicianName.REMO
+000059b0: 5645 204e 616d 654f 6650 6879 7369 6369  VE NameOfPhysici
+000059c0: 616e 7352 6561 6469 6e67 5374 7564 790a  ansReadingStudy.
+000059d0: 5245 4d4f 5645 204f 7065 7261 746f 7273  REMOVE Operators
+000059e0: 4e61 6d65 0a52 454d 4f56 4520 5363 6865  Name.REMOVE Sche
+000059f0: 6475 6c65 6450 6572 666f 726d 696e 6750  duledPerformingP
+00005a00: 6879 7369 6369 616e 4e61 6d65 0a52 454d  hysicianName.REM
+00005a10: 4f56 4520 5265 7669 6577 6572 4e61 6d65  OVE ReviewerName
+00005a20: 0a52 454d 4f56 4520 4e61 6d65 734f 6649  .REMOVE NamesOfI
+00005a30: 6e74 656e 6465 6452 6563 6970 6965 6e74  ntendedRecipient
+00005a40: 734f 6652 6573 756c 7473 0a52 454d 4f56  sOfResults.REMOV
+00005a50: 4520 536f 7572 6365 4170 706c 6963 6174  E SourceApplicat
+00005a60: 6f72 4e61 6d65 0a52 454d 4f56 4520 436c  orName.REMOVE Cl
+00005a70: 696e 6963 616c 5472 6961 6c53 706f 6e73  inicalTrialSpons
+00005a80: 6f72 4e61 6d65 0a52 454d 4f56 4520 436f  orName.REMOVE Co
+00005a90: 6e74 656e 7443 7265 6174 6f72 4e61 6d65  ntentCreatorName
+00005aa0: 0a52 454d 4f56 4520 436c 696e 6963 616c  .REMOVE Clinical
+00005ab0: 5472 6961 6c50 726f 746f 636f 6c45 7468  TrialProtocolEth
+00005ac0: 6963 7343 6f6d 6d69 7474 6565 4e61 6d65  icsCommitteeName
+00005ad0: 0a52 454d 4f56 4520 636f 6e74 6169 6e73  .REMOVE contains
+00005ae0: 3a55 4944 0a52 454d 4f56 4520 5265 6769  :UID.REMOVE Regi
+00005af0: 6f6e 4f66 5265 7369 6465 6e63 650a 5245  onOfResidence.RE
+00005b00: 4d4f 5645 2043 7572 7265 6e74 5061 7469  MOVE CurrentPati
+00005b10: 656e 744c 6f63 6174 696f 6e0a 5245 4d4f  entLocation.REMO
+00005b20: 5645 2050 6174 6965 6e74 436f 6d6d 656e  VE PatientCommen
+00005b30: 7473 0a52 454d 4f56 4520 5061 7469 656e  ts.REMOVE Patien
+00005b40: 7454 7261 6e73 706f 7274 4172 7261 6e67  tTransportArrang
+00005b50: 656d 656e 7473 0a52 454d 4f56 4520 5061  ements.REMOVE Pa
+00005b60: 7469 656e 7444 6561 7468 4461 7465 496e  tientDeathDateIn
+00005b70: 416c 7465 726e 6174 6976 6543 616c 656e  AlternativeCalen
+00005b80: 6461 720a 5245 4d4f 5645 2050 6174 6965  dar.REMOVE Patie
+00005b90: 6e74 496e 7374 6974 7574 696f 6e52 6573  ntInstitutionRes
+00005ba0: 6964 656e 6365 0a52 454d 4f56 4520 5065  idence.REMOVE Pe
+00005bb0: 7266 6f72 6d65 644c 6f63 6174 696f 6e0a  rformedLocation.
+00005bc0: 5245 4d4f 5645 2053 6368 6564 756c 6564  REMOVE Scheduled
+00005bd0: 5374 7564 794c 6f63 6174 696f 6e0a 5245  StudyLocation.RE
+00005be0: 4d4f 5645 2053 6368 6564 756c 6564 5374  MOVE ScheduledSt
+00005bf0: 7564 794c 6f63 6174 696f 6e41 4554 6974  udyLocationAETit
+00005c00: 6c65 0a52 454d 4f56 4520 4f72 6465 7245  le.REMOVE OrderE
+00005c10: 6e74 6572 6572 4c6f 6361 7469 6f6e 0a52  ntererLocation.R
+00005c20: 454d 4f56 4520 4173 7369 676e 6564 4c6f  EMOVE AssignedLo
+00005c30: 6361 7469 6f6e 0a0a 4144 4420 4973 7375  cation..ADD Issu
+00005c40: 6572 4f66 5061 7469 656e 7449 4420 5354  erOfPatientID ST
+00005c50: 4152 520a 4144 4420 5061 7469 656e 7442  ARR.ADD PatientB
+00005c60: 6972 7468 4461 7465 2076 6172 3a65 6e74  irthDate var:ent
+00005c70: 6974 795f 7469 6d65 7374 616d 700a 4144  ity_timestamp.AD
+00005c80: 4420 5374 7564 7944 6174 6520 7661 723a  D StudyDate var:
+00005c90: 6974 656d 5f74 696d 6573 7461 6d70 0a41  item_timestamp.A
+00005ca0: 4444 2050 6174 6965 6e74 4944 2076 6172  DD PatientID var
+00005cb0: 3a65 6e74 6974 795f 6964 0a41 4444 2041  :entity_id.ADD A
+00005cc0: 6363 6573 7369 6f6e 4e75 6d62 6572 2076  ccessionNumber v
+00005cd0: 6172 3a69 7465 6d5f 6964 0a41 4444 2050  ar:item_id.ADD P
+00005ce0: 6174 6965 6e74 4964 656e 7469 7479 5265  atientIdentityRe
+00005cf0: 6d6f 7665 6420 5945 530a 5245 4d4f 5645  moved YES.REMOVE
+00005d00: 206a 6974 7465 720a                       jitter.
```

### Comparing `deid-0.3.21/deid/data/deid.dicom.ultrasound` & `deid-0.3.22/deid/data/deid.dicom.ultrasound`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/deid/data/deid.dicom.xray.chest` & `deid-0.3.22/deid/data/deid.dicom.xray.chest`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/deid/dicom/actions/jitter.py` & `deid-0.3.22/deid/dicom/actions/jitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 from deid.logger import bot
 from deid.utils import get_timestamp, parse_keyvalue_pairs
 
 # Timestamps
 
@@ -39,15 +39,14 @@
     if not isinstance(value, int):
         value = int(value)
 
     original = field.element.value
     new_value = original
 
     if original is not None:
-
         # Create default for new value
         new_value = None
         dcmvr = field.element.VR
 
         # DICOM Value Representation can be either DA (Date) DT (Timestamp),
         # or something else, which is not supported.
         if dcmvr == "DA":
@@ -63,15 +62,14 @@
                 )
             except Exception:
                 new_value = get_timestamp(
                     original, jitter_days=value, format="%Y%m%d%H%M%S.%f"
                 )
 
         else:
-
             # If the field type is not supplied, attempt to parse different formats
             for fmtstr in ["%Y%m%d", "%Y%m%d%H%M%S.%f%z", "%Y%m%d%H%M%S.%f"]:
                 try:
                     new_value = get_timestamp(
                         original, jitter_days=value, format=fmtstr
                     )
                     break
```

### Comparing `deid-0.3.21/deid/dicom/actions/uids.py` & `deid-0.3.22/deid/dicom/actions/uids.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import uuid
 
 from pydicom.uid import generate_uid as pydicom_generate_uid
 
 from deid.logger import bot
```

### Comparing `deid-0.3.21/deid/dicom/config.json` & `deid-0.3.22/deid/dicom/config.json`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/deid/dicom/fields.py` & `deid-0.3.22/deid/dicom/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import re
 
 from pydicom.dataelem import DataElement
 from pydicom.dataset import Dataset, FileMetaDataset, RawDataElement
 from pydicom.sequence import Sequence
@@ -153,15 +153,14 @@
     Parameters
     ==========
     sequence: the sequence to extract, should be pydicom.sequence.Sequence
     prefix: the parent name
     """
     items = {}
     for item in sequence:
-
         # If it's a Dataset, we need to further unwrap it
         if isinstance(item, Dataset):
             for subitem in item:
                 items.update(extract_item(subitem, prefix=prefix))
 
         # Private tags are DataElements
         elif isinstance(item, DataElement):
@@ -220,15 +219,14 @@
     if expander.lower() == "endswith":
         expression = "(%s)$" % expression
     elif expander.lower() == "startswith":
         expression = "^(%s)" % expression
 
     # Loop through fields, all are strings STOPPED HERE NEED TO ADDRESS EMPTY NAME
     for uid, field in contenders.items():
-
         # Apply expander to string for name OR to tag string
         if expander.lower() in ["endswith", "startswith", "contains"]:
             if field.name_contains(expression):
                 fields[uid] = field
 
         elif expander.lower() == "except":
             if not field.name_contains(expression):
@@ -266,26 +264,24 @@
         different.
         """
         if uid not in seen:
             fields[uid] = DicomField(element, name, uid, is_filemeta)
             seen.append(uid)
 
     while datasets:
-
         # Grab the first dataset, usually just the dicom
         dataset = datasets.pop(0)
 
         # If the dataset does not have a prefix, we are at the start
         dataset.prefix = getattr(dataset, "prefix", None)
         dataset.uid = getattr(dataset, "uid", None)
         is_filemeta = isinstance(dataset, FileMetaDataset)
 
         # Includes private tags, sequences flattened, non-null values
         for contender in dataset:
-
             # All items should be data elements, skip based on keyword or tag
             if contender.keyword in skip or str(contender.tag) in skip:
                 continue
 
             # The name represents nesting
             name = contender.keyword
             uid = str(contender.tag)
@@ -293,15 +289,14 @@
             if dataset.prefix is not None:
                 name = "%s__%s" % (dataset.prefix, name)
             if dataset.uid is not None:
                 uid = "%s__%s" % (dataset.uid, uid)
 
             # if it's a sequence, extract with prefix and index
             if isinstance(contender.value, Sequence) and expand_sequences is True:
-
                 # Add the contender (usually type Dataset) to fields
                 add_element(contender, name, uid, is_filemeta)
 
                 # A nested dataset can be parsed as such
                 for idx, item in enumerate(contender.value):
                     if isinstance(item, Dataset):
                         item.prefix = name
```

### Comparing `deid-0.3.21/deid/dicom/filter.py` & `deid-0.3.22/deid/dicom/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import re
 
 from pydicom.dataset import Dataset
 
 from deid.logger import bot
@@ -20,19 +20,22 @@
 
 def apply_filter(dicom, field, filter_name, value):
     """essentially a switch statement to apply a filter to a dicom file.
 
     Parameters
     ==========
     dicom: the pydicom.dataset Dataset (pydicom.read_file)
-    field: the name of the field to apply the filter to
+    field: the name of the field to apply the filter to,
+      or the tag number as a string '0xGGGGEEEE'
     filer_name: the name of the filter to apply (e.g., contains)
     value: the value to set, if filter_name is valid
 
     """
+    if "0x" in field:
+        field = int(field, 0)  # 0=decode hex with 0x prefix
     filter_name = filter_name.lower().strip()
 
     if filter_name == "contains":
         return dicom.contains(field, value)
 
     if filter_name == "notcontains":
         return dicom.notContains(field, value)
@@ -70,15 +73,14 @@
 
     if not isinstance(contenders, list):
         contenders = [contenders]
 
     # In this loop we can only switch to True
     for contender in contenders:
         if contender is not None:
-
             try:
                 # both converted to string (handles tags)
                 contender = str(contender)
                 term = str(term)
 
                 if ignore_case:
                     contender = contender.lower().strip()
@@ -183,15 +185,14 @@
     contenders = self.get(field)
 
     if not isinstance(contenders, list):
         contenders = [contenders]
 
     for contender in contenders:
         if contender is not None:
-
             try:
                 contender = str(contender)
                 expression = str(expression)
 
                 if ignore_case:
                     contender = contender.lower().strip()
                     expression = expression.lower().strip()
```

### Comparing `deid-0.3.21/deid/dicom/groups.py` & `deid-0.3.22/deid/dicom/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 
 from pydicom.multival import MultiValue
 
 from deid.logger import bot
 
@@ -19,15 +19,14 @@
     values = set()
 
     # The function can be provided fields to save re-parsing
     if not fields:
         fields = get_fields(dicom)
 
     for action in actions:
-
         # Extract some subset of fields based on action
         subset = expand_field_expression(
             field=action["field"], dicom=dicom, contenders=fields
         )
 
         # Just grab the entire value string for a field, no parsing
         if action["action"] == "FIELD":
@@ -36,15 +35,14 @@
                     if isinstance(field.element.value, MultiValue):
                         values.update(field.element.value)
                     else:
                         values.add(field.element.value)
 
         # Split action, can optionally have a "by" and/or minlength parameter
         elif action["action"] == "SPLIT":
-
             # Default values for split are length 1 and character empty space
             bot.debug("Parsing action %s" % action)
             split_by = " "
             minlength = 1
 
             if "value" in action:
                 for param in action["value"].split(";"):
@@ -82,15 +80,14 @@
     """
     subset = {}
 
     if not fields:
         fields = get_fields(dicom)
 
     for action in actions:
-
         if action["action"] == "FIELD":
             subset.update(
                 expand_field_expression(
                     field=action["field"], dicom=dicom, contenders=fields
                 )
             )
```

### Comparing `deid-0.3.21/deid/dicom/header.py` & `deid-0.3.22/deid/dicom/header.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 
 import os
 
 from pydicom import read_file
 
@@ -52,15 +52,14 @@
 
     return lookup
 
 
 def remove_private_identifiers(
     dicom_files, save=True, overwrite=False, output_folder=None, force=True
 ):
-
     """
     Remove private identifiers.
 
     remove_private_identifiers is a wrapper for the
     simple call to dicom.remove_private_tags, it simply
     reads in the files for the user and saves accordingly
     """
@@ -95,15 +94,14 @@
     output_folder=None,
     force=True,
     config=None,
     strip_sequences=False,
     remove_private=False,
     disable_skip=False,
 ):
-
     """
     Replace identifiers.
 
     replace identifiers using pydicom, can be slow when writing
     and saving new files. If you want to replace sequences, they need
     to be extracted with get_identifiers and expand_sequences to True.
     """
```

### Comparing `deid-0.3.21/deid/dicom/parser.py` & `deid-0.3.22/deid/dicom/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import os
 import re
 from copy import deepcopy
 
 from pydicom import read_file
@@ -146,24 +146,22 @@
                 ]
                 group = int(group, 16)
                 element = int(element, 16)
                 tag = Tag(group, element)
 
                 # We keep going until we find the desired tag
                 if tag != desired:
-
                     # If the parent has been removed, we can't continue
                     if tag not in parent:
                         return None, desired
 
                     parent = parent[tag]
 
             # Otherwise it's an index into a sequence
             else:
-
                 # If the sequence is outside the bounds of the array of items
                 # within the sequence, we can't continue.
                 if int(uid) < 0 or int(uid) >= len(parent.value):
                     return None, desired
                 parent = parent[int(uid)]
 
         if return_parent:
@@ -220,15 +218,14 @@
             self.remove_private()
 
         # In the parsing, we generate a list of DicomField objects.
         fields = self.get_fields(expand_sequences=True)
 
         # if we loaded a deid recipe
         if self.recipe.deid is not None:
-
             # Prepare additional lists of values and lookup fields (index by nested uid)
             if self.recipe.has_values_lists():
                 for group, actions in self.recipe.get_values_lists().items():
                     self.lookup[group] = extract_values_list(
                         dicom=self.dicom, actions=actions, fields=fields
                     )
 
@@ -457,15 +454,14 @@
             if is_filemeta:
                 self.dicom.file_meta.add(element)
             else:
                 self.dicom.add(element)
 
         # Assume we don't want to add an empty value
         if value is not None:
-
             # If provided a field object, create based on keyword or tag identifier
             name = field
             if isinstance(field, DicomField):
                 name = field.element.keyword or field.stripped_tag
 
             # Generate a tag item, add if it's a name found in the dicom dictionary
             tag = get_tag(name)
@@ -537,15 +533,14 @@
             else:
                 bot.warning("JITTER %s unsuccessful" % field)
 
         # elif "KEEP" --> Do nothing. Keep the original
 
         # Remove the field entirely
         elif action == "REMOVE":
-
             # If a value is defined, parse it (could be filter)
             do_removal = True
             if value is not None:
                 do_removal = parse_value(
                     item=self.lookup,
                     dicom=self.dicom,
                     value=value,
```

### Comparing `deid-0.3.21/deid/dicom/pixels/clean.py` & `deid-0.3.22/deid/dicom/pixels/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 
 import math
 import os
 import random
 import re
@@ -46,15 +46,14 @@
         output_folder=None,
         add_padding=False,
         margin=3,
         deid=None,
         font=None,
         force=True,
     ):
-
         if output_folder is None:
             output_folder = get_temporary_name(prefix="clean")
 
         if font is None:
             font = self.default_font()
         self.font = font
         self.cmap = "gray"
@@ -85,15 +84,14 @@
         )
         self.dicom_file = dicom_file
         return self.results
 
     def clean(
         self, fix_interpretation: bool = True, pixel_data_attribute: str = "PixelData"
     ) -> Optional[NDArray]:
-
         if not self.results:
             bot.warning(
                 "Use %s.detect() with a dicom file to find coordinates first." % self
             )
             return
 
         bot.info("Scrubbing %s." % self.dicom_file)
@@ -308,29 +306,25 @@
         original = dicom.pixel_array
 
     # Compile coordinates from result, generate list of tuples with coordinate and value
     # keepcoordinates == 1 (included in mask) and coordinates == 0 (remove).
     coordinates = []
 
     for item in results["results"]:
-
         # We iterate through coordinates in order specified in file
         for coordinate_set in item.get("coordinates", []):
-
             # Each is a list with [value, coordinate]
             mask_value, new_coordinates = coordinate_set
 
             if not isinstance(new_coordinates, list):
                 new_coordinates = [new_coordinates]
 
             for new_coordinate in new_coordinates:
-
                 # Case 1: an "all" indicates applying to entire image
                 if new_coordinate.lower() == "all":
-
                     # 2D - Greyscale Image - Shape = (X, Y) OR 3D - RGB Image - Shape = (X, Y, Channel)
                     if len(original.shape) == 2 or (
                         len(original.shape) == 3 and dicom.SamplesPerPixel == 3
                     ):
                         # minr, minc, maxr, maxc = [0, 0, Y, X]
                         new_coordinate = [
                             0,
@@ -371,30 +365,28 @@
 
         # Update the mask: values set to 0 to be black
         mask[minc:maxc, minr:maxr] = coordinate_value
 
     # Now apply finished mask to the data
     # RGB cine clip
     if len(original.shape) == 4:
-
         # np.tile does the copying and stacking of masks into the channel dim to produce 3D masks
         # transposition to convert tile output (channel, X, Y)  into (X, Y, channel)
         # see: https://github.com/nquach/anonymize/blob/master/anonymize.py#L154
         channel3mask = numpy.transpose(numpy.tile(mask, (3, 1, 1)), (1, 2, 0))
 
         # use numpy.tile to copy and stack the 3D masks into 4D array to apply to 4D pixel data
         # tile converts (X, Y, channels) -> (frames, X, Y, channels), presumed ordering for 4D pixel data
         final_mask = numpy.tile(channel3mask, (original.shape[0], 1, 1, 1))
 
         # apply final 4D mask to 4D pixel data
         cleaned = final_mask * original
 
     # RGB image or Greyscale cine clip
     elif len(original.shape) == 3:
-
         # This condition is ambiguous.  If the image shape is 3, we may have a single frame RGB image: size (X, Y, channel)
         # or a multiframe greyscale image: size (frames, X, Y).  Interrogate the SamplesPerPixel field.
         if dicom.SamplesPerPixel == 3:
             # RGB Image
             # Convert (X, Y) -> (X, Y, channel)
             final_mask = numpy.transpose(
                 numpy.tile(mask, (original.shape[2], 1, 1)), (1, 2, 0)
```

### Comparing `deid-0.3.21/deid/dicom/pixels/detect.py` & `deid-0.3.22/deid/dicom/pixels/detect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 
 from typing import List, Optional, Union
 
 from pydicom import FileDataset, read_file
 from pydicom.sequence import Sequence
@@ -62,15 +62,14 @@
         else:
             decision["flagged"][dicom_file] = result
 
     return decision
 
 
 def _has_burned_pixels_single(dicom_file, force: bool, deid):
-
     """
     Determine if a single dicom has burned pixels.
 
     has burned pixels single will evaluate one dicom file for burned in
     pixels based on 'filter' criteria in a deid. If deid is not provided,
     will use application default. The method proceeds as follows:
 
@@ -138,18 +137,16 @@
                 group_flags = [True]
                 group_descriptions = [item.get("name", "")]
 
             else:
                 group_flags = []  # evaluation for a single line
                 group_descriptions = []
                 for group in item["filters"]:
-
                     # You cannot pop from the list
                     for a in range(len(group["action"])):
-
                         action = group["action"][a]
                         field = group["field"][a]
                         value = ""
 
                         if len(group["value"]) > a:
                             value = group["value"][a]
 
@@ -264,22 +261,20 @@
         for entry in region:
             regions.append(entry)
     else:
         regions.append(region)
 
     # Now extract coordinates
     for region in regions:
-
         if (
             "RegionLocationMinX0" in region
             and "RegionLocationMinY0" in region
             and "RegionLocationMaxX1" in region
             and "RegionLocationMaxY1" in region
         ):
-
             # https://gist.github.com/vsoch/df6957be12c34e62b21000603f1687e5
             # minr, minc, maxr, maxc = coordinate
             # self.cleaned[minc:maxc, minr:maxr] = 0  # should fill with black
             # self.cleaned[A:B, C:D]
             # image[A:B,C:D]
             # A: refers to ymin
             # B: refers to ymax
```

### Comparing `deid-0.3.21/deid/dicom/tags.py` & `deid-0.3.22/deid/dicom/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import re
 
 from pydicom._dicom_dict import DicomDictionary, RepeatersDictionary
 from pydicom.sequence import Sequence
 from pydicom.tag import Tag, tag_in_exception
@@ -41,15 +41,14 @@
     """
     found = [
         {key: value} for key, value in DicomDictionary.items() if value[4] == field
     ]
     manifest = None
 
     if len(found) > 0:
-
         # (VR, VM, Name, Retired, Keyword
         found = found[0]  # shouldn't ever have length > 1
         tag = Tag(list(found)[0])
         VR, VM, longName, _, keyword = found[tag]
 
         manifest = {
             "tag": tag,
```

### Comparing `deid-0.3.21/deid/dicom/utils.py` & `deid-0.3.22/deid/dicom/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import os
 import tempfile
 import zipfile
 
 import pydicom
```

### Comparing `deid-0.3.21/deid/dicom/validate.py` & `deid-0.3.22/deid/dicom/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 from pydicom import read_file
 
 from deid.logger import bot
 
 
@@ -22,15 +22,14 @@
     if not isinstance(dcm_files, list):
         dcm_files = [dcm_files]
 
     valids = []
 
     bot.debug("Checking %s dicom files for validation." % (len(dcm_files)))
     for dcm_file in dcm_files:
-
         try:
             with open(dcm_file, "rb") as filey:
                 read_file(filey, force=force)
             valids.append(dcm_file)
         except Exception:
             bot.warning("Cannot read input file {0!s}, skipping.".format(dcm_file))
```

### Comparing `deid-0.3.21/deid/logger/message.py` & `deid-0.3.22/deid/logger/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 
 import os
 import sys
 
 ABORT = -5
@@ -307,15 +307,14 @@
     MESSAGELEVEL. if MESSAGELEVEL is not set, the maximum level
     (5) is assumed (all messages).
     """
     try:
         level = int(os.environ.get("MESSAGELEVEL", DEBUG))
 
     except ValueError:
-
         level = os.environ.get("MESSAGELEVEL", DEBUG)
         if level == "CRITICAL":
             return FLAG
         elif level == "ABORT":
             return ABORT
         elif level == "ERROR":
             return ERROR
```

### Comparing `deid-0.3.21/deid/logger/progress.py` & `deid-0.3.22/deid/logger/progress.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/deid/main/__init__.py` & `deid-0.3.22/deid/main/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import argparse
 import os
 import sys
 import tempfile
 from glob import glob
@@ -159,15 +159,14 @@
         required=True,
     )
 
     return parser
 
 
 def main():
-
     parser = get_parser()
     try:
         args = parser.parse_args()
     except Exception:
         sys.exit(0)
 
     if args.command == "version" or args.version:
```

### Comparing `deid-0.3.21/deid/main/identifiers.py` & `deid-0.3.22/deid/main/identifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 
 import os
 import tempfile
 
 from deid.config import load_deid
 from deid.data import get_dataset
 from deid.dicom import get_files
 from deid.dicom.header import get_identifiers, replace_identifiers
 from deid.logger import bot
 
 
 def main(args, parser):
-
     # Global output folder
     output_folder = args.outfolder
     if output_folder is None:
         output_folder = tempfile.mkdtemp()
 
     # If a deid is given, check against format
     if args.deid is not None:
```

### Comparing `deid-0.3.21/deid/main/inspect.py` & `deid-0.3.22/deid/main/inspect.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import datetime
 import os
 
 from deid.config import load_deid
 from deid.data import get_dataset
```

### Comparing `deid-0.3.21/deid/utils/actions.py` & `deid-0.3.22/deid/utils/actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import re
 from datetime import datetime, timedelta
 
 import dateutil.parser
 
@@ -28,23 +28,21 @@
     if item is None:
         item = dict()
 
     # Does the user want a custom value?
     if re.search("(^var:)|(^func:)|(^deid_func:)", value):
         value_type, value_option = value.split(":", 1)
         if value_type.lower() == "var":
-
             # If selected variable not provided, skip
             if value_option not in item:
                 return None
             return item[value_option]
 
         # The user wants to use a deid provided function
         elif value_type.lower() == "deid_func":
-
             # There can be additional key=value pairs
             try:
                 value_option, extras = value_option.split(" ", 1)
             except Exception:
                 extras = ""
                 pass
 
@@ -57,15 +55,14 @@
             # The field is an entire dicom element object
             return funcs[value_option](
                 dicom=dicom, value=value, field=field, item=item, extras=extras
             )
 
         # The user is providing a specific function
         elif value_type.lower() == "func":
-
             if value_option not in item:
                 bot.warning("%s not found in item lookup." % (value_option))
                 return None
 
             # item is the lookup, value from the recipe, and field
             # The field is an entire dicom element object
             return item[value_option](dicom=dicom, value=value, field=field, item=item)
```

### Comparing `deid-0.3.21/deid/utils/fileio.py` & `deid-0.3.22/deid/utils/fileio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
 import fnmatch
 import json
 import os
 import tempfile
 from collections import OrderedDict
```

### Comparing `deid-0.3.21/deid/version.py` & `deid-0.3.22/deid/version.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
-__copyright__ = "Copyright 2016-2022, Vanessa Sochat"
+__copyright__ = "Copyright 2016-2023, Vanessa Sochat"
 __license__ = "MIT"
 
-__version__ = "0.3.21"
+__version__ = "0.3.22"
 AUTHOR = "Vanessa Sochat"
 AUTHOR_EMAIL = "vsoch@users.noreply.github.com"
 NAME = "deid"
 PACKAGE_URL = "https://github.com/pydicom/deid"
 KEYWORDS = "open source, python, anonymize, dicom"
 DESCRIPTION = "best effort deidentify dicom with python and pydicom"
 LICENSE = "LICENSE"
```

### Comparing `deid-0.3.21/deid.egg-info/PKG-INFO` & `deid-0.3.22/deid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: deid
-Version: 0.3.21
+Version: 0.3.22
 Summary: best effort deidentify dicom with python and pydicom
 Home-page: https://github.com/pydicom/deid
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 License: LICENSE
 Keywords: open source,python,anonymize,dicom
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -62,7 +63,9 @@
 ```bash
 docker build -t pydicom/deid .
 docker run pydicom/deid --help
 ```
 
 ## Issues
 If you have an issue, or want to request a feature, please do so on our [issues board](https://www.github.com/pydicom/deid/issues).
+
+
```

### Comparing `deid-0.3.21/deid.egg-info/SOURCES.txt` & `deid-0.3.22/deid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/README.md` & `deid-0.3.22/docs/README.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_config.yml` & `deid-0.3.22/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/contributing/code.md` & `deid-0.3.22/docs/_docs/contributing/code.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/contributing/docs.md` & `deid-0.3.22/docs/_docs/contributing/docs.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/development/image-format.md` & `deid-0.3.22/docs/_docs/development/image-format.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/development/index.md` & `deid-0.3.22/docs/_docs/development/index.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/examples/client.md` & `deid-0.3.22/docs/_docs/examples/client.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/examples/deid-dataset.md` & `deid-0.3.22/docs/_docs/examples/deid-dataset.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/examples/func-replace.md` & `deid-0.3.22/docs/_docs/examples/func-replace.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/examples/func-sequence-replace.md` & `deid-0.3.22/docs/_docs/examples/func-sequence-replace.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/examples/header-expanders.md` & `deid-0.3.22/docs/_docs/examples/header-expanders.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/examples/index.md` & `deid-0.3.22/docs/_docs/examples/index.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/examples/recipe.md` & `deid-0.3.22/docs/_docs/examples/recipe.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/getting-started/dicom-config.md` & `deid-0.3.22/docs/_docs/getting-started/dicom-config.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/getting-started/dicom-get.md` & `deid-0.3.22/docs/_docs/getting-started/dicom-get.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/getting-started/dicom-loading.md` & `deid-0.3.22/docs/_docs/getting-started/dicom-loading.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/getting-started/dicom-pixels.md` & `deid-0.3.22/docs/_docs/getting-started/dicom-pixels.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/getting-started/dicom-put.md` & `deid-0.3.22/docs/_docs/getting-started/dicom-put.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/getting-started/index.md` & `deid-0.3.22/docs/_docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/install/docker.md` & `deid-0.3.22/docs/_docs/install/docker.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/install/index.md` & `deid-0.3.22/docs/_docs/install/index.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/install/local.md` & `deid-0.3.22/docs/_docs/install/local.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/user-docs/client.md` & `deid-0.3.22/docs/_docs/user-docs/client.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/user-docs/index.md` & `deid-0.3.22/docs/_docs/user-docs/index.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/user-docs/recipe-filters.md` & `deid-0.3.22/docs/_docs/user-docs/recipe-filters.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,19 @@
 ##### How do I read a criteria?
 Each filter section criteria starts with `LABEL`. this is an identifier to
 report to the user given that the flag goes off. Each criteria then has the following format:
 
 ```
 <criteria> <field> <value>
 ```
-where "value" is optional, depending on the filter. For example:
+where "criteria" is a test such as "contains", "notcontains",
+"equals", "notequals", "missing", "present" or "empty";
+"field" is the single-word name of a DICOM tag (as known to pydicom),
+or the number as 8-digit hex format with 0x prefix;
+and "value" is optional, depending on the filter. For example:
 
 ```
 LABEL Burned In Annotation
 contains ImageType SAVE
 ```
 
 Reads "flag the image with a Burned In Annotation, which belongs to the blacklist filter,
```

### Comparing `deid-0.3.21/docs/_docs/user-docs/recipe-funcs.md` & `deid-0.3.22/docs/_docs/user-docs/recipe-funcs.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/user-docs/recipe-groups.md` & `deid-0.3.22/docs/_docs/user-docs/recipe-groups.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/user-docs/recipe-headers.md` & `deid-0.3.22/docs/_docs/user-docs/recipe-headers.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/user-docs/recipe-labels.md` & `deid-0.3.22/docs/_docs/user-docs/recipe-labels.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_docs/user-docs/tags.md` & `deid-0.3.22/docs/_docs/user-docs/tags.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_includes/head.html` & `deid-0.3.22/docs/_includes/head.html`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_includes/navigation.html` & `deid-0.3.22/docs/_includes/navigation.html`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_layouts/default.html` & `deid-0.3.22/docs/_layouts/default.html`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/_posts/2018-12-09-docs.md` & `deid-0.3.22/docs/_posts/2018-12-09-docs.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/Makefile` & `deid-0.3.22/docs/api_docs/Makefile`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/_static/theme.css` & `deid-0.3.22/docs/api_docs/_static/theme.css`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/assets/favicon.ico` & `deid-0.3.22/docs/api_docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/assets/logo.png` & `deid-0.3.22/docs/api_docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/conf.py` & `deid-0.3.22/docs/api_docs/conf.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/index.rst` & `deid-0.3.22/docs/api_docs/index.rst`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/source/deid.dicom.actions.rst` & `deid-0.3.22/docs/api_docs/source/deid.dicom.actions.rst`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/source/deid.dicom.pixels.rst` & `deid-0.3.22/docs/api_docs/source/deid.dicom.pixels.rst`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/source/deid.dicom.rst` & `deid-0.3.22/docs/api_docs/source/deid.dicom.rst`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/api_docs/source/deid.tests.rst` & `deid-0.3.22/docs/api_docs/source/deid.tests.rst`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/css/deid.css` & `deid-0.3.22/docs/assets/css/deid.css`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/fonts/helveticaneueout-webfont.woff` & `deid-0.3.22/docs/assets/fonts/helveticaneueout-webfont.woff`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/fonts/helveticaneueout-webfont.woff2` & `deid-0.3.22/docs/assets/fonts/helveticaneueout-webfont.woff2`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/img/apple-touch-icon.png` & `deid-0.3.22/docs/assets/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/img/favicon.ico` & `deid-0.3.22/docs/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/img/interaction-grid.png` & `deid-0.3.22/docs/assets/img/interaction-grid.png`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/img/logo.png` & `deid-0.3.22/docs/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/img/open-source-halloween-2021.png` & `deid-0.3.22/docs/assets/img/open-source-halloween-2021.png`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/img/siteicon.png` & `deid-0.3.22/docs/assets/img/siteicon.png`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/img/touch-icon.png` & `deid-0.3.22/docs/assets/img/touch-icon.png`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/js/lunr.min.js` & `deid-0.3.22/docs/assets/js/lunr.min.js`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/assets/js/search.js` & `deid-0.3.22/docs/assets/js/search.js`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/pages/changelog.html` & `deid-0.3.22/docs/pages/changelog.html`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/pages/index.md` & `deid-0.3.22/docs/pages/index.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/docs/pages/search.html` & `deid-0.3.22/docs/pages/search.html`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/dicom-extract/create-dicom-csv.py` & `deid-0.3.22/examples/dicom/dicom-extract/create-dicom-csv.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/header-manipulation/README.md` & `deid-0.3.22/examples/dicom/header-manipulation/README.md`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/header-manipulation/file-meta/example.py` & `deid-0.3.22/examples/dicom/header-manipulation/file-meta/example.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/header-manipulation/func-replacement.py` & `deid-0.3.22/examples/dicom/header-manipulation/func-replacement.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/header-manipulation/func-sequence-replace/MR.dcm` & `deid-0.3.22/examples/dicom/header-manipulation/func-sequence-replace/MR.dcm`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/header-manipulation/func-sequence-replace/cleaned.dcm` & `deid-0.3.22/examples/dicom/header-manipulation/func-sequence-replace/cleaned.dcm`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/header-manipulation/func-sequence-replace/example.py` & `deid-0.3.22/examples/dicom/header-manipulation/func-sequence-replace/example.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/pixels/run-cleaner-client.py` & `deid-0.3.22/examples/dicom/pixels/run-cleaner-client.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/pixels/run-inspect-pixels.py` & `deid-0.3.22/examples/dicom/pixels/run-inspect-pixels.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/examples/dicom/recipe/deid-dicom-example.py` & `deid-0.3.22/examples/dicom/recipe/deid-dicom-example.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/setup.cfg` & `deid-0.3.22/setup.cfg`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/setup.py` & `deid-0.3.22/setup.py`

 * *Files identical despite different names*

### Comparing `deid-0.3.21/test/test.py` & `deid-0.3.22/test/test.py`

 * *Files identical despite different names*

