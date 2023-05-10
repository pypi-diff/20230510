# Comparing `tmp/premium-23.5.10.16.tar.gz` & `tmp/premium-23.5.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/premium-23.5.10.16.tar", last modified: Wed May 10 08:21:49 2023, max compression
+gzip compressed data, was "dist/premium-23.5.11.1.tar", last modified: Tue May  9 16:25:30 2023, max compression
```

## Comparing `premium-23.5.10.16.tar` & `premium-23.5.11.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.124971 premium-23.5.10.16/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      351 2023-05-10 08:21:49.120972 premium-23.5.10.16/PKG-INFO
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-08-20 00:45:22.000000 premium-23.5.10.16/README.md
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.096971 premium-23.5.10.16/data/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-05 09:52:56.000000 premium-23.5.10.16/data/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.100971 premium-23.5.10.16/data/config/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-11-05 09:52:37.000000 premium-23.5.10.16/data/config/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.100971 premium-23.5.10.16/premium/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       46 2023-04-12 13:39:31.000000 premium-23.5.10.16/premium/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.100971 premium-23.5.10.16/premium/algorithm/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-09-18 07:48:09.000000 premium-23.5.10.16/premium/algorithm/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.100971 premium-23.5.10.16/premium/automl/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      726 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/automl/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.100971 premium-23.5.10.16/premium/base/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-02-28 03:25:12.000000 premium-23.5.10.16/premium/base/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      988 2023-02-28 03:25:36.000000 premium-23.5.10.16/premium/base/pipeline.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.100971 premium-23.5.10.16/premium/classifiers/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-12 08:44:25.000000 premium-23.5.10.16/premium/classifiers/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     4588 2023-05-08 12:52:56.000000 premium-23.5.10.16/premium/classifiers/baseline.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.100971 premium-23.5.10.16/premium/classifiers/binary/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-05-08 09:46:49.000000 premium-23.5.10.16/premium/classifiers/binary/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      111 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/config.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.104971 premium-23.5.10.16/premium/corpus/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       30 2023-02-13 02:48:47.000000 premium-23.5.10.16/premium/corpus/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1074 2023-02-16 01:59:57.000000 premium-23.5.10.16/premium/corpus/stopwords.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      933 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/corpus/texts.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      447 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/corpus/utils.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.104971 premium-23.5.10.16/premium/data/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        4 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/data/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3344 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/data/_dict.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2136 2022-08-21 08:32:02.000000 premium-23.5.10.16/premium/data/augumentation.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.104971 premium-23.5.10.16/premium/data/classification/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2022-12-15 03:45:19.000000 premium-23.5.10.16/premium/data/classification/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3682 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/data/csv.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     9076 2023-05-09 05:48:14.000000 premium-23.5.10.16/premium/data/datasets.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3002 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/data/eda.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1418 2022-12-19 07:47:54.000000 premium-23.5.10.16/premium/data/loader.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2277 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/data/postprocess.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    12455 2023-04-28 13:08:42.000000 premium-23.5.10.16/premium/data/preprocess.py
--rwxrwxr-x   0 gaoang    (1001) gaoang    (1001)     4670 2022-12-22 11:10:43.000000 premium-23.5.10.16/premium/data/utils.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6551 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/demo.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      684 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/draw.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.104971 premium-23.5.10.16/premium/experimental/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/experimental/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     6624 2022-08-31 13:10:31.000000 premium-23.5.10.16/premium/experimental/cbow.py
--rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)     2569 2022-09-06 07:29:08.000000 premium-23.5.10.16/premium/experimental/eda.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1462 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/experimental/kaggle.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     8572 2023-04-12 10:55:43.000000 premium-23.5.10.16/premium/experimental/myfasttext.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1498 2022-09-06 23:56:22.000000 premium-23.5.10.16/premium/experimental/ner.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2272 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/experimental/nn_metric.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     2914 2022-11-01 04:49:36.000000 premium-23.5.10.16/premium/experimental/segment_train.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     3315 2022-09-02 02:26:29.000000 premium-23.5.10.16/premium/experimental/textnn.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)    14328 2022-12-19 07:00:16.000000 premium-23.5.10.16/premium/experimental/torch_crf.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2385 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/frame.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     8076 2022-09-27 06:32:40.000000 premium-23.5.10.16/premium/hmm.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.104971 premium-23.5.10.16/premium/lightning/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        0 2023-04-17 06:05:11.000000 premium-23.5.10.16/premium/lightning/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2213 2023-05-04 13:34:16.000000 premium-23.5.10.16/premium/lightning/callbacks.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.112971 premium-23.5.10.16/premium/localdata/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)  1001504 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/27.mp3
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)  5340812 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/27.wav
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4695 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/cn_stopwords.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)  1134854 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/dict.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)   278548 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/emit_p.pickle
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      621 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/en_stopwords.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       61 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/oov.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)   844962 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/puredict.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)   755791 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/soledad.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      176 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/trans.pickle
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)  7310398 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/localdata/xinhua.txt
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2803 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/measure.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.116971 premium-23.5.10.16/premium/metrics/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      660 2023-03-22 07:48:42.000000 premium-23.5.10.16/premium/metrics/__init__.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)      876 2022-10-22 08:56:25.000000 premium-23.5.10.16/premium/metrics/distance.py
--rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)     2990 2023-04-12 11:56:01.000000 premium-23.5.10.16/premium/metrics/metrix.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.120972 premium-23.5.10.16/premium/models/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       42 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6835 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/base.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      200 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/bayes.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3178 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/benchmark.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    15555 2022-09-02 07:01:51.000000 premium-23.5.10.16/premium/models/bert.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6238 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/binary_classifiers.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3939 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/clf.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    10472 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/lgb.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2697 2022-11-03 11:20:22.000000 premium-23.5.10.16/premium/models/model_config.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     6144 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/multi_classifier.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)    22231 2022-09-04 03:09:30.000000 premium-23.5.10.16/premium/models/nn.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4954 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/optuna.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     7796 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/regressor.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.120972 premium-23.5.10.16/premium/models/tensorflow/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      127 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/tensorflow/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2857 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/tensorflow/binary_classifier.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      186 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/tensorflow/info.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)    11038 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/touchstone.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1783 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/models/xgb.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.120972 premium-23.5.10.16/premium/nlp/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       66 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/nlp/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3209 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/nlp/metrics.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1212 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/nlp/net.py
--rwxr--r--   0 gaoang    (1001) gaoang    (1001)     1086 2022-09-06 23:53:01.000000 premium-23.5.10.16/premium/nlp/nlp.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.120972 premium-23.5.10.16/premium/preprocessing/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        0 2022-09-04 01:32:49.000000 premium-23.5.10.16/premium/preprocessing/__init__.py
--rwxrwxr-x   0 gaoang    (1001) gaoang    (1001)     2933 2023-05-04 12:57:40.000000 premium-23.5.10.16/premium/preprocessing/ner.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      425 2023-05-10 08:21:09.000000 premium-23.5.10.16/premium/preprocessing/text.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.120972 premium-23.5.10.16/premium/pytorch/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      849 2022-11-11 02:06:02.000000 premium-23.5.10.16/premium/pytorch/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1772 2023-02-16 13:53:00.000000 premium-23.5.10.16/premium/pytorch/data.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2471 2022-12-08 04:52:17.000000 premium-23.5.10.16/premium/pytorch/tokenizer.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2136 2022-11-11 03:50:39.000000 premium-23.5.10.16/premium/pytorch/trainer.py
--rwxr-xr-x   0 gaoang    (1001) gaoang    (1001)      275 2022-12-15 03:41:20.000000 premium-23.5.10.16/premium/pytorch/utils.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     5369 2022-09-14 00:12:27.000000 premium-23.5.10.16/premium/segment.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.120972 premium-23.5.10.16/premium/text_feature/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       36 2022-11-23 03:47:20.000000 premium-23.5.10.16/premium/text_feature/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     4938 2022-11-23 03:47:52.000000 premium-23.5.10.16/premium/text_feature/bm25.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     3362 2022-11-29 11:47:18.000000 premium-23.5.10.16/premium/text_feature/sif.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.120972 premium-23.5.10.16/premium/utils/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1661 2022-12-06 08:25:40.000000 premium-23.5.10.16/premium/utils/__init__.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      563 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/utils/decorators.py
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      988 2022-08-20 00:43:56.000000 premium-23.5.10.16/premium/zz.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-10 08:21:49.100971 premium-23.5.10.16/premium.egg-info/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      351 2023-05-10 08:21:49.000000 premium-23.5.10.16/premium.egg-info/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2757 2023-05-10 08:21:49.000000 premium-23.5.10.16/premium.egg-info/SOURCES.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-05-10 08:21:49.000000 premium-23.5.10.16/premium.egg-info/dependency_links.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       65 2023-05-10 08:21:49.000000 premium-23.5.10.16/premium.egg-info/entry_points.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       76 2023-05-10 08:21:49.000000 premium-23.5.10.16/premium.egg-info/requires.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       13 2023-05-10 08:21:49.000000 premium-23.5.10.16/premium.egg-info/top_level.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-05-10 08:21:49.124971 premium-23.5.10.16/setup.cfg
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     1133 2023-05-09 16:25:54.000000 premium-23.5.10.16/setup.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.374936 premium-23.5.11.1/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      350 2023-05-09 16:25:30.374936 premium-23.5.11.1/PKG-INFO
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-08-20 00:45:22.000000 premium-23.5.11.1/README.md
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.170935 premium-23.5.11.1/data/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-11-05 09:52:56.000000 premium-23.5.11.1/data/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.174935 premium-23.5.11.1/data/config/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-11-05 09:52:37.000000 premium-23.5.11.1/data/config/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.186935 premium-23.5.11.1/premium/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       46 2023-04-12 13:39:31.000000 premium-23.5.11.1/premium/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.194935 premium-23.5.11.1/premium/algorithm/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-09-18 07:48:09.000000 premium-23.5.11.1/premium/algorithm/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.194935 premium-23.5.11.1/premium/automl/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      726 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/automl/__init__.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.194935 premium-23.5.11.1/premium/base/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-02-28 03:25:12.000000 premium-23.5.11.1/premium/base/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      988 2023-02-28 03:25:36.000000 premium-23.5.11.1/premium/base/pipeline.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.198935 premium-23.5.11.1/premium/classifiers/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-04-12 08:44:25.000000 premium-23.5.11.1/premium/classifiers/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4588 2023-05-08 12:52:53.000000 premium-23.5.11.1/premium/classifiers/baseline.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.198935 premium-23.5.11.1/premium/classifiers/binary/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-05-08 09:46:49.000000 premium-23.5.11.1/premium/classifiers/binary/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      111 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/config.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.206935 premium-23.5.11.1/premium/corpus/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       30 2023-02-13 02:48:47.000000 premium-23.5.11.1/premium/corpus/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1074 2023-02-16 01:59:57.000000 premium-23.5.11.1/premium/corpus/stopwords.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      933 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/corpus/texts.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      447 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/corpus/utils.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.222935 premium-23.5.11.1/premium/data/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        4 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/data/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3344 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/data/_dict.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2136 2022-08-21 08:32:02.000000 premium-23.5.11.1/premium/data/augumentation.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.226935 premium-23.5.11.1/premium/data/classification/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-12-15 03:45:19.000000 premium-23.5.11.1/premium/data/classification/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3682 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/data/csv.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     9076 2023-05-09 05:48:14.000000 premium-23.5.11.1/premium/data/datasets.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3002 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/data/eda.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1418 2022-12-19 07:47:54.000000 premium-23.5.11.1/premium/data/loader.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2277 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/data/postprocess.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    12455 2023-04-28 13:08:42.000000 premium-23.5.11.1/premium/data/preprocess.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     4670 2022-12-22 11:10:43.000000 premium-23.5.11.1/premium/data/utils.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6551 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/demo.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      684 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/draw.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.234935 premium-23.5.11.1/premium/experimental/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/experimental/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     6624 2022-08-31 13:10:31.000000 premium-23.5.11.1/premium/experimental/cbow.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2569 2022-09-06 07:29:08.000000 premium-23.5.11.1/premium/experimental/eda.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1462 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/experimental/kaggle.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     8572 2023-04-12 10:55:43.000000 premium-23.5.11.1/premium/experimental/myfasttext.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1498 2022-09-06 23:56:22.000000 premium-23.5.11.1/premium/experimental/ner.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2272 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/experimental/nn_metric.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2914 2022-11-01 04:49:36.000000 premium-23.5.11.1/premium/experimental/segment_train.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     3315 2022-09-02 02:26:29.000000 premium-23.5.11.1/premium/experimental/textnn.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    14328 2022-12-19 07:00:16.000000 premium-23.5.11.1/premium/experimental/torch_crf.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2385 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/frame.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     8076 2022-09-27 06:27:21.000000 premium-23.5.11.1/premium/hmm.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.234935 premium-23.5.11.1/premium/lightning/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2023-04-17 06:05:11.000000 premium-23.5.11.1/premium/lightning/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2213 2023-05-04 13:34:16.000000 premium-23.5.11.1/premium/lightning/callbacks.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.294935 premium-23.5.11.1/premium/localdata/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)  1001504 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/27.mp3
+-rw-r--r--   0 tp03      (1000) tp03      (1000)  5340812 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/27.wav
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4695 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/cn_stopwords.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)  1134854 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/dict.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)   278548 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/emit_p.pickle
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      621 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/en_stopwords.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       61 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/oov.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)   844962 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/puredict.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)   755791 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/soledad.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      176 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/trans.pickle
+-rw-r--r--   0 tp03      (1000) tp03      (1000)  7310398 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/localdata/xinhua.txt
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2803 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/measure.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.330936 premium-23.5.11.1/premium/metrics/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      660 2023-03-22 07:48:42.000000 premium-23.5.11.1/premium/metrics/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)      876 2022-10-22 08:56:25.000000 premium-23.5.11.1/premium/metrics/distance.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2990 2023-04-12 11:56:01.000000 premium-23.5.11.1/premium/metrics/metrix.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.350936 premium-23.5.11.1/premium/models/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       42 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6835 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/base.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      200 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/bayes.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3178 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/benchmark.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    15555 2022-09-02 07:01:51.000000 premium-23.5.11.1/premium/models/bert.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6238 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/binary_classifiers.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3939 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/clf.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    10472 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/lgb.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2697 2022-11-03 11:20:22.000000 premium-23.5.11.1/premium/models/model_config.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     6144 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/multi_classifier.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)    22231 2022-09-04 03:09:30.000000 premium-23.5.11.1/premium/models/nn.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4954 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/optuna.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     7796 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/regressor.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.350936 premium-23.5.11.1/premium/models/tensorflow/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      127 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/tensorflow/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2857 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/tensorflow/binary_classifier.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      186 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/tensorflow/info.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)    11038 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/touchstone.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1783 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/models/xgb.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.354936 premium-23.5.11.1/premium/nlp/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       66 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/nlp/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3209 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/nlp/metrics.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1212 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/nlp/net.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     1086 2022-09-06 23:53:01.000000 premium-23.5.11.1/premium/nlp/nlp.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.358936 premium-23.5.11.1/premium/preprocessing/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)        0 2022-09-04 01:32:49.000000 premium-23.5.11.1/premium/preprocessing/__init__.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)     2933 2023-05-04 12:57:40.000000 premium-23.5.11.1/premium/preprocessing/ner.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2435 2022-09-05 23:32:12.000000 premium-23.5.11.1/premium/preprocessing/text.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.366936 premium-23.5.11.1/premium/pytorch/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      849 2022-11-11 02:06:02.000000 premium-23.5.11.1/premium/pytorch/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1772 2023-02-16 13:53:00.000000 premium-23.5.11.1/premium/pytorch/data.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2471 2022-12-08 04:52:17.000000 premium-23.5.11.1/premium/pytorch/tokenizer.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     2136 2022-11-11 03:50:39.000000 premium-23.5.11.1/premium/pytorch/trainer.py
+-rwxr--r--   0 tp03      (1000) tp03      (1000)      275 2022-12-15 03:41:20.000000 premium-23.5.11.1/premium/pytorch/utils.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     5369 2022-09-14 00:12:27.000000 premium-23.5.11.1/premium/segment.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.370936 premium-23.5.11.1/premium/text_feature/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       36 2022-11-23 03:47:20.000000 premium-23.5.11.1/premium/text_feature/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     4938 2022-11-23 03:47:52.000000 premium-23.5.11.1/premium/text_feature/bm25.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3362 2022-11-29 11:47:18.000000 premium-23.5.11.1/premium/text_feature/sif.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.370936 premium-23.5.11.1/premium/utils/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1661 2022-12-06 08:25:40.000000 premium-23.5.11.1/premium/utils/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      563 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/utils/decorators.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      988 2022-08-20 00:43:56.000000 premium-23.5.11.1/premium/zz.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-05-09 16:25:30.194935 premium-23.5.11.1/premium.egg-info/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      350 2023-05-09 16:25:29.000000 premium-23.5.11.1/premium.egg-info/PKG-INFO
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)     2757 2023-05-09 16:25:29.000000 premium-23.5.11.1/premium.egg-info/SOURCES.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-05-09 16:25:29.000000 premium-23.5.11.1/premium.egg-info/dependency_links.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       65 2023-05-09 16:25:29.000000 premium-23.5.11.1/premium.egg-info/entry_points.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       76 2023-05-09 16:25:29.000000 premium-23.5.11.1/premium.egg-info/requires.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       13 2023-05-09 16:25:29.000000 premium-23.5.11.1/premium.egg-info/top_level.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-05-09 16:25:30.374936 premium-23.5.11.1/setup.cfg
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1123 2023-05-09 16:25:23.000000 premium-23.5.11.1/setup.py
```

### Comparing `premium-23.5.10.16/premium/automl/__init__.py` & `premium-23.5.11.1/premium/automl/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/base/pipeline.py` & `premium-23.5.11.1/premium/base/pipeline.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/classifiers/baseline.py` & `premium-23.5.11.1/premium/classifiers/baseline.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/corpus/stopwords.py` & `premium-23.5.11.1/premium/corpus/stopwords.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/corpus/texts.py` & `premium-23.5.11.1/premium/corpus/texts.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/_dict.py` & `premium-23.5.11.1/premium/data/_dict.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/augumentation.py` & `premium-23.5.11.1/premium/data/augumentation.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/csv.py` & `premium-23.5.11.1/premium/data/csv.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/datasets.py` & `premium-23.5.11.1/premium/data/datasets.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/eda.py` & `premium-23.5.11.1/premium/data/eda.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/loader.py` & `premium-23.5.11.1/premium/data/loader.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/postprocess.py` & `premium-23.5.11.1/premium/data/postprocess.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/preprocess.py` & `premium-23.5.11.1/premium/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/data/utils.py` & `premium-23.5.11.1/premium/data/utils.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/demo.py` & `premium-23.5.11.1/premium/demo.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/draw.py` & `premium-23.5.11.1/premium/draw.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/cbow.py` & `premium-23.5.11.1/premium/experimental/cbow.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/eda.py` & `premium-23.5.11.1/premium/experimental/eda.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/kaggle.py` & `premium-23.5.11.1/premium/experimental/kaggle.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/myfasttext.py` & `premium-23.5.11.1/premium/experimental/myfasttext.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/ner.py` & `premium-23.5.11.1/premium/experimental/ner.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/nn_metric.py` & `premium-23.5.11.1/premium/experimental/nn_metric.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/segment_train.py` & `premium-23.5.11.1/premium/experimental/segment_train.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/textnn.py` & `premium-23.5.11.1/premium/experimental/textnn.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/experimental/torch_crf.py` & `premium-23.5.11.1/premium/experimental/torch_crf.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/frame.py` & `premium-23.5.11.1/premium/frame.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/hmm.py` & `premium-23.5.11.1/premium/hmm.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/lightning/callbacks.py` & `premium-23.5.11.1/premium/lightning/callbacks.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/27.mp3` & `premium-23.5.11.1/premium/localdata/27.mp3`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/27.wav` & `premium-23.5.11.1/premium/localdata/27.wav`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/cn_stopwords.txt` & `premium-23.5.11.1/premium/localdata/cn_stopwords.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/dict.txt` & `premium-23.5.11.1/premium/localdata/dict.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/emit_p.pickle` & `premium-23.5.11.1/premium/localdata/emit_p.pickle`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/en_stopwords.txt` & `premium-23.5.11.1/premium/localdata/en_stopwords.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/puredict.txt` & `premium-23.5.11.1/premium/localdata/puredict.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/soledad.txt` & `premium-23.5.11.1/premium/localdata/soledad.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/localdata/xinhua.txt` & `premium-23.5.11.1/premium/localdata/xinhua.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/measure.py` & `premium-23.5.11.1/premium/measure.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/metrics/__init__.py` & `premium-23.5.11.1/premium/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/metrics/distance.py` & `premium-23.5.11.1/premium/metrics/distance.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/metrics/metrix.py` & `premium-23.5.11.1/premium/metrics/metrix.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/base.py` & `premium-23.5.11.1/premium/models/base.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/benchmark.py` & `premium-23.5.11.1/premium/models/benchmark.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/bert.py` & `premium-23.5.11.1/premium/models/bert.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/binary_classifiers.py` & `premium-23.5.11.1/premium/models/binary_classifiers.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/clf.py` & `premium-23.5.11.1/premium/models/clf.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/lgb.py` & `premium-23.5.11.1/premium/models/lgb.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/model_config.py` & `premium-23.5.11.1/premium/models/model_config.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/multi_classifier.py` & `premium-23.5.11.1/premium/models/multi_classifier.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/nn.py` & `premium-23.5.11.1/premium/models/nn.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/optuna.py` & `premium-23.5.11.1/premium/models/optuna.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/regressor.py` & `premium-23.5.11.1/premium/models/regressor.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/tensorflow/binary_classifier.py` & `premium-23.5.11.1/premium/models/tensorflow/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/touchstone.py` & `premium-23.5.11.1/premium/models/touchstone.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/models/xgb.py` & `premium-23.5.11.1/premium/models/xgb.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/nlp/metrics.py` & `premium-23.5.11.1/premium/nlp/metrics.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/nlp/net.py` & `premium-23.5.11.1/premium/nlp/net.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/nlp/nlp.py` & `premium-23.5.11.1/premium/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/preprocessing/ner.py` & `premium-23.5.11.1/premium/preprocessing/ner.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/pytorch/__init__.py` & `premium-23.5.11.1/premium/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/pytorch/data.py` & `premium-23.5.11.1/premium/pytorch/data.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/pytorch/tokenizer.py` & `premium-23.5.11.1/premium/pytorch/tokenizer.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/pytorch/trainer.py` & `premium-23.5.11.1/premium/pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/segment.py` & `premium-23.5.11.1/premium/segment.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/text_feature/bm25.py` & `premium-23.5.11.1/premium/text_feature/bm25.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/text_feature/sif.py` & `premium-23.5.11.1/premium/text_feature/sif.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/utils/__init__.py` & `premium-23.5.11.1/premium/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/utils/decorators.py` & `premium-23.5.11.1/premium/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium/zz.py` & `premium-23.5.11.1/premium/zz.py`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/premium.egg-info/SOURCES.txt` & `premium-23.5.11.1/premium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `premium-23.5.10.16/setup.py` & `premium-23.5.11.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codefast as cf 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="premium",
-    version=cf.generate_version(),
+    version="23.5.11.1",
     author="sK9xTFBq0H",
     author_email="google@gmail.com",
     description="Python AI toolkits",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     packages=setuptools.find_packages(),
```

