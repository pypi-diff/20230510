# Comparing `tmp/torch_conduit-0.3.0.tar.gz` & `tmp/torch_conduit-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_conduit-0.3.0.tar", max compression
+gzip compressed data, was "torch_conduit-0.3.1.tar", max compression
```

## Comparing `torch_conduit-0.3.0.tar` & `torch_conduit-0.3.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1081 2022-01-09 18:24:01.201254 torch_conduit-0.3.0/LICENSE
--rw-r--r--   0        0        0      408 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/README.md
--rw-r--r--   0        0        0       12 2022-12-18 12:46:23.375194 torch_conduit-0.3.0/conduit/__init__.py
--rw-r--r--   0        0        0     1329 2022-12-19 15:56:41.671401 torch_conduit-0.3.0/conduit/conf/configen.yaml
--rw-r--r--   0        0        0       51 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/__init__.py
--rw-r--r--   0        0        0      208 2022-12-19 15:56:41.671401 torch_conduit-0.3.0/conduit/data/constants.py
--rw-r--r--   0        0        0       20 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datamodules/__init__.py
--rw-r--r--   0        0        0       28 2022-12-18 12:46:23.247194 torch_conduit-0.3.0/conduit/data/datamodules/audio/__init__.py
--rw-r--r--   0        0        0     2558 2023-03-22 19:05:02.482581 torch_conduit-0.3.0/conduit/data/datamodules/audio/base.py
--rw-r--r--   0        0        0     2867 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/data/datamodules/audio/ecoacoustics.py
--rw-r--r--   0        0        0    12126 2023-03-22 15:35:36.662964 torch_conduit-0.3.0/conduit/data/datamodules/base.py
--rw-r--r--   0        0        0        0 2022-12-18 12:46:23.255194 torch_conduit-0.3.0/conduit/data/datamodules/tabular/__init__.py
--rw-r--r--   0        0        0     1091 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datamodules/tabular/dummy.py
--rw-r--r--   0        0        0      186 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/data/datamodules/vision/__init__.py
--rw-r--r--   0        0        0     3987 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datamodules/vision/base.py
--rw-r--r--   0        0        0     2678 2022-12-19 15:56:41.671401 torch_conduit-0.3.0/conduit/data/datamodules/vision/camelyon17.py
--rw-r--r--   0        0        0     2155 2022-12-19 15:56:41.671401 torch_conduit-0.3.0/conduit/data/datamodules/vision/celeba.py
--rw-r--r--   0        0        0     3430 2023-02-01 11:04:32.428283 torch_conduit-0.3.0/conduit/data/datamodules/vision/cmnist.py
--rw-r--r--   0        0        0     1145 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datamodules/vision/dummy.py
--rw-r--r--   0        0        0     1976 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/data/datamodules/vision/nico.py
--rw-r--r--   0        0        0     1980 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/data/datamodules/vision/nico_plus_plus.py
--rw-r--r--   0        0        0     1647 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/data/datamodules/vision/pacs.py
--rw-r--r--   0        0        0     2337 2023-02-02 17:36:21.303492 torch_conduit-0.3.0/conduit/data/datamodules/vision/waterbirds.py
--rw-r--r--   0        0        0       65 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/__init__.py
--rw-r--r--   0        0        0       28 2022-12-18 12:46:23.295194 torch_conduit-0.3.0/conduit/data/datasets/audio/__init__.py
--rw-r--r--   0        0        0     2798 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/data/datasets/audio/base.py
--rw-r--r--   0        0        0    11284 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/data/datasets/audio/ecoacoustics.py
--rw-r--r--   0        0        0    10725 2023-02-02 17:36:21.303492 torch_conduit-0.3.0/conduit/data/datasets/base.py
--rw-r--r--   0        0        0       41 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/tabular/__init__.py
--rw-r--r--   0        0        0     1811 2023-01-18 10:25:37.423919 torch_conduit-0.3.0/conduit/data/datasets/tabular/base.py
--rw-r--r--   0        0        0     1832 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/tabular/dummy.py
--rw-r--r--   0        0        0    27572 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/data/datasets/utils.py
--rw-r--r--   0        0        0      334 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/data/datasets/vision/__init__.py
--rw-r--r--   0        0        0     4834 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/base.py
--rw-r--r--   0        0        0     6351 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/camelyon17.py
--rw-r--r--   0        0        0     5310 2023-02-25 16:39:35.362547 torch_conduit-0.3.0/conduit/data/datasets/vision/celeba.py
--rw-r--r--   0        0        0     9862 2023-04-24 19:49:50.515281 torch_conduit-0.3.0/conduit/data/datasets/vision/cmnist.py
--rw-r--r--   0        0        0     1131 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/dummy.py
--rw-r--r--   0        0        0     8944 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/fmow.py
--rw-r--r--   0        0        0    12403 2023-05-04 15:57:09.326105 torch_conduit-0.3.0/conduit/data/datasets/vision/isic.py
--rw-r--r--   0        0        0     7475 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/iwildcam.py
--rw-r--r--   0        0        0     7221 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/nico.py
--rw-r--r--   0        0        0     8179 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/data/datasets/vision/nico_plus_plus.py
--rw-r--r--   0        0        0     7912 2023-02-01 11:04:32.432283 torch_conduit-0.3.0/conduit/data/datasets/vision/nih.py
--rw-r--r--   0        0        0     6291 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/pacs.py
--rw-r--r--   0        0        0     3917 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/ssrp.py
--rw-r--r--   0        0        0     3610 2023-02-01 11:04:32.432283 torch_conduit-0.3.0/conduit/data/datasets/vision/utils.py
--rw-r--r--   0        0        0       26 2023-02-02 17:36:21.303492 torch_conduit-0.3.0/conduit/data/datasets/vision/waterbirds/__init__.py
--rw-r--r--   0        0        0     5094 2023-02-02 17:36:21.303492 torch_conduit-0.3.0/conduit/data/datasets/vision/waterbirds/waterbirds.py
--rw-r--r--   0        0        0   156339 2023-02-02 17:36:21.303492 torch_conduit-0.3.0/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip
--rw-r--r--   0        0        0     2998 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/vision/wrappers.py
--rw-r--r--   0        0        0     5673 2023-01-19 16:12:52.451248 torch_conduit-0.3.0/conduit/data/datasets/wrappers.py
--rw-r--r--   0        0        0    18335 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/data/structures.py
--rw-r--r--   0        0        0        0 2022-12-18 12:46:23.359194 torch_conduit-0.3.0/conduit/fair/__init__.py
--rw-r--r--   0        0        0       51 2022-12-18 12:46:23.343194 torch_conduit-0.3.0/conduit/fair/data/__init__.py
--rw-r--r--   0        0        0       68 2022-12-18 12:46:23.343194 torch_conduit-0.3.0/conduit/fair/data/datamodules/__init__.py
--rw-r--r--   0        0        0      214 2022-12-18 12:46:23.343194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/__init__.py
--rw-r--r--   0        0        0      692 2022-12-18 12:46:23.335194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/admissions.py
--rw-r--r--   0        0        0      814 2022-12-18 12:46:23.335194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/adult.py
--rw-r--r--   0        0        0     6015 2023-02-01 11:04:32.432283 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/base.py
--rw-r--r--   0        0        0      625 2022-12-18 12:46:23.327194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/compas.py
--rw-r--r--   0        0        0      645 2022-12-18 12:46:23.331194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/credit.py
--rw-r--r--   0        0        0      642 2022-12-18 12:46:23.323194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/crime.py
--rw-r--r--   0        0        0      606 2022-12-18 12:46:23.339194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/german.py
--rw-r--r--   0        0        0      608 2022-12-18 12:46:23.323194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/health.py
--rw-r--r--   0        0        0      573 2022-12-18 12:46:23.327194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/law.py
--rw-r--r--   0        0        0      579 2022-12-18 12:46:23.331194 torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/sqf.py
--rw-r--r--   0        0        0        0 2022-12-18 12:46:23.319194 torch_conduit-0.3.0/conduit/fair/data/datamodules/vision/__init__.py
--rw-r--r--   0        0        0       66 2022-12-18 12:46:23.355194 torch_conduit-0.3.0/conduit/fair/data/datasets/__init__.py
--rw-r--r--   0        0        0      974 2022-12-19 16:39:10.546686 torch_conduit-0.3.0/conduit/fair/data/datasets/dummy.py
--rw-r--r--   0        0        0     2336 2022-12-18 12:46:23.351194 torch_conduit-0.3.0/conduit/fair/data/datasets/ethicml.py
--rw-r--r--   0        0        0        0 2022-12-18 12:46:23.347194 torch_conduit-0.3.0/conduit/fair/data/datasets/vision/__init__.py
--rw-r--r--   0        0        0       20 2022-12-18 12:46:23.359194 torch_conduit-0.3.0/conduit/fair/losses/__init__.py
--rw-r--r--   0        0        0     1041 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/fair/losses/loss.py
--rw-r--r--   0        0        0     5992 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/hydra/conduit/data/datamodules/conf.py
--rw-r--r--   0        0        0     4195 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/hydra/conduit/data/datasets/conf.py
--rw-r--r--   0        0        0     6455 2022-12-19 15:18:44.170868 torch_conduit-0.3.0/conduit/hydra/conduit/fair/data/datamodules/conf.py
--rw-r--r--   0        0        0      457 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/hydra/conduit/models/self_supervised/loss/conf.py
--rw-r--r--   0        0        0      399 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/hydra/conduit/models/self_supervised/memory_bank/conf.py
--rw-r--r--   0        0        0      347 2022-12-18 12:46:23.375194 torch_conduit-0.3.0/conduit/logging.py
--rw-r--r--   0        0        0    20943 2023-05-04 16:42:34.589932 torch_conduit-0.3.0/conduit/metrics.py
--rw-r--r--   0        0        0       21 2022-12-18 12:46:23.383194 torch_conduit-0.3.0/conduit/models/__init__.py
--rw-r--r--   0        0        0    14963 2023-02-01 11:04:32.432283 torch_conduit-0.3.0/conduit/models/self_supervised/loss.py
--rw-r--r--   0        0        0     2386 2022-12-19 15:56:41.675401 torch_conduit-0.3.0/conduit/models/self_supervised/memory_bank.py
--rw-r--r--   0        0        0     1463 2023-04-17 21:49:37.066959 torch_conduit-0.3.0/conduit/models/utils.py
--rw-r--r--   0        0        0     9867 2023-04-17 20:52:30.804691 torch_conduit-0.3.0/conduit/progress.py
--rw-r--r--   0        0        0       64 2022-01-09 18:24:01.201254 torch_conduit-0.3.0/conduit/py.typed
--rw-r--r--   0        0        0      388 2023-04-17 21:49:37.066959 torch_conduit-0.3.0/conduit/structures.py
--rw-r--r--   0        0        0       23 2023-04-17 21:49:37.066959 torch_conduit-0.3.0/conduit/transforms/__init__.py
--rw-r--r--   0        0        0     3216 2022-12-18 12:46:23.371194 torch_conduit-0.3.0/conduit/transforms/audio.py
--rw-r--r--   0        0        0     2490 2023-02-01 11:04:32.432283 torch_conduit-0.3.0/conduit/transforms/fixmatch.py
--rw-r--r--   0        0        0     3271 2022-12-18 12:46:23.363194 torch_conduit-0.3.0/conduit/transforms/image.py
--rw-r--r--   0        0        0     8902 2023-02-01 11:04:32.432283 torch_conduit-0.3.0/conduit/transforms/multicrop.py
--rw-r--r--   0        0        0     6014 2023-01-18 10:25:37.427919 torch_conduit-0.3.0/conduit/transforms/tabular.py
--rw-r--r--   0        0        0     1606 2023-04-17 21:49:37.066959 torch_conduit-0.3.0/conduit/types.py
--rw-r--r--   0        0        0     5899 2023-05-04 16:42:56.678067 torch_conduit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2662 1970-01-01 00:00:00.000000 torch_conduit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-01-09 18:24:01.201254 torch_conduit-0.3.1/LICENSE
+-rw-r--r--   0        0        0      408 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/README.md
+-rw-r--r--   0        0        0       12 2022-12-18 12:46:23.375194 torch_conduit-0.3.1/conduit/__init__.py
+-rw-r--r--   0        0        0     1329 2022-12-19 15:56:41.671401 torch_conduit-0.3.1/conduit/conf/configen.yaml
+-rw-r--r--   0        0        0       51 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/__init__.py
+-rw-r--r--   0        0        0      208 2022-12-19 15:56:41.671401 torch_conduit-0.3.1/conduit/data/constants.py
+-rw-r--r--   0        0        0       20 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datamodules/__init__.py
+-rw-r--r--   0        0        0       28 2022-12-18 12:46:23.247194 torch_conduit-0.3.1/conduit/data/datamodules/audio/__init__.py
+-rw-r--r--   0        0        0     2558 2023-03-22 19:05:02.482581 torch_conduit-0.3.1/conduit/data/datamodules/audio/base.py
+-rw-r--r--   0        0        0     2867 2023-05-04 16:42:34.589932 torch_conduit-0.3.1/conduit/data/datamodules/audio/ecoacoustics.py
+-rw-r--r--   0        0        0    12126 2023-03-22 15:35:36.662964 torch_conduit-0.3.1/conduit/data/datamodules/base.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.255194 torch_conduit-0.3.1/conduit/data/datamodules/tabular/__init__.py
+-rw-r--r--   0        0        0     1091 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datamodules/tabular/dummy.py
+-rw-r--r--   0        0        0      186 2023-05-04 16:42:34.589932 torch_conduit-0.3.1/conduit/data/datamodules/vision/__init__.py
+-rw-r--r--   0        0        0     3987 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datamodules/vision/base.py
+-rw-r--r--   0        0        0     2678 2022-12-19 15:56:41.671401 torch_conduit-0.3.1/conduit/data/datamodules/vision/camelyon17.py
+-rw-r--r--   0        0        0     2155 2022-12-19 15:56:41.671401 torch_conduit-0.3.1/conduit/data/datamodules/vision/celeba.py
+-rw-r--r--   0        0        0     3430 2023-02-01 11:04:32.428283 torch_conduit-0.3.1/conduit/data/datamodules/vision/cmnist.py
+-rw-r--r--   0        0        0     1145 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datamodules/vision/dummy.py
+-rw-r--r--   0        0        0     1976 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/data/datamodules/vision/nico.py
+-rw-r--r--   0        0        0     1980 2023-05-04 16:42:34.589932 torch_conduit-0.3.1/conduit/data/datamodules/vision/nico_plus_plus.py
+-rw-r--r--   0        0        0     1647 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/data/datamodules/vision/pacs.py
+-rw-r--r--   0        0        0     2337 2023-02-02 17:36:21.303492 torch_conduit-0.3.1/conduit/data/datamodules/vision/waterbirds.py
+-rw-r--r--   0        0        0       65 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/__init__.py
+-rw-r--r--   0        0        0       28 2022-12-18 12:46:23.295194 torch_conduit-0.3.1/conduit/data/datasets/audio/__init__.py
+-rw-r--r--   0        0        0     2798 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/data/datasets/audio/base.py
+-rw-r--r--   0        0        0    11284 2023-05-04 16:42:34.589932 torch_conduit-0.3.1/conduit/data/datasets/audio/ecoacoustics.py
+-rw-r--r--   0        0        0    10725 2023-02-02 17:36:21.303492 torch_conduit-0.3.1/conduit/data/datasets/base.py
+-rw-r--r--   0        0        0       41 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/tabular/__init__.py
+-rw-r--r--   0        0        0     1811 2023-01-18 10:25:37.423919 torch_conduit-0.3.1/conduit/data/datasets/tabular/base.py
+-rw-r--r--   0        0        0     1832 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/tabular/dummy.py
+-rw-r--r--   0        0        0    27787 2023-05-10 10:53:13.240908 torch_conduit-0.3.1/conduit/data/datasets/utils.py
+-rw-r--r--   0        0        0      334 2023-05-04 16:42:34.589932 torch_conduit-0.3.1/conduit/data/datasets/vision/__init__.py
+-rw-r--r--   0        0        0     4834 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/base.py
+-rw-r--r--   0        0        0     6351 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/camelyon17.py
+-rw-r--r--   0        0        0     5310 2023-02-25 16:39:35.362547 torch_conduit-0.3.1/conduit/data/datasets/vision/celeba.py
+-rw-r--r--   0        0        0     9862 2023-04-24 19:49:50.515281 torch_conduit-0.3.1/conduit/data/datasets/vision/cmnist.py
+-rw-r--r--   0        0        0     1131 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/dummy.py
+-rw-r--r--   0        0        0     8944 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/fmow.py
+-rw-r--r--   0        0        0    12403 2023-05-04 15:57:09.326105 torch_conduit-0.3.1/conduit/data/datasets/vision/isic.py
+-rw-r--r--   0        0        0     7475 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/iwildcam.py
+-rw-r--r--   0        0        0     7221 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/nico.py
+-rw-r--r--   0        0        0     8179 2023-05-04 16:42:34.589932 torch_conduit-0.3.1/conduit/data/datasets/vision/nico_plus_plus.py
+-rw-r--r--   0        0        0     7912 2023-02-01 11:04:32.432283 torch_conduit-0.3.1/conduit/data/datasets/vision/nih.py
+-rw-r--r--   0        0        0     6291 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/pacs.py
+-rw-r--r--   0        0        0     3917 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/ssrp.py
+-rw-r--r--   0        0        0     3610 2023-02-01 11:04:32.432283 torch_conduit-0.3.1/conduit/data/datasets/vision/utils.py
+-rw-r--r--   0        0        0       26 2023-02-02 17:36:21.303492 torch_conduit-0.3.1/conduit/data/datasets/vision/waterbirds/__init__.py
+-rw-r--r--   0        0        0     5094 2023-02-02 17:36:21.303492 torch_conduit-0.3.1/conduit/data/datasets/vision/waterbirds/waterbirds.py
+-rw-r--r--   0        0        0   156339 2023-02-02 17:36:21.303492 torch_conduit-0.3.1/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip
+-rw-r--r--   0        0        0     2998 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/vision/wrappers.py
+-rw-r--r--   0        0        0     5673 2023-01-19 16:12:52.451248 torch_conduit-0.3.1/conduit/data/datasets/wrappers.py
+-rw-r--r--   0        0        0    18335 2023-05-04 16:42:34.589932 torch_conduit-0.3.1/conduit/data/structures.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.359194 torch_conduit-0.3.1/conduit/fair/__init__.py
+-rw-r--r--   0        0        0       51 2022-12-18 12:46:23.343194 torch_conduit-0.3.1/conduit/fair/data/__init__.py
+-rw-r--r--   0        0        0       68 2022-12-18 12:46:23.343194 torch_conduit-0.3.1/conduit/fair/data/datamodules/__init__.py
+-rw-r--r--   0        0        0      214 2022-12-18 12:46:23.343194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/__init__.py
+-rw-r--r--   0        0        0      692 2022-12-18 12:46:23.335194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/admissions.py
+-rw-r--r--   0        0        0      814 2022-12-18 12:46:23.335194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/adult.py
+-rw-r--r--   0        0        0     6015 2023-02-01 11:04:32.432283 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/base.py
+-rw-r--r--   0        0        0      625 2022-12-18 12:46:23.327194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/compas.py
+-rw-r--r--   0        0        0      645 2022-12-18 12:46:23.331194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/credit.py
+-rw-r--r--   0        0        0      642 2022-12-18 12:46:23.323194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/crime.py
+-rw-r--r--   0        0        0      606 2022-12-18 12:46:23.339194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/german.py
+-rw-r--r--   0        0        0      608 2022-12-18 12:46:23.323194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/health.py
+-rw-r--r--   0        0        0      573 2022-12-18 12:46:23.327194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/law.py
+-rw-r--r--   0        0        0      579 2022-12-18 12:46:23.331194 torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/sqf.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.319194 torch_conduit-0.3.1/conduit/fair/data/datamodules/vision/__init__.py
+-rw-r--r--   0        0        0       66 2022-12-18 12:46:23.355194 torch_conduit-0.3.1/conduit/fair/data/datasets/__init__.py
+-rw-r--r--   0        0        0      974 2022-12-19 16:39:10.546686 torch_conduit-0.3.1/conduit/fair/data/datasets/dummy.py
+-rw-r--r--   0        0        0     2336 2022-12-18 12:46:23.351194 torch_conduit-0.3.1/conduit/fair/data/datasets/ethicml.py
+-rw-r--r--   0        0        0        0 2022-12-18 12:46:23.347194 torch_conduit-0.3.1/conduit/fair/data/datasets/vision/__init__.py
+-rw-r--r--   0        0        0       20 2022-12-18 12:46:23.359194 torch_conduit-0.3.1/conduit/fair/losses/__init__.py
+-rw-r--r--   0        0        0     1041 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/fair/losses/loss.py
+-rw-r--r--   0        0        0     5992 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/hydra/conduit/data/datamodules/conf.py
+-rw-r--r--   0        0        0     4195 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/hydra/conduit/data/datasets/conf.py
+-rw-r--r--   0        0        0     6455 2022-12-19 15:18:44.170868 torch_conduit-0.3.1/conduit/hydra/conduit/fair/data/datamodules/conf.py
+-rw-r--r--   0        0        0      457 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/hydra/conduit/models/self_supervised/loss/conf.py
+-rw-r--r--   0        0        0      399 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/hydra/conduit/models/self_supervised/memory_bank/conf.py
+-rw-r--r--   0        0        0      347 2022-12-18 12:46:23.375194 torch_conduit-0.3.1/conduit/logging.py
+-rw-r--r--   0        0        0    20943 2023-05-04 16:42:34.589932 torch_conduit-0.3.1/conduit/metrics.py
+-rw-r--r--   0        0        0       21 2022-12-18 12:46:23.383194 torch_conduit-0.3.1/conduit/models/__init__.py
+-rw-r--r--   0        0        0    14963 2023-02-01 11:04:32.432283 torch_conduit-0.3.1/conduit/models/self_supervised/loss.py
+-rw-r--r--   0        0        0     2386 2022-12-19 15:56:41.675401 torch_conduit-0.3.1/conduit/models/self_supervised/memory_bank.py
+-rw-r--r--   0        0        0     1463 2023-04-17 21:49:37.066959 torch_conduit-0.3.1/conduit/models/utils.py
+-rw-r--r--   0        0        0     9867 2023-04-17 20:52:30.804691 torch_conduit-0.3.1/conduit/progress.py
+-rw-r--r--   0        0        0       64 2022-01-09 18:24:01.201254 torch_conduit-0.3.1/conduit/py.typed
+-rw-r--r--   0        0        0      388 2023-04-17 21:49:37.066959 torch_conduit-0.3.1/conduit/structures.py
+-rw-r--r--   0        0        0       23 2023-04-17 21:49:37.066959 torch_conduit-0.3.1/conduit/transforms/__init__.py
+-rw-r--r--   0        0        0     3216 2022-12-18 12:46:23.371194 torch_conduit-0.3.1/conduit/transforms/audio.py
+-rw-r--r--   0        0        0     2490 2023-02-01 11:04:32.432283 torch_conduit-0.3.1/conduit/transforms/fixmatch.py
+-rw-r--r--   0        0        0     3271 2022-12-18 12:46:23.363194 torch_conduit-0.3.1/conduit/transforms/image.py
+-rw-r--r--   0        0        0     8902 2023-02-01 11:04:32.432283 torch_conduit-0.3.1/conduit/transforms/multicrop.py
+-rw-r--r--   0        0        0     6014 2023-01-18 10:25:37.427919 torch_conduit-0.3.1/conduit/transforms/tabular.py
+-rw-r--r--   0        0        0     1606 2023-04-17 21:49:37.066959 torch_conduit-0.3.1/conduit/types.py
+-rw-r--r--   0        0        0     5899 2023-05-10 10:53:21.148952 torch_conduit-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2662 1970-01-01 00:00:00.000000 torch_conduit-0.3.1/PKG-INFO
```

### Comparing `torch_conduit-0.3.0/LICENSE` & `torch_conduit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/conf/configen.yaml` & `torch_conduit-0.3.1/conduit/conf/configen.yaml`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/audio/base.py` & `torch_conduit-0.3.1/conduit/data/datamodules/audio/base.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/audio/ecoacoustics.py` & `torch_conduit-0.3.1/conduit/data/datamodules/audio/ecoacoustics.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/base.py` & `torch_conduit-0.3.1/conduit/data/datamodules/base.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/tabular/dummy.py` & `torch_conduit-0.3.1/conduit/data/datamodules/tabular/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/base.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/base.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/camelyon17.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/camelyon17.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/celeba.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/celeba.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/cmnist.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/cmnist.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/dummy.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/nico.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/nico.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/nico_plus_plus.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/nico_plus_plus.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/pacs.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/pacs.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datamodules/vision/waterbirds.py` & `torch_conduit-0.3.1/conduit/data/datamodules/vision/waterbirds.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/audio/base.py` & `torch_conduit-0.3.1/conduit/data/datasets/audio/base.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/audio/ecoacoustics.py` & `torch_conduit-0.3.1/conduit/data/datasets/audio/ecoacoustics.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/base.py` & `torch_conduit-0.3.1/conduit/data/datasets/base.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/tabular/base.py` & `torch_conduit-0.3.1/conduit/data/datasets/tabular/base.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/tabular/dummy.py` & `torch_conduit-0.3.1/conduit/data/datasets/tabular/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/utils.py` & `torch_conduit-0.3.1/conduit/data/datasets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,15 +314,18 @@
         # Tensor
         elif isinstance(elem, Tensor):
             out = None
             if torch.utils.data.get_worker_info() is not None:  # type: ignore
                 # If we're in a background process, concatenate directly into a
                 # shared memory tensor to avoid an extra copy
                 numel = sum(x.numel() for x in batch)
-                storage = elem.storage()._new_shared(numel)
+                if hasattr(elem, "_typed_storage"):  # in PyTorch 2.0, it's called _typed_storage
+                    storage = elem._typed_storage()._new_shared(numel, device=elem.device)
+                else:
+                    storage = elem.storage()._new_shared(numel)
                 out = elem.new(storage).resize_(len(batch), *list(elem.size()))
             ndims = elem.dim()
             # If 'batch' is a sequence of sub-batched tensors we concatenate the elements along the
             # batch dimesion. Note, the problem of inferring whether the tensors are sub-batched or
             # not is ill-posed given that the dimensionality of samples varies with modality; the
             # current solution is tailored for tabular and image data.
             if (ndims > 0) and ((ndims % 2) == 0):
```

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/base.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/base.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/camelyon17.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/camelyon17.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/celeba.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/celeba.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/cmnist.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/cmnist.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/dummy.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/fmow.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/fmow.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/isic.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/isic.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/iwildcam.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/iwildcam.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/nico.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/nico.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/nico_plus_plus.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/nico_plus_plus.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/nih.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/nih.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/pacs.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/pacs.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/ssrp.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/ssrp.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/utils.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/utils.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/waterbirds/waterbirds.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/waterbirds/waterbirds.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip` & `torch_conduit-0.3.1/conduit/data/datasets/vision/waterbirds/waterbirds_fixed.csv.zip`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/vision/wrappers.py` & `torch_conduit-0.3.1/conduit/data/datasets/vision/wrappers.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/datasets/wrappers.py` & `torch_conduit-0.3.1/conduit/data/datasets/wrappers.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/data/structures.py` & `torch_conduit-0.3.1/conduit/data/structures.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/admissions.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/admissions.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/adult.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/adult.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/base.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/base.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/compas.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/compas.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/credit.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/credit.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/crime.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/crime.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/german.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/german.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/health.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/health.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/law.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/law.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datamodules/tabular/sqf.py` & `torch_conduit-0.3.1/conduit/fair/data/datamodules/tabular/sqf.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datasets/dummy.py` & `torch_conduit-0.3.1/conduit/fair/data/datasets/dummy.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/data/datasets/ethicml.py` & `torch_conduit-0.3.1/conduit/fair/data/datasets/ethicml.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/fair/losses/loss.py` & `torch_conduit-0.3.1/conduit/fair/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/hydra/conduit/data/datamodules/conf.py` & `torch_conduit-0.3.1/conduit/hydra/conduit/data/datamodules/conf.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/hydra/conduit/data/datasets/conf.py` & `torch_conduit-0.3.1/conduit/hydra/conduit/data/datasets/conf.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/hydra/conduit/fair/data/datamodules/conf.py` & `torch_conduit-0.3.1/conduit/hydra/conduit/fair/data/datamodules/conf.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/metrics.py` & `torch_conduit-0.3.1/conduit/metrics.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/models/self_supervised/loss.py` & `torch_conduit-0.3.1/conduit/models/self_supervised/loss.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/models/self_supervised/memory_bank.py` & `torch_conduit-0.3.1/conduit/models/self_supervised/memory_bank.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/models/utils.py` & `torch_conduit-0.3.1/conduit/models/utils.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/progress.py` & `torch_conduit-0.3.1/conduit/progress.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/transforms/audio.py` & `torch_conduit-0.3.1/conduit/transforms/audio.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/transforms/fixmatch.py` & `torch_conduit-0.3.1/conduit/transforms/fixmatch.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/transforms/image.py` & `torch_conduit-0.3.1/conduit/transforms/image.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/transforms/multicrop.py` & `torch_conduit-0.3.1/conduit/transforms/multicrop.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/transforms/tabular.py` & `torch_conduit-0.3.1/conduit/transforms/tabular.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/conduit/types.py` & `torch_conduit-0.3.1/conduit/types.py`

 * *Files identical despite different names*

### Comparing `torch_conduit-0.3.0/pyproject.toml` & `torch_conduit-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "torch-conduit"
-version = "0.3.0"
+version = "0.3.1"
 description = "Lightweight framework for dataloading with PyTorch and channeling the power of PyTorch Lightning"
 authors = ["PAL <info@predictive-analytics-lab.com>"]
 license = "Apache License 2.0"
 packages = [
   { include = "conduit" },
 ]
 include=["conduit/py.typed"]
```

### Comparing `torch_conduit-0.3.0/PKG-INFO` & `torch_conduit-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-conduit
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lightweight framework for dataloading with PyTorch and channeling the power of PyTorch Lightning
 Home-page: https://github.com/wearepal/conduit
 License: Apache-2.0
 Keywords: typing,python,pytorch,datasets,pytorch-lightning,lightning-bolts
 Author: PAL
 Author-email: info@predictive-analytics-lab.com
 Requires-Python: >=3.8.0,<3.12
```

