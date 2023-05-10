# Comparing `tmp/text2story-1.1.9.tar.gz` & `tmp/text2story-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2story-1.1.9.tar", last modified: Mon Dec 12 16:38:49 2022, max compression
+gzip compressed data, was "text2story-1.2.0.tar", last modified: Wed May 10 14:30:53 2023, max compression
```

## Comparing `text2story-1.1.9.tar` & `text2story-1.2.0.tar`

### file list

```diff
@@ -1,82 +1,92 @@
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2022-10-19 09:22:59.000000 text2story-1.1.9/LICENSE
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      335 2022-10-26 11:58:34.000000 text2story-1.1.9/MANIFEST.in
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8288 2022-12-12 16:38:49.314479 text2story-1.1.9/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     7784 2022-10-24 11:50:49.000000 text2story-1.1.9/README.md
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1378 2022-12-12 14:50:58.000000 text2story-1.1.9/pyproject.toml
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       38 2022-12-12 16:38:49.314479 text2story-1.1.9/setup.cfg
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       96 2022-10-19 09:13:05.000000 text2story-1.1.9/setup.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.310479 text2story-1.1.9/src/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.310479 text2story-1.1.9/src/text2story/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/__main__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.310479 text2story-1.1.9/src/text2story/annotators/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.310479 text2story-1.1.9/src/text2story/annotators/ALLENNLP/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.310479 text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.310479 text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.310479 text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/PropBankBr.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    21788 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/my_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/my_reader.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/ALLENNLP/preprocess.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/annotators/CUSTOMPT/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/CUSTOMPT/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/CUSTOMPT/event_model.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/CUSTOMPT/feature_extractor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/annotators/NLTK/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/NLTK/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/annotators/PY_HEIDELTIME/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2721 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/PY_HEIDELTIME/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/annotators/SPACY/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4362 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/annotators/SPACY/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/annotators/SPARKNLP/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2022-10-26 12:28:21.000000 text2story-1.1.9/src/text2story/annotators/SPARKNLP/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2108 2022-11-04 10:37:31.000000 text2story-1.1.9/src/text2story/annotators/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/brat2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/brat2viz/__init__.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/brat2viz/brat2drs/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/brat2viz/brat2drs/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17253 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/brat2viz/brat2drs/brat2drs.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/brat2viz/brat2drs/files_monitor.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/brat2viz/drs2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/brat2viz/drs2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/brat2viz/drs2viz/app.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2022-10-19 09:12:42.000000 text2story-1.1.9/src/text2story/brat2viz/drs2viz/parser.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4564 2022-11-04 13:39:56.000000 text2story-1.1.9/src/text2story/brat2viz/drs2viz/viz.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/core/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12106 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/core/annotator.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2667 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/core/entity_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      505 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/core/exceptions.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      529 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/core/link_structures.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17906 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/core/narrative.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2978 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/core/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/experiments/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/experiments/evaluation.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/experiments/metrics.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/experiments/run_experiments.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1618 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/experiments/stats.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/readers/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/readers/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/readers/read.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15986 2022-12-12 16:35:28.000000 text2story-1.1.9/src/text2story/readers/read_brat.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/readers/read_ecb.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/readers/read_framenet.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/readers/read_propbank.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      618 2022-12-12 14:40:22.000000 text2story-1.1.9/src/text2story/readers/token_corpus.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/readers/utils.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.314479 text2story-1.1.9/src/text2story/text2viz/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/text2viz/Text2Viz.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/text2viz/__init__.py
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2022-10-13 08:54:40.000000 text2story-1.1.9/src/text2story/text2viz/visualization.py
-drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2022-12-12 16:38:49.310479 text2story-1.1.9/src/text2story.egg-info/
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8288 2022-12-12 16:38:49.000000 text2story-1.1.9/src/text2story.egg-info/PKG-INFO
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2418 2022-12-12 16:38:49.000000 text2story-1.1.9/src/text2story.egg-info/SOURCES.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2022-12-12 16:38:49.000000 text2story-1.1.9/src/text2story.egg-info/dependency_links.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      243 2022-12-12 16:38:49.000000 text2story-1.1.9/src/text2story.egg-info/requires.txt
--rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       11 2022-12-12 16:38:49.000000 text2story-1.1.9/src/text2story.egg-info/top_level.txt
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.786344 text2story-1.2.0/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    33470 2023-05-10 14:09:15.000000 text2story-1.2.0/LICENSE
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      442 2023-05-10 14:09:15.000000 text2story-1.2.0/MANIFEST.in
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9809 2023-05-10 14:30:53.786344 text2story-1.2.0/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     8610 2023-05-10 14:09:15.000000 text2story-1.2.0/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      114 2023-05-10 14:09:15.000000 text2story-1.2.0/pyproject.toml
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1586 2023-05-10 14:30:53.786344 text2story-1.2.0/setup.cfg
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       70 2023-05-10 14:09:15.000000 text2story-1.2.0/setup.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.778344 text2story-1.2.0/text2story/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      757 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       67 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/__main__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.778344 text2story-1.2.0/text2story/annotators/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.778344 text2story-1.2.0/text2story/annotators/ALLENNLP/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.774344 text2story-1.2.0/text2story/annotators/ALLENNLP/Models/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.778344 text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.778344 text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      739 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       14 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/non_padded_namespaces.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1343 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   265058 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    10386 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/PropBankBr.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    25536 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13691 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/my_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    20375 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/my_reader.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6217 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/ALLENNLP/preprocess.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/annotators/CUSTOMPT/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14794 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/CUSTOMPT/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   371646 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/CUSTOMPT/crf_v2.1.joblib
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    15093 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/CUSTOMPT/event_model.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13972 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/CUSTOMPT/feature_extractor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/annotators/NLTK/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2948 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/NLTK/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/annotators/PY_HEIDELTIME/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2721 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/PY_HEIDELTIME/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/annotators/SPACY/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4362 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/SPACY/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/annotators/SPARKNLP/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9462 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/SPARKNLP/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2199 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/annotators/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/brat2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      548 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/__init__.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/brat2viz/brat2drs/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       37 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/brat2drs/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17253 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/brat2drs/brat2drs.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1059 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/brat2drs/files_monitor.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/brat2viz/drs2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/drs2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2428 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/drs2viz/app.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    13487 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/drs2viz/parser.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     4564 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/brat2viz/drs2viz/viz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/core/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    12126 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/core/annotator.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2667 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/core/entity_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      505 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/core/exceptions.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      529 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/core/link_structures.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    17906 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/core/narrative.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5281 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/core/utils.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.782344 text2story-1.2.0/text2story/experiments/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16454 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/experiments/evaluation.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14458 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/experiments/metrics.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1192 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/experiments/run_experiments.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1618 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/experiments/stats.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.786344 text2story-1.2.0/text2story/readers/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      380 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/fn-lirics.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)   312656 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/pb-vn2.json
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      547 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/read.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    22674 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/read_brat.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    16999 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/read_ecb.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     6081 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/read_framenet.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    11525 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/read_propbank.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1180 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/token_corpus.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     1221 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/utils.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      353 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/readers/vn-lirics.json
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.786344 text2story-1.2.0/text2story/select/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      121 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/select/README.md
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14728 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/select/bubble.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5159 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/select/event.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.786344 text2story-1.2.0/text2story/text2viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     5371 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/text2viz/Text2Viz.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       36 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/text2viz/__init__.py
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      699 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/text2viz/visualization.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.786344 text2story-1.2.0/text2story/viz/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)    14759 2023-05-10 14:09:15.000000 text2story-1.2.0/text2story/viz/bubble_tikz.py
+drwxrwxr-x   0 evelinamorim  (1000) evelinamorim  (1000)        0 2023-05-10 14:30:53.778344 text2story-1.2.0/text2story.egg-info/
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     9809 2023-05-10 14:30:53.000000 text2story-1.2.0/text2story.egg-info/PKG-INFO
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)     2483 2023-05-10 14:30:53.000000 text2story-1.2.0/text2story.egg-info/SOURCES.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-10 14:30:53.000000 text2story-1.2.0/text2story.egg-info/dependency_links.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)      224 2023-05-10 14:30:53.000000 text2story-1.2.0/text2story.egg-info/requires.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)       16 2023-05-10 14:30:53.000000 text2story-1.2.0/text2story.egg-info/top_level.txt
+-rw-rw-r--   0 evelinamorim  (1000) evelinamorim  (1000)        1 2023-05-10 14:11:36.000000 text2story-1.2.0/text2story.egg-info/zip-safe
```

### Comparing `text2story-1.1.9/LICENSE` & `text2story-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/PKG-INFO` & `text2story-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.1.9
+Version: 1.2.0
 Summary: It provides a framework to label a text according to the main elements of narrative (events, participants,time) and their relations
+Home-page: https://www.inesctec.pt/pt/centros/liaad
 Author: LIAAD lab
-Project-URL: Homepage, https://text2story project website/
-Keywords: narrative,nlp,annotation
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+License: GNU Public Licence
+Keywords: natural-language-processing,nlp,natural-language-understanding,deep-learning
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 # Text2Story main package
 The Text2Story main package contains the main classes and methods for the T2S pipeline: from text to formal representation to visualization or other representation.
 
 - **Relation to Brat2Viz**
 The Text2Story package is a generalization of Brat2Viz and should in fact contain all the funcionalities and variants of the T2S project output.
@@ -47,32 +59,36 @@
    ```bash
     pip install git+https://github.com/JMendes1995/py_heideltime.git
    ```
 4. Give tree parser of py_heideltime package permission to execute
    ```bash
     chmod +x $(VENV_HOME)/lib/python3.8/site-packages/py_heideltime/Heideltime/TreeTaggerLinux/bin/tree-tagger
    ```
-5. Installation of the text2story package.
+5. Installation of plantuml package, which is used in the visualization.
+   ```
+   pip install git+https://github.com/SamuelMarks/python-plantuml#egg=plantuml
+   ```
+6. Installation of the text2story package.
    ```bash
      python -m pip install text2story
    ```
 
 The following steps are optional to use the text2story package, but essential to run the our TLDR Python notebook locally (https://bit.ly/3s36Bxf).
 
-6. Adding virtual enviroment to Jupyter Notebook.
+7. Adding virtual enviroment to Jupyter Notebook.
    ```bash
       python3.8 -m pip install --user ipykernel
    ```
 
-7. Adding your virtual enviroment to Jupyter.
+8. Adding your virtual enviroment to Jupyter.
    ```bash
       python -m ipykernel install --user --name=venv
    ```
 
-8. Changing the kernel in the Jupyter, by cliking in Kernel -> Change Kernel -> (kernel name).
+9. Changing the kernel in the Jupyter, by cliking in Kernel -> Change Kernel -> (kernel name).
 
 
 
 ### Usage
 
 
 ```python
@@ -91,16 +107,25 @@
 
 doc.extract_events('allennlp') # Extraction of events with allennlp tool
 doc.extract_semantic_role_link('allennlp') # Extraction of semantic role links with all tools (should be done after extracting events since most semantic relations are between an actor and an event)
 
 doc.ISO_annotation('annotations.ann') # Outputs ISO annotation in .ann format (txt) in a file called 'annotations.ann', which is a standard of BRAT annotation tool
 
 
-## Structure
 ```
+
+## Examples: Python Notebooks
+
+A  basic notebook that teaches how to use our reader of annotations, which format is assumed is to be in the BRAT format is in the following link: [How to read a BRAT file](https://colab.research.google.com/drive/1_jc6SJNAdWMYBMVlGPldFDmGNg4gFUCs?usp=sharing).
+
+There is the TLDR Python notebook, which extracts the main narrative elements and draw an MSC visulization:  [Too Long Didn't Read Tutorial](https://bit.ly/3s36Bxf).
+
+Finally, there is a notebook that shows how to produce a bubble visualization: [How To: Bubble Visualization](https://colab.research.google.com/drive/1V2DCuP1qAlwUXThTKNUnZ98WxARZXC_v?usp=sharing).
+
+## Structure
 .
 │   README.md
 |   env.yml
 │   requirements.txt
 |   pyproject.toml
 |   MANIFEST.in
 |   LICENSE
```

### Comparing `text2story-1.1.9/README.md` & `text2story-1.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -33,32 +33,36 @@
    ```bash
     pip install git+https://github.com/JMendes1995/py_heideltime.git
    ```
 4. Give tree parser of py_heideltime package permission to execute
    ```bash
     chmod +x $(VENV_HOME)/lib/python3.8/site-packages/py_heideltime/Heideltime/TreeTaggerLinux/bin/tree-tagger
    ```
-5. Installation of the text2story package.
+5. Installation of plantuml package, which is used in the visualization.
+   ```
+   pip install git+https://github.com/SamuelMarks/python-plantuml#egg=plantuml
+   ```
+6. Installation of the text2story package.
    ```bash
      python -m pip install text2story
    ```
 
 The following steps are optional to use the text2story package, but essential to run the our TLDR Python notebook locally (https://bit.ly/3s36Bxf).
 
-6. Adding virtual enviroment to Jupyter Notebook.
+7. Adding virtual enviroment to Jupyter Notebook.
    ```bash
       python3.8 -m pip install --user ipykernel
    ```
 
-7. Adding your virtual enviroment to Jupyter.
+8. Adding your virtual enviroment to Jupyter.
    ```bash
       python -m ipykernel install --user --name=venv
    ```
 
-8. Changing the kernel in the Jupyter, by cliking in Kernel -> Change Kernel -> (kernel name).
+9. Changing the kernel in the Jupyter, by cliking in Kernel -> Change Kernel -> (kernel name).
 
 
 
 ### Usage
 
 
 ```python
@@ -77,16 +81,25 @@
 
 doc.extract_events('allennlp') # Extraction of events with allennlp tool
 doc.extract_semantic_role_link('allennlp') # Extraction of semantic role links with all tools (should be done after extracting events since most semantic relations are between an actor and an event)
 
 doc.ISO_annotation('annotations.ann') # Outputs ISO annotation in .ann format (txt) in a file called 'annotations.ann', which is a standard of BRAT annotation tool
 
 
-## Structure
 ```
+
+## Examples: Python Notebooks
+
+A  basic notebook that teaches how to use our reader of annotations, which format is assumed is to be in the BRAT format is in the following link: [How to read a BRAT file](https://colab.research.google.com/drive/1_jc6SJNAdWMYBMVlGPldFDmGNg4gFUCs?usp=sharing).
+
+There is the TLDR Python notebook, which extracts the main narrative elements and draw an MSC visulization:  [Too Long Didn't Read Tutorial](https://bit.ly/3s36Bxf).
+
+Finally, there is a notebook that shows how to produce a bubble visualization: [How To: Bubble Visualization](https://colab.research.google.com/drive/1V2DCuP1qAlwUXThTKNUnZ98WxARZXC_v?usp=sharing).
+
+## Structure
 .
 │   README.md
 |   env.yml
 │   requirements.txt
 |   pyproject.toml
 |   MANIFEST.in
 |   LICENSE
```

### Comparing `text2story-1.1.9/src/text2story/__init__.py` & `text2story-1.2.0/text2story/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt` & `text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/Vocabulary/labels.txt`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json` & `text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/config.json`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt` & `text2story-1.2.0/text2story/annotators/ALLENNLP/Models/srl-pt_bertimbau-base/linear_layer.pt`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/ALLENNLP/PropBankBr.py` & `text2story-1.2.0/text2story/annotators/ALLENNLP/PropBankBr.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/ALLENNLP/__init__.py` & `text2story-1.2.0/text2story/annotators/ALLENNLP/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,53 +9,61 @@
 import pandas as pd
 import numpy as np
 from itertools import zip_longest
 
 import nltk
 from nltk.tokenize import sent_tokenize
 
+from text2story.annotators.ALLENNLP import my_model,my_reader
+from text2story.core.utils import bsearch_tuplelist
+
 from allennlp.predictors.predictor import Predictor
 from allennlp.models.archival import load_archive
-from text2story.annotators.ALLENNLP import my_model,my_reader
 from allennlp_models.structured_prediction.predictors import SemanticRoleLabelerPredictor
 from allennlp.models import Model
 from overrides import overrides
 from typing import List, Iterator, Optional
 from nltk import tokenize, download
 download('punkt')
 
 from allennlp.data import DatasetReader, Instance
 from allennlp.data.vocabulary import Vocabulary
 from allennlp.common.util import JsonDict
 
+import spacy
+
 import urllib.request
 import os
 import torch
 from shutil import copyfile
+import json
+
 
 ### Global Variables ###
 
 SRL_TYPE_MAPPING = {
     "TMP": "time",
     "LOC": "location",
     "ADV": "theme",  # Adverbial
     "MNR": "manner",
     "CAU": "cause",
+    "PRP":"cause",
     "EXT": "theme",  # should be attribute -> changed for compatibility
     "DIS": "theme",  # connection of two expressions -> should be theme -> changed for compatibility
     "PNC": "purpose",
-    "PRP": "purpose",
+    "PR": "purpose",
     "NEG": "theme",  # should be attribute -> changed for compatibility | NEG = negation
     "DIR": "path",  # should be setting -> changed for compatibility
     "MOD": "instrument",  # MOD = Modal
     "PRD": "theme",  # Secondary predicate -> should be attribute -> changed for compatibility
     "ADJ": "theme",
     "COM": "agent",  # COM = Comitative -> used to express accompaniment
     "GOL": "goal",  # GOL = goal
-    "REC": "instrument"  # REC = reciprocal
+    "REC": "instrument",  # REC = reciprocal
+    "PAS": "passive" # passive verb
 }
 
 pipeline = {}
 
 ### Portuguese SRL predictor ###
 
 @Predictor.register("predictor_pt")
@@ -177,14 +185,20 @@
         urllib.request.urlretrieve("https://storage.googleapis.com/allennlp-public-models/structured-prediction-srl-bert.2020.12.15.tar.gz",\
                 srl_path)
 
 
     pipeline["srl_en"] = Predictor.from_path(srl_path)
     # regular expression to capture SRL tags
     pipeline["srl_re_tags"] = r".*[ARG][0-9]|ARGM"
+    pipeline["ARGM_STR"] = "ARGM"
+
+    if not(spacy.util.is_package('en_core_web_lg')):
+        spacy.cli.download('en_core_web_lg')
+
+    pipeline['en'] = spacy.load('en_core_web_lg')
 
 def load_pt():
 
     current_path = os.path.dirname(os.path.abspath(__file__))
 
     srl_pt_model_path = os.path.join(current_path, "cache")
     srl_pt_model_path = os.path.join(srl_pt_model_path, "srl-pt_bertimbau-base")
@@ -197,14 +211,21 @@
     pipeline["srl_pt"] = Predictor.from_archive(
             archive, "predictor_pt", dataset_reader_to_load="train"
         )
 
     # regular expression to capture SRL tags
     pipeline["srl_re_tags"] = r".*[A][0-9]|AM"
 
+    # since allennlp does not have NER, download the spacy model
+    if not(spacy.util.is_package('pt_core_news_lg')):
+        spacy.cli.download('pt_core_news_lg')
+    pipeline["ARGM_STR"] = "B-AM"
+
+    pipeline["pt"] =  spacy.load('pt_core_news_lg')
+
 def _normalize_sent_tags(sentence_df):
     """
     Normalize the frames retrieved from the SRL from one sentence.
     Each word must have only one label.
 
     @param sentence_df: DataFrame of the SRL each column is a word from the sentence and each row is the results of SRL
     for one frame.
@@ -347,24 +368,26 @@
     @return: Dict list with the actor, its semantic role and the its character position span in the text
 
     @note: CAN MALFUNCTION IF SRL DOES NOT FIND FRAMES IN EVERY SENTENCE.
     The char positions are checked in the entire text, if there is a word before in a sentence not recognized by the SRL
     it will malfunction slightly (give wrong position values).
     """
     result_list = []
+    ARGM_STR = pipeline["ARGM_STR"]
     for actor in srl_by_token["actor"].unique():
         rows = srl_by_token[srl_by_token["actor"] == actor]
         tags = rows["tag"]
         if actor.startswith("EVENT"):
             sem_role_type = "EVENT"
-        elif any("ARGM" in tag for tag in tags):
-            argm_tags = [tag for tag in tags if "ARGM" in tag]
+        elif any(ARGM_STR in tag for tag in tags):
+            argm_tags = [tag for tag in tags if ARGM_STR in tag]
+            #print("-->",argm_tags[0].split("-")[-1])
             sem_role_type = SRL_TYPE_MAPPING[argm_tags[0].split("-")[-1]]
         else:
-            sem_role_type = "THEME"
+            sem_role_type = "PARTICIPANT"
 
         char_spans = []
         for token in rows.index:
             char_offset = text.find(token, char_offset)
             char_spans.append(char_offset)
             char_offset += len(token)
 
@@ -464,15 +487,15 @@
     and still be considered part of the same event. number_of_args = event_threshold - 1
 
     @return: df_by_actor -> Pandas DataFrame with each actor, their semantic roles and character spans
     character_offset -> The current character position offset in the full text
     """
     # 2. Remove words out of vocabulary in every frame #
     oov_mask = []
-    for name, values in sentence_df.iteritems():
+    for name, values in sentence_df.items():
         oov_mask.append(any(~(values == "O")))
     sentence_df = sentence_df.loc[:, oov_mask]
     sentence_df = sentence_df.apply(lambda x: x.sort_values(ascending=False).values)  # Begin tags in the end always
 
     # 3. Normalize SRL tags for each word in the sentence dataframe #
     normalized_tags, begin_tags = _normalize_sent_tags(sentence_df)
 
@@ -492,14 +515,92 @@
     }, index=sentence_df.columns)
 
     # 6. Find semantic roles and character spans for each actor in the sentence #
     df_by_actor, character_offset = _srl_by_actor(df, text, char_offset)
 
     return df_by_actor, character_offset
 
+def get_participant_tags(text, participant_lst, lang):
+    """
+    it adds POS tags and NER tags to the participant list
+
+    @param text: the original text to be processed as narrative
+    @param list[tuple[int,int]]: A list of character span of the participant
+    candidates
+    Returns
+    ------
+    list[tuple[tuple[int, int], str, str]]
+       a list of participants of narratives, where the first is the character
+       span of that participant, the second elements is the POS tag, anf third
+       element is the NER tag, if it is a entity
+    """
+    participant_lst = sorted(participant_lst, key=lambda x:x[0])
+    tagged_participants = {}
+
+    doc = pipeline[lang](text)
+
+    for tok in doc:
+        pos = bsearch_tuplelist(tok.idx, participant_lst)
+        if pos != -1:
+            # only update the tag value with the lexical head of the
+            # participant
+            if pos not in tagged_participants:
+                offset_participant = participant_lst[pos]
+                if tok.ent_type_ == '':
+                    tagged_participants[pos] = (offset_participant, tok.pos_, 'UNDEF')
+                else:
+                    tagged_participants[pos] = (offset_participant, tok.pos_,tok.ent_type_.lower().capitalize())
+
+    tagged_participants_lst = []
+    # it is possible that some participant was not found by the bsearch?
+    for idx in range(len(participant_lst)):
+        if idx not in tagged_participants:
+            tagged_participants_lst.append((participant_lst[idx],"UNDEF","UNDEF"))
+        else:
+            tagged_participants_lst.append(tagged_participants[idx])
+
+    return tagged_participants_lst
+
+def extract_actors(lang, text):
+    """
+    Main function that applies the SRL pipeline to extract participant entities from each sentence.
+
+    @param lang: The language of the text
+    @param text: The full text to be annotated
+    Returns
+    -------
+    list[tuple[tuple[int, int], str, str]]
+        the list of actors identified where each actor is represented by a tuple
+    """
+    # 1. DATAFRAME WITH THE SRL RESULTS OF EVERY FRAME FOR EACH SENTENCE IN THE TEXT #
+    dfs_by_sent = _make_srl_df(lang, text)
+
+    # FIND EVENTS - PIPELINE #
+    character_offset, srl_actors_list = 0, []
+    for sent_df in dfs_by_sent:
+        df_by_actor, character_offset = _srl_pipeline(sent_df, text, character_offset, verb_tags=["B-V", "I-V"],
+                                                      event_threshold=2)
+
+        srl_actors_list.append(df_by_actor)
+
+
+    srl_actors_list = [item for sublist in srl_actors_list for item in sublist]  # flatten list
+    srl_df = pd.DataFrame(srl_actors_list)
+    if len(srl_df) == 0:
+        return []
+
+    participants_df = srl_df[srl_df["sem_role_type"] == "PARTICIPANT"]
+    participants_lst = participants_df["char_span"].values.tolist()
+
+    # TODO: these participants still dont have POS and NER tags
+    participants_tagged_lst = get_participant_tags(text, participants_lst, lang)
+    #participants_lst = [ (p, "NOUN", "Per") for p in participants_lst]
+
+    return participants_tagged_lst
+
 
 def extract_events(lang, text):
     """
     Main function that applies the SRL pipeline to extract event entities from each sentence.
     Joins every event actor from each sentence in the text.
 
     @param lang: The language of the text
```

### Comparing `text2story-1.1.9/src/text2story/annotators/ALLENNLP/my_model.py` & `text2story-1.2.0/text2story/annotators/ALLENNLP/my_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/ALLENNLP/my_reader.py` & `text2story-1.2.0/text2story/annotators/ALLENNLP/my_reader.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/ALLENNLP/preprocess.py` & `text2story-1.2.0/text2story/annotators/ALLENNLP/preprocess.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/CUSTOMPT/__init__.py` & `text2story-1.2.0/text2story/annotators/CUSTOMPT/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/CUSTOMPT/crf_v2.1.joblib` & `text2story-1.2.0/text2story/annotators/CUSTOMPT/crf_v2.1.joblib`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/CUSTOMPT/event_model.py` & `text2story-1.2.0/text2story/annotators/CUSTOMPT/event_model.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/CUSTOMPT/feature_extractor.py` & `text2story-1.2.0/text2story/annotators/CUSTOMPT/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/NLTK/__init__.py` & `text2story-1.2.0/text2story/annotators/NLTK/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/PY_HEIDELTIME/__init__.py` & `text2story-1.2.0/text2story/annotators/PY_HEIDELTIME/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/SPACY/__init__.py` & `text2story-1.2.0/text2story/annotators/SPACY/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/SPARKNLP/__init__.py` & `text2story-1.2.0/text2story/annotators/SPARKNLP/__init__.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/annotators/__init__.py` & `text2story-1.2.0/text2story/annotators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from text2story.core.exceptions import InvalidTool
 from text2story.annotators import SPACY, NLTK, SPARKNLP, PY_HEIDELTIME, ALLENNLP, CUSTOMPT
 
 sys.path.insert(0, Path(__file__).parent)
 
-ACTOR_EXTRACTION_TOOLS = ['spacy', 'nltk', 'sparknlp']
+ACTOR_EXTRACTION_TOOLS = ['spacy', 'nltk', 'sparknlp','allennlp']
 TIME_EXTRACTION_TOOLS = ['py_heideltime']
 EVENT_EXTRACTION_TOOLS = ['allennlp','custompt']
 OBJECTAL_LINKS_RESOLUTION_TOOLS = ['allennlp']
 SEMANTIC_ROLE_LABELLING_TOOLS = ['allennlp']
 
 
 def load(lang):
@@ -42,14 +42,16 @@
 
 def extract_actors(tool, lang, text):
 
     if tool == 'spacy':
         return SPACY.extract_actors(lang, text)
     elif tool == 'nltk':
         return NLTK.extract_actors(lang, text)
+    elif tool == 'allennlp':
+        return ALLENNLP.extract_actors(lang, text)
     #elif tool == 'sparknlp':
     #    return SPARKNLP.extract_actors(lang, text)
 
     raise InvalidTool
 
 
 def extract_times(tool, lang, text, publication_time):
```

### Comparing `text2story-1.1.9/src/text2story/brat2viz/brat2drs/brat2drs.py` & `text2story-1.2.0/text2story/brat2viz/brat2drs/brat2drs.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/brat2viz/brat2drs/files_monitor.py` & `text2story-1.2.0/text2story/brat2viz/brat2drs/files_monitor.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/brat2viz/drs2viz/app.py` & `text2story-1.2.0/text2story/brat2viz/drs2viz/app.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/brat2viz/drs2viz/parser.py` & `text2story-1.2.0/text2story/brat2viz/drs2viz/parser.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/brat2viz/drs2viz/viz.py` & `text2story-1.2.0/text2story/brat2viz/drs2viz/viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/core/annotator.py` & `text2story-1.2.0/text2story/core/annotator.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,28 +81,31 @@
         # If no tool specified, use all
         if nr_tools == 0:
             self.tools = ACTOR_EXTRACTION_TOOLS
             nr_tools = len(self.tools)
 
         # Gather the annotations made by the tools specified and combine the results
         annotations = []
+        idxs = []
         for tool in self.tools:
             annotations.append(extract_actors(tool, lang, text))
 
         final_annotation = []
 
         idxs = [0] * nr_tools # Current actor position from each tool
 
+
         while not(all([len(annotations[i]) == idxs[i] for i in range(nr_tools)])): # We finish when we consumed every actor identified by every tool
             tool_id = -1
             tool_id_start_char_offset = len(text) # len(self.text) acting as infinite
 
             # Get the next entity chunk to be gather (the one with the lowest start character span)
             for i in range(nr_tools):
                 if idxs[i] < len(annotations[i]):
+
                     current_actor = annotations[i][idxs[i]]
                     current_actor_start_character_span = current_actor[0][0]
 
                     if current_actor_start_character_span < tool_id_start_char_offset:
                         tool_id = i
                         tool_id_start_char_offset = current_actor_start_character_span
```

### Comparing `text2story-1.1.9/src/text2story/core/entity_structures.py` & `text2story-1.2.0/text2story/core/entity_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/core/link_structures.py` & `text2story-1.2.0/text2story/core/link_structures.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/core/narrative.py` & `text2story-1.2.0/text2story/core/narrative.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/experiments/evaluation.py` & `text2story-1.2.0/text2story/experiments/evaluation.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/experiments/metrics.py` & `text2story-1.2.0/text2story/experiments/metrics.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/experiments/run_experiments.py` & `text2story-1.2.0/text2story/experiments/run_experiments.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/experiments/stats.py` & `text2story-1.2.0/text2story/experiments/stats.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/readers/read.py` & `text2story-1.2.0/text2story/readers/read.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/readers/read_brat.py` & `text2story-1.2.0/text2story/readers/read_brat.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,54 @@
 import sys
 from pathlib import Path
 
 from . import read
 from . import token_corpus
 
 import spacy
+from spacy.tokenizer import Tokenizer
+from spacy.lang.char_classes import ALPHA, ALPHA_LOWER, ALPHA_UPPER, CONCAT_QUOTES, LIST_ELLIPSES, LIST_ICONS, HYPHENS
+from spacy.util import compile_infix_regex
+
 import re
+import copy
+import numpy as np
+
 
 # regular expression of an integer number
 NUMBER_RE = re.compile("^[0-9]*[1-9][0-9]*$")
 LINK_TYPES = ["SEMROLE", "SRLINK"]
 
 LINK_TYPES = ["SEMROLE","SRLINK"]
 
+infix_re = re.compile(r'[-]')
+
+
+def custom_tokenizer(nlp):
+    infixes = (
+        LIST_ELLIPSES
+        + LIST_ICONS
+        + [
+            r"(?<=[0-9])[+\-\*^](?=[0-9-])",
+            r"(?<=[{al}{q}])\.(?=[{au}{q}])".format(
+                al=ALPHA_LOWER, au=ALPHA_UPPER, q=CONCAT_QUOTES
+            ),
+            r"(?<=[{a}]),(?=[{a}])".format(a=ALPHA),
+            r"(?<=[{a}])(?:{h})(?=[{a}])".format(a=ALPHA, h=HYPHENS),
+            r"(?<=[{a}0-9])[:<>=/](?=[{a}])".format(a=ALPHA),
+        ]
+    )
+
+    infix_re = compile_infix_regex(infixes)
+
+    return Tokenizer(nlp.vocab, prefix_search=nlp.tokenizer.prefix_search,
+                                suffix_search=nlp.tokenizer.suffix_search,
+                                infix_finditer=infix_re.finditer,
+                                token_match=nlp.tokenizer.token_match,
+                                rules=nlp.Defaults.tokenizer_exceptions)
 
 class ReadBrat(read.Read):
     """
       Reader to brat file annotations and their text files
     """
 
     def __init__(self):
@@ -25,14 +57,18 @@
         Load spacy model to read process brat files. Also
         store the files processed.
         """
         if not(spacy.util.is_package('pt_core_news_lg')):
             spacy.cli.download('pt_core_news_lg')
 
         self.nlp = spacy.load("pt_core_news_lg")
+
+
+        self.nlp.tokenizer = custom_tokenizer(self.nlp)
+
         self.file_lst = []
         self.ann_ref = {}
 
     def toColumn(self, data_dir, output_dir):
         """
         Convert a set of files to column format, similar to Conll
 
@@ -307,103 +343,263 @@
                     self.file_lst.append(fullname + ".txt")
 
                     if len(token_lst) > 0:
                         data_tokens.append(token_lst)
 
         return data_tokens
 
+    def extract_token_corpus(self, doc, ann_idx, ann, ann_ref):
+        """
+        Build a list of tokens using TokenCorpus object. It uses 
+        a document of spacy.Document type (doc) and a list of indexes.
+
+        ann_idx is a maps a 2-tuple integer to a list of annotation. Regarfing, 
+        the 2-tuple, the first element  is the start character offset of 
+        an annotated token in the 
+        raw text of the document, and the second element is end of the character 
+        offset of an annotated token.
+
+        ann is a dictionary that maps a 2-tuple of indexes to a list of 
+        the annotation of the given span indexes. 
+
+        ann_ref is a dictionary that maps a reference (i.e. an id of an annotation 
+        assigned by BRAT) to the attribute list of an annotation span
+        """
+        count = 0
+        token_lst = []
+        ref2tok = {}
+
+    
+        sent_id = -1
+        for tok_idx, tok in enumerate(doc):
+
+            if tok.is_sent_start:
+                sent_id += 1
+
+            
+            mytok = token_corpus.TokenCorpus()
+            mytok.id = count
+            mytok.text = tok.text
+            mytok.lemma = tok.lemma_
+            mytok.pos = tok.pos_
+            mytok.dep = tok.dep_
+            mytok.head = tok.head.text
+            mytok.head_pos = tok.head.pos_
+            mytok.head_lemma = tok.head.lemma_
+            mytok.offset = tok.idx
+            mytok.sent_id = sent_id
+
+
+
+            ans = self.search_all_idx(tok.idx, ann_idx)
+
+            # TODO: it is necessary perform a more efficient search
+            # a possible subtoken annotation
+            # perform more than one search, and build a list of id's
+            ans_sub = self.search_subtoken(tok.idx, tok.idx + len(tok.text), \
+                        ann_idx)
+
+            ans = ans.union(ans_sub)
+
+            if len(ans) != 0:
+                # annotations in token
+                # a token can be annotated twice, and besides that,
+                # can be a part of a span annotation..The iteration in ans
+                # tries to get the span annotations in one token, and the 
+                # iteration in ann[(t0,t1)] bellow tries to get several annotations
+                # in only one token
+                ref_lst_tok = set()
+                for idx in ans:
+                    (t0, t1) = ann_idx[idx]
+
+
+                    for ref, ann_type, elems in ann[(t0, t1)]:
+
+                        mytok.attr.append((ann_type, ann_ref[ref]))
+                        mytok.id_ann.append(ref) 
+                        # all the annotations ids that a token can be assigned
+                        ref_lst_tok.add(ref)
+
+
+                # now update the mapping of references to tokens with
+                # the token object that was build in this iteration
+                for ref in ref_lst_tok:
+                    if ref in ref2tok:
+                        ref2tok[ref].append(mytok)
+                    else:
+                        ref2tok[ref] = [mytok]
+
+            token_lst.append(mytok)
+
+            count += 1
+
+        return token_lst, ref2tok
+
+    # TODO: refactor this method. It is a very long and confusing method
     def process_file(self, data_file):
         """
         It reads only one file of annotation and text, then returns
         the processed tokens as TokenCorpus type
 
         @param string: path of data to gather and process
 
         @return [TokenCorpus]: a list of tokens
         """
 
         file_ann = "%s.ann" % data_file
         file_txt = "%s.txt" % data_file
 
-        token_lst = []
+
         if not os.path.exists(file_txt) or not os.path.exists(file_ann):
-            return token_lst
+            return []
 
         ann = {}  # the index is the offset of the annotation
         ann_ref = {}  # annotation by reference
+        ann_rel = {} # annotation by relation
+
+        # the pattern of a reference for an argument of a relation
+        ARG_REL = re.compile("T\d+") 
 
         with open(file_ann, "r") as fd:
+            
             for line in fd:
                 line_toks = line.split()
-                # TODO: currently only read event annotations
                 if line[0] != '#' and line[0] == 'T':
 
                     # ann[offset start] = (ref, ann_type, value_str)
                     if ';' in line_toks[3]:
                         # this situation is when the annotation of th event
                         # is two segments not adjacents
                         tmp = line_toks[3].split(';')
-                        ann[(int(line_toks[2]), int(tmp[0]))] = (line_toks[0], line_toks[1], line_toks[5:])
-                        ann[(int(tmp[1]), int(line_toks[4]))] = (line_toks[0], line_toks[1], line_toks[5:])
+                        ann[(int(line_toks[2]), int(tmp[0]))] = [(line_toks[0], line_toks[1], line_toks[5:])]
+                        ann[(int(tmp[1]), int(line_toks[4]))] = [(line_toks[0], line_toks[1], line_toks[5:])]
+                        ann_ref[line[0]] = (
+                            [(int(line_toks[2]), int(tmp[0])), (int(tmp[1]), int(line_toks[4]))], [])
+
+
                         ann_ref[line_toks[0]] = {}
-                        #ann_ref[line_toks[0]] = (
-                        #    [(int(line_toks[2]), int(tmp[0])), (int(tmp[1]), int(line_toks[4]))], [])
                     else:
                         if NUMBER_RE.match(line_toks[2]):
-                            ann[(int(line_toks[2]), int(line_toks[3]))] = (
-                                line_toks[0], line_toks[1], line_toks[4:])
-                            #ann_ref[line_toks[0]] = ([(int(line_toks[2]), int(line_toks[3]))], [])
+
+                            offset_start, offset_end = int(line_toks[2]), int(line_toks[3])
+
+                            if (offset_start, offset_end) in ann:
+                                ann[(offset_start, offset_end)].append((line_toks[0], line_toks[1], line_toks[4:]))
+                            else:
+                                ann[(offset_start, offset_end)] = [(line_toks[0], line_toks[1], line_toks[4:])]
+                                
                             ann_ref[line_toks[0]] = {}
+                elif line[0] == 'R':
+                    rel_id = line_toks[0]
+
+                    rel_type = line_toks[1]
+                    ref_lst = ARG_REL.findall(line)
+
+                    if len(ref_lst) > 1:
+
+                        ref1 = ref_lst[0]
+                        ref2 = ref_lst[1]
+
+                        if ref1 in ann_rel:
+                            ann_rel[ref1].append((rel_id, rel_type, ref2, "arg2"))
+                        else:
+                            ann_rel[ref1] = [(rel_id, rel_type, ref2,"arg2")]
+
+                        if ref2 in ann_rel:
+                            ann_rel[ref2].append((rel_id, rel_type, ref1,"arg1"))
+                        else:
+                            ann_rel[ref2] = [(rel_id, rel_type, ref1,"arg1")]
+
+                    else:
+                        print("Warning: There is a relation with only one argument.")
+
+
+
                 elif line[0] == 'A':
+
                     ref = line_toks[2]
                     if ref in ann_ref:
                         #ann_ref[ref][1].append((line[1], line[3]))
                         ann_ref[ref][line_toks[1]] = line_toks[3]
                     else:
                         ann_ref[ref] = {line_toks[1]:line_toks[3]}
 
         idx_lst = ann.keys()
 
         idx_lst = sorted(idx_lst, key=lambda elem: elem[0])
 
+        # a mapping between ref and Tok object
+        # the use it to point to the tokens that it own relations
+        ref2tok = {} 
+        token_lst = []
+
         with open(file_txt, "r") as fd:
 
             doc = self.nlp(fd.read())
-            count = 0
+            token_lst, ref2tok = self.extract_token_corpus(doc, idx_lst, ann, ann_ref)
 
-            for tok in doc:
 
-                mytok = token_corpus.TokenCorpus()
-                mytok.id = count
-                mytok.text = tok.text
-                mytok.lemma = tok.lemma_
-                mytok.pos = tok.pos_
-                mytok.dep = tok.dep_
-                mytok.head = tok.head.text
-                mytok.head_pos = tok.head.pos_
-                mytok.head_lemma = tok.head.lemma_
-                mytok.offset = tok.idx
-
-                ans = self.search_idx(tok.idx, idx_lst)
-                if ans != -1:
-                    # annotations in token
-                    (t0, t1) = idx_lst[ans]
-                    ref, ann_type, _ = ann[(t0, t1)]
+        # update relation field for each token
+        # each relation field is a list of TokenRelation object, which 
+        # points to a TokenCorpus and specifies the type of relation
+        for mytok in token_lst:
 
-                    # TODO: more detail of the annotation in ann_ref
+            if mytok.id_ann != []:
 
-                    mytok.ann = ann_type
-                    mytok.attr = ann_ref[ref]
+                for ref  in mytok.id_ann:
 
-                token_lst.append(mytok)
+                    if ref in ann_rel: # if the current token has any relation, then...
+
+                        # the relation for the reference ref
+                        for rel_id, rel_type, ref_arg,argn in ann_rel[ref]:
+                            rel_obj = token_corpus.TokenRelation(rel_id, ref2tok[ref_arg], rel_type, argn, ref_arg)
+                            mytok.relations.append(rel_obj)
 
-                count += 1
 
         return token_lst
 
+    def search_all_idx(self, idx, idx_lst):
+        """
+        Since a token can be annotated with multiple id's, it is necessary 
+        to perform multiple search for each one of these id's.
+        """
+
+        all_idx_lst = set()
+
+        copy_idx_lst = [e for e in idx_lst]
+        
+        while True:
+
+            ans = self.search_idx(idx, copy_idx_lst)
+            if ans == -1:
+                return all_idx_lst
+            else:
+                # update index according to the position
+                # in the idx_lst 
+                elem = copy_idx_lst[ans]
+                copy_idx_lst.pop(ans)
+                if len(idx_lst) > 0:
+                    # can I afford such expensive operation
+                    # since few of them are possible performed?
+                    ans = idx_lst.index(elem)
+
+                all_idx_lst.add(ans)
+
+
+    def search_subtoken(self, tok_start, tok_end, idx_lst):
+
+        ans = set()
+
+        for pos, (start, end) in enumerate(idx_lst):
+            
+            if start >= tok_start and end <= tok_end:
+                ans.add(pos)
+
+        return ans
+
     def search_idx(self, idx, idx_lst):
         """
         it searches for tuples (t0, t1) in idx_lst where idx >= t0 and idx <= t1
 
         @param integer: an index
         @param [(integer,integer)]: a list of index
 
@@ -419,15 +615,15 @@
         while b <= e:
             (t0, t1) = idx_lst[m]
 
             if idx == t0:
                 pos = m
                 break
             elif idx > t0:
-                if idx > t1:
+                if idx >= t1:
                     b = m + 1
                 else:
                     pos = m
                     break
             else:
                 e = m - 1
```

### Comparing `text2story-1.1.9/src/text2story/readers/read_ecb.py` & `text2story-1.2.0/text2story/readers/read_ecb.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/readers/read_framenet.py` & `text2story-1.2.0/text2story/readers/read_framenet.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/readers/read_propbank.py` & `text2story-1.2.0/text2story/readers/read_propbank.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/readers/utils.py` & `text2story-1.2.0/text2story/readers/utils.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/text2viz/Text2Viz.py` & `text2story-1.2.0/text2story/text2viz/Text2Viz.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story/text2viz/visualization.py` & `text2story-1.2.0/text2story/text2viz/visualization.py`

 * *Files identical despite different names*

### Comparing `text2story-1.1.9/src/text2story.egg-info/PKG-INFO` & `text2story-1.2.0/text2story.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 Metadata-Version: 2.1
 Name: text2story
-Version: 1.1.9
+Version: 1.2.0
 Summary: It provides a framework to label a text according to the main elements of narrative (events, participants,time) and their relations
+Home-page: https://www.inesctec.pt/pt/centros/liaad
 Author: LIAAD lab
-Project-URL: Homepage, https://text2story project website/
-Keywords: narrative,nlp,annotation
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+License: GNU Public Licence
+Keywords: natural-language-processing,nlp,natural-language-understanding,deep-learning
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 # Text2Story main package
 The Text2Story main package contains the main classes and methods for the T2S pipeline: from text to formal representation to visualization or other representation.
 
 - **Relation to Brat2Viz**
 The Text2Story package is a generalization of Brat2Viz and should in fact contain all the funcionalities and variants of the T2S project output.
@@ -47,32 +59,36 @@
    ```bash
     pip install git+https://github.com/JMendes1995/py_heideltime.git
    ```
 4. Give tree parser of py_heideltime package permission to execute
    ```bash
     chmod +x $(VENV_HOME)/lib/python3.8/site-packages/py_heideltime/Heideltime/TreeTaggerLinux/bin/tree-tagger
    ```
-5. Installation of the text2story package.
+5. Installation of plantuml package, which is used in the visualization.
+   ```
+   pip install git+https://github.com/SamuelMarks/python-plantuml#egg=plantuml
+   ```
+6. Installation of the text2story package.
    ```bash
      python -m pip install text2story
    ```
 
 The following steps are optional to use the text2story package, but essential to run the our TLDR Python notebook locally (https://bit.ly/3s36Bxf).
 
-6. Adding virtual enviroment to Jupyter Notebook.
+7. Adding virtual enviroment to Jupyter Notebook.
    ```bash
       python3.8 -m pip install --user ipykernel
    ```
 
-7. Adding your virtual enviroment to Jupyter.
+8. Adding your virtual enviroment to Jupyter.
    ```bash
       python -m ipykernel install --user --name=venv
    ```
 
-8. Changing the kernel in the Jupyter, by cliking in Kernel -> Change Kernel -> (kernel name).
+9. Changing the kernel in the Jupyter, by cliking in Kernel -> Change Kernel -> (kernel name).
 
 
 
 ### Usage
 
 
 ```python
@@ -91,16 +107,25 @@
 
 doc.extract_events('allennlp') # Extraction of events with allennlp tool
 doc.extract_semantic_role_link('allennlp') # Extraction of semantic role links with all tools (should be done after extracting events since most semantic relations are between an actor and an event)
 
 doc.ISO_annotation('annotations.ann') # Outputs ISO annotation in .ann format (txt) in a file called 'annotations.ann', which is a standard of BRAT annotation tool
 
 
-## Structure
 ```
+
+## Examples: Python Notebooks
+
+A  basic notebook that teaches how to use our reader of annotations, which format is assumed is to be in the BRAT format is in the following link: [How to read a BRAT file](https://colab.research.google.com/drive/1_jc6SJNAdWMYBMVlGPldFDmGNg4gFUCs?usp=sharing).
+
+There is the TLDR Python notebook, which extracts the main narrative elements and draw an MSC visulization:  [Too Long Didn't Read Tutorial](https://bit.ly/3s36Bxf).
+
+Finally, there is a notebook that shows how to produce a bubble visualization: [How To: Bubble Visualization](https://colab.research.google.com/drive/1V2DCuP1qAlwUXThTKNUnZ98WxARZXC_v?usp=sharing).
+
+## Structure
 .
 │   README.md
 |   env.yml
 │   requirements.txt
 |   pyproject.toml
 |   MANIFEST.in
 |   LICENSE
```

