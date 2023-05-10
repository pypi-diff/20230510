# Comparing `tmp/memcnn-1.5.1.tar.gz` & `tmp/memcnn-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memcnn-1.5.1.tar", last modified: Wed Aug 11 15:16:07 2021, max compression
+gzip compressed data, was "dist/memcnn-1.5.2.tar", last modified: Wed May 10 09:29:48 2023, max compression
```

## Comparing `memcnn-1.5.1.tar` & `memcnn-1.5.2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      219 2021-08-11 15:14:03.000000 memcnn-1.5.1/AUTHORS.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3589 2021-08-11 15:14:03.000000 memcnn-1.5.1/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4531 2021-08-11 15:14:03.000000 memcnn-1.5.1/HISTORY.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2021-08-11 15:14:03.000000 memcnn-1.5.1/LICENSE.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      417 2021-08-11 15:14:03.000000 memcnn-1.5.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7457 2021-08-11 15:16:07.000000 memcnn-1.5.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14816 2021-08-11 15:14:03.000000 memcnn-1.5.1/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2021-08-11 15:14:03.000000 memcnn-1.5.1/devRequirements.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/docs/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/Makefile
--rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/authors.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5795 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/conf.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/contributing.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/history.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      303 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/index.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4267 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/installation.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      768 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/make.bat
--rw-r--r--   0 circleci  (3434) circleci  (3434)      447 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/modules.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/readme.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2679 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/usage.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2021-08-11 15:14:03.000000 memcnn-1.5.1/docs/usage_experiments.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2021-08-11 15:14:03.000000 memcnn-1.5.1/docsRequirements.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      637 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/config/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      562 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/config/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/config/config.json.example
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2224 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/config/experiments.json
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/config/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/config/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2140 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/config/tests/test_config.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/data/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/data/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2289 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/data/cifar.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1177 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/data/sampling.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/data/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/data/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2194 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/data/tests/test_cifar.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/data/tests/test_sampling.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/experiment/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/experiment/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2450 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/experiment/factory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2749 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/experiment/manager.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/experiment/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/experiment/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1275 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/experiment/tests/test_factory.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2455 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/experiment/tests/test_manager.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17560 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/additive.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20317 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/affine.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9769 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/resnet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    20513 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/revop.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/models/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3118 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_amp.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5488 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_couplings.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3263 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_is_invertible_module.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2550 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_memory_saving.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3273 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      835 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_multi.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      571 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_resnet.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16640 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_revop.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1081 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/models/tests/test_split_dim.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4735 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/train.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/trainers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/trainers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5330 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/trainers/classification.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/trainers/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/trainers/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2310 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/trainers/tests/test_classification.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3521 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/trainers/tests/test_train.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/utils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/utils/log.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      812 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/utils/loss.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1023 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/utils/stats.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn/utils/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/utils/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      993 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/utils/tests/test_log.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/utils/tests/test_loss.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      897 2021-08-11 15:14:03.000000 memcnn-1.5.1/memcnn/utils/tests/test_stats.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7457 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1957 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2021-08-11 15:16:07.000000 memcnn-1.5.1/memcnn.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2021-08-11 15:14:03.000000 memcnn-1.5.1/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      477 2021-08-11 15:16:07.000000 memcnn-1.5.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2009 2021-08-11 15:14:03.000000 memcnn-1.5.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.725286 memcnn-1.5.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      219 2023-05-10 09:24:55.000000 memcnn-1.5.2/AUTHORS.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3589 2023-05-10 09:24:55.000000 memcnn-1.5.2/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4738 2023-05-10 09:24:55.000000 memcnn-1.5.2/HISTORY.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1078 2023-05-10 09:24:55.000000 memcnn-1.5.2/LICENSE.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      417 2023-05-10 09:24:55.000000 memcnn-1.5.2/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8608 2023-05-10 09:29:48.725286 memcnn-1.5.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14816 2023-05-10 09:24:55.000000 memcnn-1.5.2/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      112 2023-05-10 09:24:55.000000 memcnn-1.5.2/devRequirements.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.717286 memcnn-1.5.2/docs/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/Makefile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/authors.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5795 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/conf.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/contributing.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       28 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/history.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      303 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/index.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4267 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/installation.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      768 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/make.bat
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      447 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/modules.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       27 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/readme.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2679 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/usage.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      684 2023-05-10 09:24:55.000000 memcnn-1.5.2/docs/usage_experiments.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       88 2023-05-10 09:24:55.000000 memcnn-1.5.2/docsRequirements.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.717286 memcnn-1.5.2/memcnn/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      637 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.717286 memcnn-1.5.2/memcnn/config/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      562 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/config/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       78 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/config/config.json.example
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2224 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/config/experiments.json
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.717286 memcnn-1.5.2/memcnn/config/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/config/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2140 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/config/tests/test_config.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.717286 memcnn-1.5.2/memcnn/data/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/data/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2538 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/data/cifar.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1177 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/data/sampling.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.717286 memcnn-1.5.2/memcnn/data/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/data/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2194 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/data/tests/test_cifar.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/data/tests/test_sampling.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.721286 memcnn-1.5.2/memcnn/experiment/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/experiment/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2450 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/experiment/factory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2749 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/experiment/manager.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.721286 memcnn-1.5.2/memcnn/experiment/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/experiment/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1275 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/experiment/tests/test_factory.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2455 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/experiment/tests/test_manager.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.721286 memcnn-1.5.2/memcnn/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17560 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/additive.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20317 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/affine.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9769 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/resnet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    20513 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/revop.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.725286 memcnn-1.5.2/memcnn/models/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3118 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_amp.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5488 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_couplings.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3263 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_is_invertible_module.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2550 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_memory_saving.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3273 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      835 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_multi.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      571 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_resnet.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16640 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_revop.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1081 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/models/tests/test_split_dim.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4735 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/train.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.725286 memcnn-1.5.2/memcnn/trainers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/trainers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5330 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/trainers/classification.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.725286 memcnn-1.5.2/memcnn/trainers/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/trainers/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2310 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/trainers/tests/test_classification.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3521 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/trainers/tests/test_train.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.725286 memcnn-1.5.2/memcnn/utils/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/utils/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1380 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/utils/log.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      812 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/utils/loss.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1023 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/utils/stats.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.725286 memcnn-1.5.2/memcnn/utils/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/utils/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      993 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/utils/tests/test_log.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      763 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/utils/tests/test_loss.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      897 2023-05-10 09:24:55.000000 memcnn-1.5.2/memcnn/utils/tests/test_stats.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-05-10 09:29:48.717286 memcnn-1.5.2/memcnn.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8608 2023-05-10 09:29:48.000000 memcnn-1.5.2/memcnn.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1957 2023-05-10 09:29:48.000000 memcnn-1.5.2/memcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-05-10 09:29:48.000000 memcnn-1.5.2/memcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2023-05-10 09:29:48.000000 memcnn-1.5.2/memcnn.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-05-10 09:29:48.000000 memcnn-1.5.2/memcnn.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       55 2023-05-10 09:24:55.000000 memcnn-1.5.2/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      477 2023-05-10 09:29:48.725286 memcnn-1.5.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2009 2023-05-10 09:24:55.000000 memcnn-1.5.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `memcnn-1.5.1/CONTRIBUTING.rst` & `memcnn-1.5.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/HISTORY.rst` & `memcnn-1.5.2/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+1.5.2 (2023-05-10)
+------------------
+* Fixed issue with CIFAR data loaders not being able to be pickled because of local Lambda operations
+* Fixed CI issues, disabled PyTorch v1.0, v1.1, and latest checks
+
 1.5.1 (2021-08-07)
 ------------------
 * Added support for 2-dimensional inputs for AffineAdapterSigmoid
 * Fixed CI issues
 
 1.5.0 (2020-11-24)
 ------------------
```

### Comparing `memcnn-1.5.1/LICENSE.txt` & `memcnn-1.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/PKG-INFO` & `memcnn-1.5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,176 +1,172 @@
 Metadata-Version: 2.1
 Name: memcnn
-Version: 1.5.1
+Version: 1.5.2
 Summary: A PyTorch framework for developing memory efficient deep invertible networks.
 Home-page: http://pypi.python.org/pypi/memcnn/
 Author: S.C. van de Leemput
 Author-email: silvandeleemput@gmail.com
 License: LICENSE.txt
+Description: ======
+        MemCNN
+        ======
+        
+        .. image:: https://img.shields.io/circleci/build/github/silvandeleemput/memcnn/master.svg        
+                :alt: CircleCI - Status master branch
+                :target: https://circleci.com/gh/silvandeleemput/memcnn/tree/master
+        
+        .. image:: https://img.shields.io/docker/cloud/build/silvandeleemput/memcnn.svg
+                :alt: Docker - Status
+                :target: https://hub.docker.com/r/silvandeleemput/memcnn
+        
+        .. image:: https://readthedocs.org/projects/memcnn/badge/?version=latest        
+                :alt: Documentation - Status master branch
+                :target: https://memcnn.readthedocs.io/en/latest/?badge=latest
+        
+        .. image:: https://img.shields.io/codacy/grade/95de32e0d7c54d038611da47e9f0948b/master.svg
+                :alt: Codacy - Branch grade
+                :target: https://app.codacy.com/project/silvandeleemput/memcnn/dashboardgit
+        
+        .. image:: https://img.shields.io/codecov/c/gh/silvandeleemput/memcnn/master.svg   
+                :alt: Codecov - Status master branch
+                :target: https://codecov.io/gh/silvandeleemput/memcnn
+        
+        .. image:: https://img.shields.io/pypi/v/memcnn.svg
+                :alt: PyPI - Latest release
+                :target: https://pypi.python.org/pypi/memcnn
+        
+        .. image:: https://img.shields.io/conda/vn/silvandeleemput/memcnn?label=anaconda
+                :alt: Conda - Latest release
+                :target: https://anaconda.org/silvandeleemput/memcnn
+        
+        .. image:: https://img.shields.io/pypi/implementation/memcnn.svg        
+                :alt: PyPI - Implementation
+                :target: https://pypi.python.org/pypi/memcnn
+        
+        .. image:: https://img.shields.io/pypi/pyversions/memcnn.svg        
+                :alt: PyPI - Python version
+                :target: https://pypi.python.org/pypi/memcnn
+        
+        .. image:: https://img.shields.io/github/license/silvandeleemput/memcnn.svg        
+                :alt: GitHub - Repository license
+                :target: https://github.com/silvandeleemput/memcnn/blob/master/LICENSE.txt
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.01576/status.svg
+                :alt: JOSS - DOI
+                :target: https://doi.org/10.21105/joss.01576
+        
+        A `PyTorch <http://pytorch.org/>`__ framework for developing memory-efficient invertible neural networks.
+        
+        * Free software: `MIT license <https://github.com/silvandeleemput/memcnn/blob/master/LICENSE.txt>`__ (please cite our work if you use it)
+        * Documentation: https://memcnn.readthedocs.io.
+        * Installation: https://memcnn.readthedocs.io/en/latest/installation.html
+        
+        Features
+        --------
+        
+        * Enable memory savings during training by wrapping arbitrary invertible PyTorch functions with the `InvertibleModuleWrapper` class.
+        * Simple toggling of memory saving by setting the `keep_input` property of the `InvertibleModuleWrapper`.
+        * Turn arbitrary non-linear PyTorch functions into invertible versions using the `AdditiveCoupling` or the `AffineCoupling` classes.
+        * Training and evaluation code for reproducing RevNet experiments using MemCNN.
+        * CI tests for Python v3.7 and torch v1.0, v1.1, v1.4 and v1.7 with good code coverage.
+        
+        Examples
+        --------
+        
+        Creating an AdditiveCoupling with memory savings
+        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        
+        .. code:: python
+        
+            import torch
+            import torch.nn as nn
+            import memcnn
+        
+        
+            # define a new torch Module with a sequence of operations: Relu o BatchNorm2d o Conv2d
+            class ExampleOperation(nn.Module):
+                def __init__(self, channels):
+                    super(ExampleOperation, self).__init__()
+                    self.seq = nn.Sequential(
+                                                nn.Conv2d(in_channels=channels, out_channels=channels,
+                                                          kernel_size=(3, 3), padding=1),
+                                                nn.BatchNorm2d(num_features=channels),
+                                                nn.ReLU(inplace=True)
+                                            )
+        
+                def forward(self, x):
+                    return self.seq(x)
+        
+        
+            # generate some random input data (batch_size, num_channels, y_elements, x_elements)
+            X = torch.rand(2, 10, 8, 8)
+        
+            # application of the operation(s) the normal way
+            model_normal = ExampleOperation(channels=10)
+            model_normal.eval()
+        
+            Y = model_normal(X)
+        
+            # turn the ExampleOperation invertible using an additive coupling
+            invertible_module = memcnn.AdditiveCoupling(
+                Fm=ExampleOperation(channels=10 // 2),
+                Gm=ExampleOperation(channels=10 // 2)
+            )
+        
+            # test that it is actually a valid invertible module (has a valid inverse method)
+            assert memcnn.is_invertible_module(invertible_module, test_input_shape=X.shape)
+        
+            # wrap our invertible_module using the InvertibleModuleWrapper and benefit from memory savings during training
+            invertible_module_wrapper = memcnn.InvertibleModuleWrapper(fn=invertible_module, keep_input=True, keep_input_inverse=True)
+        
+            # by default the module is set to training, the following sets this to evaluation
+            # note that this is required to pass input tensors to the model with requires_grad=False (inference only)
+            invertible_module_wrapper.eval()
+        
+            # test that the wrapped module is also a valid invertible module
+            assert memcnn.is_invertible_module(invertible_module_wrapper, test_input_shape=X.shape)
+        
+            # compute the forward pass using the wrapper
+            Y2 = invertible_module_wrapper.forward(X)
+        
+            # the input (X) can be approximated (X2) by applying the inverse method of the wrapper on Y2
+            X2 = invertible_module_wrapper.inverse(Y2)
+        
+            # test that the input and approximation are similar
+            assert torch.allclose(X, X2, atol=1e-06)
+        
+        Run PyTorch Experiments
+        -----------------------
+        
+        After installing MemCNN run:
+        
+        .. code:: bash
+        
+            python -m memcnn.train [MODEL] [DATASET] [--fresh] [--no-cuda]
+        
+        * Available values for ``DATASET`` are ``cifar10`` and ``cifar100``.
+        * Available values for ``MODEL`` are ``resnet32``, ``resnet110``, ``resnet164``, ``revnet38``, ``revnet110``, ``revnet164``
+        * Use the ``--fresh`` flag to remove earlier experiment results.
+        * Use the ``--no-cuda`` flag to train on the CPU rather than the GPU through CUDA.
+        
+        Datasets are automatically downloaded if they are not available.
+        
+        When using Python 3.* replace the ``python`` directive with the appropriate Python 3 directive. For example when using the MemCNN docker image use ``python3.6``.
+        
+        When MemCNN was installed using `pip` or from sources you might need to setup a configuration file before running this command.
+        Read the corresponding section about how to do this here: https://memcnn.readthedocs.io/en/latest/installation.html
+        
+        
 Keywords: memcnn invertible PyTorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-
-======
-MemCNN
-======
-
-.. image:: https://img.shields.io/circleci/build/github/silvandeleemput/memcnn/master.svg        
-        :alt: CircleCI - Status master branch
-        :target: https://circleci.com/gh/silvandeleemput/memcnn/tree/master
-
-.. image:: https://img.shields.io/docker/cloud/build/silvandeleemput/memcnn.svg
-        :alt: Docker - Status
-        :target: https://hub.docker.com/r/silvandeleemput/memcnn
-
-.. image:: https://readthedocs.org/projects/memcnn/badge/?version=latest        
-        :alt: Documentation - Status master branch
-        :target: https://memcnn.readthedocs.io/en/latest/?badge=latest
-
-.. image:: https://img.shields.io/codacy/grade/95de32e0d7c54d038611da47e9f0948b/master.svg
-        :alt: Codacy - Branch grade
-        :target: https://app.codacy.com/project/silvandeleemput/memcnn/dashboardgit
-
-.. image:: https://img.shields.io/codecov/c/gh/silvandeleemput/memcnn/master.svg   
-        :alt: Codecov - Status master branch
-        :target: https://codecov.io/gh/silvandeleemput/memcnn
-
-.. image:: https://img.shields.io/pypi/v/memcnn.svg
-        :alt: PyPI - Latest release
-        :target: https://pypi.python.org/pypi/memcnn
-
-.. image:: https://img.shields.io/conda/vn/silvandeleemput/memcnn?label=anaconda
-        :alt: Conda - Latest release
-        :target: https://anaconda.org/silvandeleemput/memcnn
-
-.. image:: https://img.shields.io/pypi/implementation/memcnn.svg        
-        :alt: PyPI - Implementation
-        :target: https://pypi.python.org/pypi/memcnn
-
-.. image:: https://img.shields.io/pypi/pyversions/memcnn.svg        
-        :alt: PyPI - Python version
-        :target: https://pypi.python.org/pypi/memcnn
-
-.. image:: https://img.shields.io/github/license/silvandeleemput/memcnn.svg        
-        :alt: GitHub - Repository license
-        :target: https://github.com/silvandeleemput/memcnn/blob/master/LICENSE.txt
-
-.. image:: http://joss.theoj.org/papers/10.21105/joss.01576/status.svg
-        :alt: JOSS - DOI
-        :target: https://doi.org/10.21105/joss.01576
-
-A `PyTorch <http://pytorch.org/>`__ framework for developing memory-efficient invertible neural networks.
-
-* Free software: `MIT license <https://github.com/silvandeleemput/memcnn/blob/master/LICENSE.txt>`__ (please cite our work if you use it)
-* Documentation: https://memcnn.readthedocs.io.
-* Installation: https://memcnn.readthedocs.io/en/latest/installation.html
-
-Features
---------
-
-* Enable memory savings during training by wrapping arbitrary invertible PyTorch functions with the `InvertibleModuleWrapper` class.
-* Simple toggling of memory saving by setting the `keep_input` property of the `InvertibleModuleWrapper`.
-* Turn arbitrary non-linear PyTorch functions into invertible versions using the `AdditiveCoupling` or the `AffineCoupling` classes.
-* Training and evaluation code for reproducing RevNet experiments using MemCNN.
-* CI tests for Python v3.7 and torch v1.0, v1.1, v1.4 and v1.7 with good code coverage.
-
-Examples
---------
-
-Creating an AdditiveCoupling with memory savings
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code:: python
-
-    import torch
-    import torch.nn as nn
-    import memcnn
-
-
-    # define a new torch Module with a sequence of operations: Relu o BatchNorm2d o Conv2d
-    class ExampleOperation(nn.Module):
-        def __init__(self, channels):
-            super(ExampleOperation, self).__init__()
-            self.seq = nn.Sequential(
-                                        nn.Conv2d(in_channels=channels, out_channels=channels,
-                                                  kernel_size=(3, 3), padding=1),
-                                        nn.BatchNorm2d(num_features=channels),
-                                        nn.ReLU(inplace=True)
-                                    )
-
-        def forward(self, x):
-            return self.seq(x)
-
-
-    # generate some random input data (batch_size, num_channels, y_elements, x_elements)
-    X = torch.rand(2, 10, 8, 8)
-
-    # application of the operation(s) the normal way
-    model_normal = ExampleOperation(channels=10)
-    model_normal.eval()
-
-    Y = model_normal(X)
-
-    # turn the ExampleOperation invertible using an additive coupling
-    invertible_module = memcnn.AdditiveCoupling(
-        Fm=ExampleOperation(channels=10 // 2),
-        Gm=ExampleOperation(channels=10 // 2)
-    )
-
-    # test that it is actually a valid invertible module (has a valid inverse method)
-    assert memcnn.is_invertible_module(invertible_module, test_input_shape=X.shape)
-
-    # wrap our invertible_module using the InvertibleModuleWrapper and benefit from memory savings during training
-    invertible_module_wrapper = memcnn.InvertibleModuleWrapper(fn=invertible_module, keep_input=True, keep_input_inverse=True)
-
-    # by default the module is set to training, the following sets this to evaluation
-    # note that this is required to pass input tensors to the model with requires_grad=False (inference only)
-    invertible_module_wrapper.eval()
-
-    # test that the wrapped module is also a valid invertible module
-    assert memcnn.is_invertible_module(invertible_module_wrapper, test_input_shape=X.shape)
-
-    # compute the forward pass using the wrapper
-    Y2 = invertible_module_wrapper.forward(X)
-
-    # the input (X) can be approximated (X2) by applying the inverse method of the wrapper on Y2
-    X2 = invertible_module_wrapper.inverse(Y2)
-
-    # test that the input and approximation are similar
-    assert torch.allclose(X, X2, atol=1e-06)
-
-Run PyTorch Experiments
------------------------
-
-After installing MemCNN run:
-
-.. code:: bash
-
-    python -m memcnn.train [MODEL] [DATASET] [--fresh] [--no-cuda]
-
-* Available values for ``DATASET`` are ``cifar10`` and ``cifar100``.
-* Available values for ``MODEL`` are ``resnet32``, ``resnet110``, ``resnet164``, ``revnet38``, ``revnet110``, ``revnet164``
-* Use the ``--fresh`` flag to remove earlier experiment results.
-* Use the ``--no-cuda`` flag to train on the CPU rather than the GPU through CUDA.
-
-Datasets are automatically downloaded if they are not available.
-
-When using Python 3.* replace the ``python`` directive with the appropriate Python 3 directive. For example when using the MemCNN docker image use ``python3.6``.
-
-When MemCNN was installed using `pip` or from sources you might need to setup a configuration file before running this command.
-Read the corresponding section about how to do this here: https://memcnn.readthedocs.io/en/latest/installation.html
-
-
-
```

### Comparing `memcnn-1.5.1/README.rst` & `memcnn-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/docs/Makefile` & `memcnn-1.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/docs/conf.py` & `memcnn-1.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/docs/installation.rst` & `memcnn-1.5.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/docs/make.bat` & `memcnn-1.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/docs/usage.rst` & `memcnn-1.5.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/docs/usage_experiments.rst` & `memcnn-1.5.2/docs/usage_experiments.rst`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/__init__.py` & `memcnn-1.5.2/memcnn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for MemCNN."""
 
 __author__ = """Sil van de Leemput"""
 __email__ = 'silvandeleemput@gmail.com'
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 
 
 from memcnn.models.revop import ReversibleBlock, InvertibleModuleWrapper, create_coupling, is_invertible_module
 from memcnn.models.additive import AdditiveCoupling
 from memcnn.models.affine import AffineCoupling, AffineAdapterNaive, AffineAdapterSigmoid
 
 __all__ = [
```

### Comparing `memcnn-1.5.1/memcnn/config/__init__.py` & `memcnn-1.5.2/memcnn/config/__init__.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/config/experiments.json` & `memcnn-1.5.2/memcnn/config/experiments.json`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/config/tests/test_config.py` & `memcnn-1.5.2/memcnn/config/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/data/sampling.py` & `memcnn-1.5.2/memcnn/data/sampling.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/data/tests/test_cifar.py` & `memcnn-1.5.2/memcnn/data/tests/test_cifar.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/data/tests/test_sampling.py` & `memcnn-1.5.2/memcnn/data/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/experiment/factory.py` & `memcnn-1.5.2/memcnn/experiment/factory.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/experiment/manager.py` & `memcnn-1.5.2/memcnn/experiment/manager.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/experiment/tests/test_factory.py` & `memcnn-1.5.2/memcnn/experiment/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/experiment/tests/test_manager.py` & `memcnn-1.5.2/memcnn/experiment/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/additive.py` & `memcnn-1.5.2/memcnn/models/additive.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/affine.py` & `memcnn-1.5.2/memcnn/models/affine.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/resnet.py` & `memcnn-1.5.2/memcnn/models/resnet.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/revop.py` & `memcnn-1.5.2/memcnn/models/revop.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_amp.py` & `memcnn-1.5.2/memcnn/models/tests/test_amp.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_couplings.py` & `memcnn-1.5.2/memcnn/models/tests/test_couplings.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_is_invertible_module.py` & `memcnn-1.5.2/memcnn/models/tests/test_is_invertible_module.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_memory_saving.py` & `memcnn-1.5.2/memcnn/models/tests/test_memory_saving.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_models.py` & `memcnn-1.5.2/memcnn/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_multi.py` & `memcnn-1.5.2/memcnn/models/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_resnet.py` & `memcnn-1.5.2/memcnn/models/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_revop.py` & `memcnn-1.5.2/memcnn/models/tests/test_revop.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/models/tests/test_split_dim.py` & `memcnn-1.5.2/memcnn/models/tests/test_split_dim.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/train.py` & `memcnn-1.5.2/memcnn/train.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/trainers/classification.py` & `memcnn-1.5.2/memcnn/trainers/classification.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/trainers/tests/test_classification.py` & `memcnn-1.5.2/memcnn/trainers/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/trainers/tests/test_train.py` & `memcnn-1.5.2/memcnn/trainers/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/utils/log.py` & `memcnn-1.5.2/memcnn/utils/log.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/utils/loss.py` & `memcnn-1.5.2/memcnn/utils/loss.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/utils/stats.py` & `memcnn-1.5.2/memcnn/utils/stats.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/utils/tests/test_log.py` & `memcnn-1.5.2/memcnn/utils/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/utils/tests/test_loss.py` & `memcnn-1.5.2/memcnn/utils/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn/utils/tests/test_stats.py` & `memcnn-1.5.2/memcnn/utils/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/memcnn.egg-info/PKG-INFO` & `memcnn-1.5.2/memcnn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,176 +1,172 @@
 Metadata-Version: 2.1
 Name: memcnn
-Version: 1.5.1
+Version: 1.5.2
 Summary: A PyTorch framework for developing memory efficient deep invertible networks.
 Home-page: http://pypi.python.org/pypi/memcnn/
 Author: S.C. van de Leemput
 Author-email: silvandeleemput@gmail.com
 License: LICENSE.txt
+Description: ======
+        MemCNN
+        ======
+        
+        .. image:: https://img.shields.io/circleci/build/github/silvandeleemput/memcnn/master.svg        
+                :alt: CircleCI - Status master branch
+                :target: https://circleci.com/gh/silvandeleemput/memcnn/tree/master
+        
+        .. image:: https://img.shields.io/docker/cloud/build/silvandeleemput/memcnn.svg
+                :alt: Docker - Status
+                :target: https://hub.docker.com/r/silvandeleemput/memcnn
+        
+        .. image:: https://readthedocs.org/projects/memcnn/badge/?version=latest        
+                :alt: Documentation - Status master branch
+                :target: https://memcnn.readthedocs.io/en/latest/?badge=latest
+        
+        .. image:: https://img.shields.io/codacy/grade/95de32e0d7c54d038611da47e9f0948b/master.svg
+                :alt: Codacy - Branch grade
+                :target: https://app.codacy.com/project/silvandeleemput/memcnn/dashboardgit
+        
+        .. image:: https://img.shields.io/codecov/c/gh/silvandeleemput/memcnn/master.svg   
+                :alt: Codecov - Status master branch
+                :target: https://codecov.io/gh/silvandeleemput/memcnn
+        
+        .. image:: https://img.shields.io/pypi/v/memcnn.svg
+                :alt: PyPI - Latest release
+                :target: https://pypi.python.org/pypi/memcnn
+        
+        .. image:: https://img.shields.io/conda/vn/silvandeleemput/memcnn?label=anaconda
+                :alt: Conda - Latest release
+                :target: https://anaconda.org/silvandeleemput/memcnn
+        
+        .. image:: https://img.shields.io/pypi/implementation/memcnn.svg        
+                :alt: PyPI - Implementation
+                :target: https://pypi.python.org/pypi/memcnn
+        
+        .. image:: https://img.shields.io/pypi/pyversions/memcnn.svg        
+                :alt: PyPI - Python version
+                :target: https://pypi.python.org/pypi/memcnn
+        
+        .. image:: https://img.shields.io/github/license/silvandeleemput/memcnn.svg        
+                :alt: GitHub - Repository license
+                :target: https://github.com/silvandeleemput/memcnn/blob/master/LICENSE.txt
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.01576/status.svg
+                :alt: JOSS - DOI
+                :target: https://doi.org/10.21105/joss.01576
+        
+        A `PyTorch <http://pytorch.org/>`__ framework for developing memory-efficient invertible neural networks.
+        
+        * Free software: `MIT license <https://github.com/silvandeleemput/memcnn/blob/master/LICENSE.txt>`__ (please cite our work if you use it)
+        * Documentation: https://memcnn.readthedocs.io.
+        * Installation: https://memcnn.readthedocs.io/en/latest/installation.html
+        
+        Features
+        --------
+        
+        * Enable memory savings during training by wrapping arbitrary invertible PyTorch functions with the `InvertibleModuleWrapper` class.
+        * Simple toggling of memory saving by setting the `keep_input` property of the `InvertibleModuleWrapper`.
+        * Turn arbitrary non-linear PyTorch functions into invertible versions using the `AdditiveCoupling` or the `AffineCoupling` classes.
+        * Training and evaluation code for reproducing RevNet experiments using MemCNN.
+        * CI tests for Python v3.7 and torch v1.0, v1.1, v1.4 and v1.7 with good code coverage.
+        
+        Examples
+        --------
+        
+        Creating an AdditiveCoupling with memory savings
+        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+        
+        .. code:: python
+        
+            import torch
+            import torch.nn as nn
+            import memcnn
+        
+        
+            # define a new torch Module with a sequence of operations: Relu o BatchNorm2d o Conv2d
+            class ExampleOperation(nn.Module):
+                def __init__(self, channels):
+                    super(ExampleOperation, self).__init__()
+                    self.seq = nn.Sequential(
+                                                nn.Conv2d(in_channels=channels, out_channels=channels,
+                                                          kernel_size=(3, 3), padding=1),
+                                                nn.BatchNorm2d(num_features=channels),
+                                                nn.ReLU(inplace=True)
+                                            )
+        
+                def forward(self, x):
+                    return self.seq(x)
+        
+        
+            # generate some random input data (batch_size, num_channels, y_elements, x_elements)
+            X = torch.rand(2, 10, 8, 8)
+        
+            # application of the operation(s) the normal way
+            model_normal = ExampleOperation(channels=10)
+            model_normal.eval()
+        
+            Y = model_normal(X)
+        
+            # turn the ExampleOperation invertible using an additive coupling
+            invertible_module = memcnn.AdditiveCoupling(
+                Fm=ExampleOperation(channels=10 // 2),
+                Gm=ExampleOperation(channels=10 // 2)
+            )
+        
+            # test that it is actually a valid invertible module (has a valid inverse method)
+            assert memcnn.is_invertible_module(invertible_module, test_input_shape=X.shape)
+        
+            # wrap our invertible_module using the InvertibleModuleWrapper and benefit from memory savings during training
+            invertible_module_wrapper = memcnn.InvertibleModuleWrapper(fn=invertible_module, keep_input=True, keep_input_inverse=True)
+        
+            # by default the module is set to training, the following sets this to evaluation
+            # note that this is required to pass input tensors to the model with requires_grad=False (inference only)
+            invertible_module_wrapper.eval()
+        
+            # test that the wrapped module is also a valid invertible module
+            assert memcnn.is_invertible_module(invertible_module_wrapper, test_input_shape=X.shape)
+        
+            # compute the forward pass using the wrapper
+            Y2 = invertible_module_wrapper.forward(X)
+        
+            # the input (X) can be approximated (X2) by applying the inverse method of the wrapper on Y2
+            X2 = invertible_module_wrapper.inverse(Y2)
+        
+            # test that the input and approximation are similar
+            assert torch.allclose(X, X2, atol=1e-06)
+        
+        Run PyTorch Experiments
+        -----------------------
+        
+        After installing MemCNN run:
+        
+        .. code:: bash
+        
+            python -m memcnn.train [MODEL] [DATASET] [--fresh] [--no-cuda]
+        
+        * Available values for ``DATASET`` are ``cifar10`` and ``cifar100``.
+        * Available values for ``MODEL`` are ``resnet32``, ``resnet110``, ``resnet164``, ``revnet38``, ``revnet110``, ``revnet164``
+        * Use the ``--fresh`` flag to remove earlier experiment results.
+        * Use the ``--no-cuda`` flag to train on the CPU rather than the GPU through CUDA.
+        
+        Datasets are automatically downloaded if they are not available.
+        
+        When using Python 3.* replace the ``python`` directive with the appropriate Python 3 directive. For example when using the MemCNN docker image use ``python3.6``.
+        
+        When MemCNN was installed using `pip` or from sources you might need to setup a configuration file before running this command.
+        Read the corresponding section about how to do this here: https://memcnn.readthedocs.io/en/latest/installation.html
+        
+        
 Keywords: memcnn invertible PyTorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-License-File: AUTHORS.rst
-
-======
-MemCNN
-======
-
-.. image:: https://img.shields.io/circleci/build/github/silvandeleemput/memcnn/master.svg        
-        :alt: CircleCI - Status master branch
-        :target: https://circleci.com/gh/silvandeleemput/memcnn/tree/master
-
-.. image:: https://img.shields.io/docker/cloud/build/silvandeleemput/memcnn.svg
-        :alt: Docker - Status
-        :target: https://hub.docker.com/r/silvandeleemput/memcnn
-
-.. image:: https://readthedocs.org/projects/memcnn/badge/?version=latest        
-        :alt: Documentation - Status master branch
-        :target: https://memcnn.readthedocs.io/en/latest/?badge=latest
-
-.. image:: https://img.shields.io/codacy/grade/95de32e0d7c54d038611da47e9f0948b/master.svg
-        :alt: Codacy - Branch grade
-        :target: https://app.codacy.com/project/silvandeleemput/memcnn/dashboardgit
-
-.. image:: https://img.shields.io/codecov/c/gh/silvandeleemput/memcnn/master.svg   
-        :alt: Codecov - Status master branch
-        :target: https://codecov.io/gh/silvandeleemput/memcnn
-
-.. image:: https://img.shields.io/pypi/v/memcnn.svg
-        :alt: PyPI - Latest release
-        :target: https://pypi.python.org/pypi/memcnn
-
-.. image:: https://img.shields.io/conda/vn/silvandeleemput/memcnn?label=anaconda
-        :alt: Conda - Latest release
-        :target: https://anaconda.org/silvandeleemput/memcnn
-
-.. image:: https://img.shields.io/pypi/implementation/memcnn.svg        
-        :alt: PyPI - Implementation
-        :target: https://pypi.python.org/pypi/memcnn
-
-.. image:: https://img.shields.io/pypi/pyversions/memcnn.svg        
-        :alt: PyPI - Python version
-        :target: https://pypi.python.org/pypi/memcnn
-
-.. image:: https://img.shields.io/github/license/silvandeleemput/memcnn.svg        
-        :alt: GitHub - Repository license
-        :target: https://github.com/silvandeleemput/memcnn/blob/master/LICENSE.txt
-
-.. image:: http://joss.theoj.org/papers/10.21105/joss.01576/status.svg
-        :alt: JOSS - DOI
-        :target: https://doi.org/10.21105/joss.01576
-
-A `PyTorch <http://pytorch.org/>`__ framework for developing memory-efficient invertible neural networks.
-
-* Free software: `MIT license <https://github.com/silvandeleemput/memcnn/blob/master/LICENSE.txt>`__ (please cite our work if you use it)
-* Documentation: https://memcnn.readthedocs.io.
-* Installation: https://memcnn.readthedocs.io/en/latest/installation.html
-
-Features
---------
-
-* Enable memory savings during training by wrapping arbitrary invertible PyTorch functions with the `InvertibleModuleWrapper` class.
-* Simple toggling of memory saving by setting the `keep_input` property of the `InvertibleModuleWrapper`.
-* Turn arbitrary non-linear PyTorch functions into invertible versions using the `AdditiveCoupling` or the `AffineCoupling` classes.
-* Training and evaluation code for reproducing RevNet experiments using MemCNN.
-* CI tests for Python v3.7 and torch v1.0, v1.1, v1.4 and v1.7 with good code coverage.
-
-Examples
---------
-
-Creating an AdditiveCoupling with memory savings
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-.. code:: python
-
-    import torch
-    import torch.nn as nn
-    import memcnn
-
-
-    # define a new torch Module with a sequence of operations: Relu o BatchNorm2d o Conv2d
-    class ExampleOperation(nn.Module):
-        def __init__(self, channels):
-            super(ExampleOperation, self).__init__()
-            self.seq = nn.Sequential(
-                                        nn.Conv2d(in_channels=channels, out_channels=channels,
-                                                  kernel_size=(3, 3), padding=1),
-                                        nn.BatchNorm2d(num_features=channels),
-                                        nn.ReLU(inplace=True)
-                                    )
-
-        def forward(self, x):
-            return self.seq(x)
-
-
-    # generate some random input data (batch_size, num_channels, y_elements, x_elements)
-    X = torch.rand(2, 10, 8, 8)
-
-    # application of the operation(s) the normal way
-    model_normal = ExampleOperation(channels=10)
-    model_normal.eval()
-
-    Y = model_normal(X)
-
-    # turn the ExampleOperation invertible using an additive coupling
-    invertible_module = memcnn.AdditiveCoupling(
-        Fm=ExampleOperation(channels=10 // 2),
-        Gm=ExampleOperation(channels=10 // 2)
-    )
-
-    # test that it is actually a valid invertible module (has a valid inverse method)
-    assert memcnn.is_invertible_module(invertible_module, test_input_shape=X.shape)
-
-    # wrap our invertible_module using the InvertibleModuleWrapper and benefit from memory savings during training
-    invertible_module_wrapper = memcnn.InvertibleModuleWrapper(fn=invertible_module, keep_input=True, keep_input_inverse=True)
-
-    # by default the module is set to training, the following sets this to evaluation
-    # note that this is required to pass input tensors to the model with requires_grad=False (inference only)
-    invertible_module_wrapper.eval()
-
-    # test that the wrapped module is also a valid invertible module
-    assert memcnn.is_invertible_module(invertible_module_wrapper, test_input_shape=X.shape)
-
-    # compute the forward pass using the wrapper
-    Y2 = invertible_module_wrapper.forward(X)
-
-    # the input (X) can be approximated (X2) by applying the inverse method of the wrapper on Y2
-    X2 = invertible_module_wrapper.inverse(Y2)
-
-    # test that the input and approximation are similar
-    assert torch.allclose(X, X2, atol=1e-06)
-
-Run PyTorch Experiments
------------------------
-
-After installing MemCNN run:
-
-.. code:: bash
-
-    python -m memcnn.train [MODEL] [DATASET] [--fresh] [--no-cuda]
-
-* Available values for ``DATASET`` are ``cifar10`` and ``cifar100``.
-* Available values for ``MODEL`` are ``resnet32``, ``resnet110``, ``resnet164``, ``revnet38``, ``revnet110``, ``revnet164``
-* Use the ``--fresh`` flag to remove earlier experiment results.
-* Use the ``--no-cuda`` flag to train on the CPU rather than the GPU through CUDA.
-
-Datasets are automatically downloaded if they are not available.
-
-When using Python 3.* replace the ``python`` directive with the appropriate Python 3 directive. For example when using the MemCNN docker image use ``python3.6``.
-
-When MemCNN was installed using `pip` or from sources you might need to setup a configuration file before running this command.
-Read the corresponding section about how to do this here: https://memcnn.readthedocs.io/en/latest/installation.html
-
-
-
```

### Comparing `memcnn-1.5.1/memcnn.egg-info/SOURCES.txt` & `memcnn-1.5.2/memcnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memcnn-1.5.1/setup.py` & `memcnn-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 from distutils.core import setup
 from setuptools.command.install import install
 from setuptools import find_packages
 
 # circleci.py version
-VERSION = '1.5.1'
+VERSION = '1.5.2'
 
 with open('README.rst', 'r') as fh:
     long_description = fh.read().split('Results\n-------')[0]
 
 with open('requirements.txt', 'r') as fh:
     requirements = [e.strip() for e in fh.readlines() if e.strip() != '']
```

