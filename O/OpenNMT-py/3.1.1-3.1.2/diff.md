# Comparing `tmp/OpenNMT-py-3.1.1.tar.gz` & `tmp/OpenNMT-py-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenNMT-py-3.1.1.tar", last modified: Thu Mar 30 16:48:45 2023, max compression
+gzip compressed data, was "OpenNMT-py-3.1.2.tar", last modified: Wed May 10 17:39:07 2023, max compression
```

## Comparing `OpenNMT-py-3.1.1.tar` & `OpenNMT-py-3.1.2.tar`

### file list

```diff
@@ -1,131 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.292260 OpenNMT-py-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.268260 OpenNMT-py-3.1.1/OpenNMT_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-03-30 16:48:45.000000 OpenNMT-py-3.1.1/OpenNMT_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-30 16:48:45.000000 OpenNMT-py-3.1.1/OpenNMT_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 16:48:45.000000 OpenNMT-py-3.1.1/OpenNMT_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-30 16:48:45.000000 OpenNMT-py-3.1.1/OpenNMT_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-30 16:48:45.000000 OpenNMT-py-3.1.1/OpenNMT_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-30 16:48:45.000000 OpenNMT-py-3.1.1/OpenNMT_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-03-30 16:48:45.292260 OpenNMT-py-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.268260 OpenNMT-py-3.1.1/onmt/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.268260 OpenNMT-py-3.1.1/onmt/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/bin/average_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/bin/build_vocab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/bin/release_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5092 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/bin/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/bin/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/bin/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.272260 OpenNMT-py-3.1.1/onmt/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/decoders/cnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/decoders/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/decoders/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    24841 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/decoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.276260 OpenNMT-py-3.1.1/onmt/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/encoders/cnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/encoders/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/encoders/ggnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/encoders/mean_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/encoders/rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/encoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.280260 OpenNMT-py-3.1.1/onmt/inputters/
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/inputters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/inputters/dynamic_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/inputters/inputter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/inputters/text_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/inputters/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15027 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.280260 OpenNMT-py-3.1.1/onmt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/models/model_saver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.284260 OpenNMT-py-3.1.1/onmt/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/average_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/conv_multi_step_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/copy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/global_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/multi_headed_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/position_ffn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/sparse_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/sparse_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    24384 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/stacked_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/util_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/modules/weight_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    46254 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/opts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.284260 OpenNMT-py-3.1.1/onmt/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/scorers/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/scorers/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/scorers/ter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.284260 OpenNMT-py-3.1.1/onmt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    28824 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/tests/test_beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/tests/test_copy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/tests/test_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/tests/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-03-30 16:48:35.000000 OpenNMT-py-3.1.1/onmt/tests/test_greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/test_structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/test_subword_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/test_text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/test_translation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/tests/utils_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/train_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    24611 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.288260 OpenNMT-py-3.1.1/onmt/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/bart.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/docify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/fuzzymatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/inlinetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    21922 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/transforms/uppercase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.288260 OpenNMT-py-3.1.1/onmt/translate/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19338 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/decode_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/process_zh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    36060 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/translation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    42496 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/translate/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 16:48:45.292260 OpenNMT-py-3.1.1/onmt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/cnn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/earlystopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15791 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    28164 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/report_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/rnn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/scoring_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/onmt/utils/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 16:48:45.292260 OpenNMT-py-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-03-30 16:48:36.000000 OpenNMT-py-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.110291 OpenNMT-py-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 17:39:07.000000 OpenNMT-py-3.1.2/OpenNMT_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-10 17:39:07.110291 OpenNMT-py-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/onmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/onmt/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1665 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/average_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10596 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/build_vocab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/release_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5186 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/bin/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/onmt/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/cnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26303 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/decoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.098291 OpenNMT-py-3.1.2/onmt/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/cnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/ggnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/mean_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/encoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.102291 OpenNMT-py-3.1.2/onmt/inputters/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/dynamic_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/inputter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11227 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/text_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/inputters/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.102291 OpenNMT-py-3.1.2/onmt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/models/model_saver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.102291 OpenNMT-py-3.1.2/onmt/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/average_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/conv_multi_step_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/copy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15703 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/global_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/multi_headed_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/position_ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/rmsnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/sparse_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/sparse_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24384 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/stacked_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/util_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/modules/weight_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47553 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/opts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.102291 OpenNMT-py-3.1.2/onmt/scorers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/scorers/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/scorers/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/scorers/ter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.106291 OpenNMT-py-3.1.2/onmt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28824 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_copy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18449 2023-05-10 17:39:01.000000 OpenNMT-py-3.1.2/onmt/tests/test_greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_subword_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22901 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_translation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/tests/utils_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/train_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23568 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.106291 OpenNMT-py-3.1.2/onmt/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8598 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/docify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/fuzzymatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/inlinetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22246 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10145 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/transforms/uppercase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.106291 OpenNMT-py-3.1.2/onmt/translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19338 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/decode_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/process_zh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37183 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/translation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42702 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/translate/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 17:39:07.110291 OpenNMT-py-3.1.2/onmt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/cnn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/earlystopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15983 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28164 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/report_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/rnn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/scoring_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/onmt/utils/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 17:39:07.110291 OpenNMT-py-3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-10 17:39:02.000000 OpenNMT-py-3.1.2/setup.py
```

### Comparing `OpenNMT-py-3.1.1/LICENSE.md` & `OpenNMT-py-3.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/OpenNMT_py.egg-info/PKG-INFO` & `OpenNMT-py-3.1.2/OpenNMT_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenNMT-py
-Version: 3.1.1
+Version: 3.1.2
 Summary: A python implementation of OpenNMT
 Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
 Project-URL: Forum, http://forum.opennmt.net/
 Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
 Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `OpenNMT-py-3.1.1/OpenNMT_py.egg-info/SOURCES.txt` & `OpenNMT-py-3.1.2/OpenNMT_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 onmt/modules/copy_generator.py
 onmt/modules/embeddings.py
 onmt/modules/gate.py
 onmt/modules/global_attention.py
 onmt/modules/lora.py
 onmt/modules/multi_headed_attn.py
 onmt/modules/position_ffn.py
+onmt/modules/rmsnorm.py
 onmt/modules/sparse_activations.py
 onmt/modules/sparse_losses.py
 onmt/modules/sru.py
 onmt/modules/stacked_rnn.py
 onmt/modules/structured_attention.py
 onmt/modules/util_class.py
 onmt/modules/weight_norm.py
@@ -76,14 +77,15 @@
 onmt/tests/test_text_utils.py
 onmt/tests/test_transform.py
 onmt/tests/test_translation_server.py
 onmt/tests/test_translator.py
 onmt/tests/utils_for_tests.py
 onmt/transforms/__init__.py
 onmt/transforms/bart.py
+onmt/transforms/clean.py
 onmt/transforms/docify.py
 onmt/transforms/features.py
 onmt/transforms/fuzzymatch.py
 onmt/transforms/inlinetags.py
 onmt/transforms/misc.py
 onmt/transforms/normalize.py
 onmt/transforms/sampling.py
```

### Comparing `OpenNMT-py-3.1.1/PKG-INFO` & `OpenNMT-py-3.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenNMT-py
-Version: 3.1.1
+Version: 3.1.2
 Summary: A python implementation of OpenNMT
 Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
 Project-URL: Forum, http://forum.opennmt.net/
 Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
 Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `OpenNMT-py-3.1.1/README.md` & `OpenNMT-py-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/bin/average_models.py` & `OpenNMT-py-3.1.2/onmt/bin/average_models.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/bin/build_vocab.py` & `OpenNMT-py-3.1.2/onmt/bin/build_vocab.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 #!/usr/bin/env python
 """Get vocabulary coutings from transformed corpora samples."""
 import os
+import copy
+import multiprocessing as mp
+import pyonmttok
+from functools import partial
 from onmt.utils.logging import init_logger, logger
 from onmt.utils.misc import set_random_seed, check_path
 from onmt.utils.parse import ArgumentParser
 from onmt.opts import dynamic_prepare_opts
 from onmt.inputters.text_corpus import build_corpora_iters, get_corpora
 from onmt.inputters.text_utils import process, append_features_to_text
 from onmt.transforms import make_transforms, get_transforms_cls
 from onmt.constants import CorpusName, CorpusTask
 from collections import Counter
-import multiprocessing as mp
+
+
+MAXBUCKETSIZE = 256000
 
 
 def write_files_from_queues(sample_path, queues):
     """
     Standalone process that reads data from
     queues in order and write to sample files.
     """
@@ -103,15 +109,15 @@
     if opts.dump_samples:
         logger.info("The samples on which the vocab is built will be "
                     "dumped to disk. It may slow down the process.")
     corpora = get_corpora(opts, task=CorpusTask.TRAIN)
     counter_src = Counter()
     counter_tgt = Counter()
     counter_src_feats = [Counter() for _ in range(opts.n_src_feats)]
-    from functools import partial
+
     queues = {c_name: [mp.Queue(opts.vocab_sample_queue_size)
                        for i in range(opts.num_threads)]
               for c_name in corpora.keys()}
     sample_path = os.path.join(
         os.path.dirname(opts.save_data), CorpusName.SAMPLE)
     if opts.dump_samples:
         write_process = mp.Process(
@@ -130,14 +136,58 @@
             for i in range(opts.n_src_feats):
                 counter_src_feats[i].update(sub_counter_src_feats[i])
     if opts.dump_samples:
         write_process.join()
     return counter_src, counter_tgt, counter_src_feats
 
 
+def ingest_tokens(opts, transforms, n_sample, learner, stride, offset):
+    def _mp_ingest(data):
+        func = partial(process, CorpusName.TRAIN)
+        chunk = len(data) // opts.num_threads
+        with mp.Pool(opts.num_threads) as pool:
+            buckets = pool.map(func, [data[i * chunk: (i + 1) * chunk]
+                                      for i in range(0, opts.num_threads)])
+        for bucket in buckets:
+            for ex in bucket:
+                if ex is not None:
+                    src_line, tgt_line = (ex['src']['src'],
+                                          ex['tgt']['tgt'])
+                    learner.ingest(src_line)
+                    learner.ingest(tgt_line)
+
+    corpora = get_corpora(opts, task=CorpusTask.TRAIN)
+    datasets_iterables = build_corpora_iters(
+        corpora, transforms, opts.data,
+        skip_empty_level=opts.skip_empty_level,
+        stride=stride, offset=offset)
+    to_ingest = []
+    for c_name, c_iter in datasets_iterables.items():
+        for i, item in enumerate(c_iter):
+            if n_sample >= 0 and i >= n_sample:
+                break
+            if len(to_ingest) >= MAXBUCKETSIZE:
+                _mp_ingest(to_ingest)
+                to_ingest = []
+            to_ingest.append(item)
+        _mp_ingest(to_ingest)
+
+
+def make_learner(tokenization_type, symbols):
+    if tokenization_type == "bpe":
+        # BPE training
+        learner = pyonmttok.BPELearner(tokenizer=None,
+                                       symbols=symbols)
+    elif tokenization_type == "sentencepiece":
+        # SentencePiece training
+        learner = pyonmttok.SentencePieceLearner(vocab_size=symbols,
+                                                 character_coverage=0.98)
+    return learner
+
+
 def build_vocab_main(opts):
     """Apply transforms to samples of specified data and build vocab from it.
 
     Transforms that need vocab will be disabled in this.
     Built vocab is saved in plain text format as following and can be pass as
     `-src_vocab` (and `-tgt_vocab`) when training:
     ```
@@ -150,14 +200,37 @@
     assert opts.n_sample == -1 or opts.n_sample > 1, \
         f"Illegal argument n_sample={opts.n_sample}."
 
     logger = init_logger()
     set_random_seed(opts.seed, False)
     transforms_cls = get_transforms_cls(opts._all_transform)
 
+    if opts.learn_subwords:
+        logger.info(f"Ingesting {opts.src_subword_type} model from corpus")
+        learner = make_learner(opts.src_subword_type,
+                               opts.learn_subwords_size)
+        if opts.src_subword_model is not None:
+            tok_path = opts.src_subword_model
+        else:
+            data_dir = os.path.split(opts.save_data)[0]
+            if not os.path.exists(data_dir):
+                os.makedirs(data_dir)
+            tok_path = os.path.join(
+                data_dir, f"{opts.src_subword_type}.model")
+        save_opts = copy.deepcopy(opts)
+        opts.src_subword_type = 'none'
+        opts.tgt_subword_type = 'none'
+        opts.src_onmttok_kwargs["joiner_annotate"] = False
+        opts.tgt_onmttok_kwargs["joiner_annotate"] = False
+        transforms = make_transforms(opts, transforms_cls, None)
+        ingest_tokens(opts, transforms, opts.n_sample, learner, 1, 0)
+        logger.info(f"Learning {tok_path} model, patience")
+        learner.learn(tok_path)
+        opts = save_opts
+
     transforms = make_transforms(opts, transforms_cls, None)
 
     logger.info(f"Counter vocab from {opts.n_sample} samples.")
     src_counter, tgt_counter, src_feats_counter = build_vocab(
         opts, transforms, n_sample=opts.n_sample)
 
     logger.info(f"Counters src: {len(src_counter)}")
```

### Comparing `OpenNMT-py-3.1.1/onmt/bin/release_model.py` & `OpenNMT-py-3.1.2/onmt/bin/release_model.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/bin/server.py` & `OpenNMT-py-3.1.2/onmt/bin/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,27 @@
     @app.route('/translate', methods=['POST'])
     def translate():
         inputs = request.get_json(force=True)
         if debug:
             logger.info(inputs)
         out = {}
         try:
-            trans, scores, n_best, _, aligns = translation_server.run(inputs)
+            trans, scores, n_best, _, aligns, align_scores = \
+                translation_server.run(inputs)
             assert len(trans) == len(inputs) * n_best
             assert len(scores) == len(inputs) * n_best
             assert len(aligns) == len(inputs) * n_best
 
             out = [[] for _ in range(n_best)]
             for i in range(len(trans)):
                 response = {"src": inputs[i // n_best]['src'], "tgt": trans[i],
                             "n_best": n_best, "pred_score": scores[i]}
                 if len(aligns[i]) > 0 and aligns[i][0] is not None:
                     response["align"] = aligns[i]
+                    response["align_score"] = align_scores[i]
                 out[i % n_best].append(response)
         except ServerModelError as e:
             model_id = inputs[0].get("id")
             if debug:
                 logger.warning("Unload model #{} "
                                "because of an error".format(model_id))
             translation_server.models[model_id].unload()
```

### Comparing `OpenNMT-py-3.1.1/onmt/bin/train.py` & `OpenNMT-py-3.1.2/onmt/bin/train.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/bin/translate.py` & `OpenNMT-py-3.1.2/onmt/bin/translate.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/constants.py` & `OpenNMT-py-3.1.2/onmt/constants.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/decoders/__init__.py` & `OpenNMT-py-3.1.2/onmt/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/decoders/cnn_decoder.py` & `OpenNMT-py-3.1.2/onmt/decoders/cnn_decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/decoders/decoder.py` & `OpenNMT-py-3.1.2/onmt/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/decoders/ensemble.py` & `OpenNMT-py-3.1.2/onmt/decoders/ensemble.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/decoders/transformer.py` & `OpenNMT-py-3.1.2/onmt/decoders/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import torch.nn as nn
 
 from onmt.decoders.decoder import DecoderBase
 from onmt.modules import MultiHeadedAttention, AverageAttention
 from onmt.modules.position_ffn import PositionwiseFeedForward
 from onmt.modules.position_ffn import ActivationFunction
 from onmt.utils.misc import sequence_mask
+from onmt.modules.rmsnorm import RMSNorm
 
 
 class TransformerDecoderLayerBase(nn.Module):
     def __init__(
         self,
         d_model,
         heads,
@@ -23,15 +24,16 @@
         attention_dropout,
         self_attn_type="scaled-dot",
         max_relative_positions=0,
         aan_useffn=False,
         full_context_alignment=False,
         alignment_heads=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
-        add_qkvbias=False
+        add_qkvbias=False,
+        layer_norm='standard'
     ):
         """
         Args:
             d_model (int): the dimension of keys/values/queries in
                 :class:`MultiHeadedAttention`, also the input size of
                 the first-layer of the :class:`PositionwiseFeedForward`.
             heads (int): the number of heads for MultiHeadedAttention.
@@ -51,14 +53,15 @@
                 whether enable an extra full context decoder forward for
                 alignment
             alignment_heads (int):
                 N. of cross attention heads to use for alignment guiding
             pos_ffn_activation_fn (ActivationFunction):
                 activation function choice for PositionwiseFeedForward layer
             add_qkvbias (bool): whether to add bias to the Key/Value nn.Linear
+            layer_norm (string): type of layer normalization standard/rms
 
         """
         super(TransformerDecoderLayerBase, self).__init__()
 
         self.self_attn_type = self_attn_type
         if self_attn_type == "scaled-dot":
             self.self_attn = MultiHeadedAttention(
@@ -71,17 +74,22 @@
             )
         elif self_attn_type == "average":
             self.self_attn = AverageAttention(
                 d_model, dropout=attention_dropout, aan_useffn=aan_useffn
             )
 
         self.feed_forward = PositionwiseFeedForward(d_model, d_ff, dropout,
-                                                    pos_ffn_activation_fn
-                                                    )
-        self.layer_norm_1 = nn.LayerNorm(d_model, eps=1e-6)
+                                                    pos_ffn_activation_fn,
+                                                    layer_norm)
+        if layer_norm == 'standard':
+            self.layer_norm_1 = nn.LayerNorm(d_model, eps=1e-6)
+        elif layer_norm == 'rms':
+            self.layer_norm_1 = RMSNorm(d_model, eps=1e-6)
+        else:
+            raise ValueError(f'{layer_norm} layer norm type is not supported')
         self.drop = nn.Dropout(dropout)
         self.full_context_alignment = full_context_alignment
         self.alignment_heads = alignment_heads
 
     def forward(self, *args, **kwargs):
         """Extend `_forward` for (possibly) multiple decoder pass:
         Always a default (future masked) decoder forward pass,
@@ -146,15 +154,16 @@
 
     def _forward_self_attn(self, layer_in_norm, dec_mask, step):
         if self.self_attn_type == "scaled-dot":
             return self.self_attn(
                 layer_in_norm,
                 layer_in_norm,
                 layer_in_norm,
-                mask=dec_mask
+                mask=dec_mask,
+                step=step
             )
         elif self.self_attn_type == "average":
             return self.self_attn(
                 layer_in_norm, mask=dec_mask, step=step
             )
         else:
             raise ValueError(
@@ -180,15 +189,16 @@
         attention_dropout,
         self_attn_type="scaled-dot",
         max_relative_positions=0,
         aan_useffn=False,
         full_context_alignment=False,
         alignment_heads=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
-        add_qkvbias=False
+        add_qkvbias=False,
+        layer_norm='standard'
     ):
         """
         Args:
             See TransformerDecoderLayerBase
         """
         super(TransformerDecoderLayer, self).__init__(
             d_model,
@@ -198,22 +208,28 @@
             attention_dropout,
             self_attn_type,
             max_relative_positions,
             aan_useffn,
             full_context_alignment,
             alignment_heads,
             pos_ffn_activation_fn=pos_ffn_activation_fn,
-            add_qkvbias=add_qkvbias
+            add_qkvbias=add_qkvbias,
+            layer_norm=layer_norm
         )
         self.context_attn = MultiHeadedAttention(
             heads, d_model, dropout=attention_dropout,
             attn_type="context",
             add_qkvbias=add_qkvbias
         )
-        self.layer_norm_2 = nn.LayerNorm(d_model, eps=1e-6)
+        if layer_norm == 'standard':
+            self.layer_norm_2 = nn.LayerNorm(d_model, eps=1e-6)
+        elif layer_norm == 'rms':
+            self.layer_norm_2 = RMSNorm(d_model, eps=1e-6)
+        else:
+            raise ValueError(f'{layer_norm} layer norm type is not supported')
 
     def update_dropout(self, dropout, attention_dropout):
         super(TransformerDecoderLayer, self).update_dropout(
             dropout, attention_dropout
         )
         self.context_attn.update_dropout(attention_dropout)
 
@@ -275,27 +291,33 @@
         )
         layer_out = self.feed_forward(self.drop(mid) + query)
 
         return layer_out, attns
 
 
 class TransformerDecoderBase(DecoderBase):
-    def __init__(self, d_model, copy_attn, embeddings, alignment_layer):
+    def __init__(self, d_model, copy_attn, embeddings, alignment_layer,
+                 layer_norm):
         super(TransformerDecoderBase, self).__init__()
 
         self.embeddings = embeddings
 
         # Decoder State
         self.state = {}
 
         # previously, there was a GlobalAttention module here for copy
         # attention. But it was never actually used -- the "copy" attention
         # just reuses the context attention.
         self._copy = copy_attn
-        self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
+        if layer_norm == 'standard':
+            self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
+        elif layer_norm == 'rms':
+            self.layer_norm = RMSNorm(d_model, eps=1e-6)
+        else:
+            raise ValueError(f'{layer_norm} layer norm type is not supported')
 
         self.alignment_layer = alignment_layer
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
         return cls(
@@ -312,15 +334,16 @@
             embeddings,
             opt.max_relative_positions,
             opt.aan_useffn,
             opt.full_context_alignment,
             opt.alignment_layer,
             alignment_heads=opt.alignment_heads,
             pos_ffn_activation_fn=opt.pos_ffn_activation_fn,
-            add_qkvbias=opt.add_qkvbias
+            add_qkvbias=opt.add_qkvbias,
+            layer_norm=opt.layer_norm
         )
 
     def init_state(self, src, enc_out, enc_final_hs):
         """Initialize decoder state."""
         self.state["src"] = src
 
     def map_state(self, fn):
@@ -377,14 +400,15 @@
         aan_useffn (bool): Turn on the FFN layer in the AAN decoder
         full_context_alignment (bool):
             whether enable an extra full context decoder forward for alignment
         alignment_layer (int): N° Layer to supervise with for alignment guiding
         alignment_heads (int):
             N. of cross attention heads to use for alignment guiding
         add_qkvbias (bool): whether to add bias to the Key/Value nn.Linear
+        layer_norm (string): type of layer normalization standard/rms
     """
 
     def __init__(
         self,
         num_layers,
         d_model,
         heads,
@@ -396,18 +420,19 @@
         embeddings,
         max_relative_positions,
         aan_useffn,
         full_context_alignment,
         alignment_layer,
         alignment_heads,
         pos_ffn_activation_fn=ActivationFunction.relu,
-        add_qkvbias=False
+        add_qkvbias=False,
+        layer_norm='standard'
     ):
         super(TransformerDecoder, self).__init__(
-            d_model, copy_attn, embeddings, alignment_layer
+            d_model, copy_attn, embeddings, alignment_layer, layer_norm
         )
 
         self.transformer_layers = nn.ModuleList(
             [
                 TransformerDecoderLayer(
                     d_model,
                     heads,
@@ -416,15 +441,16 @@
                     attention_dropout,
                     self_attn_type=self_attn_type,
                     max_relative_positions=max_relative_positions,
                     aan_useffn=aan_useffn,
                     full_context_alignment=full_context_alignment,
                     alignment_heads=alignment_heads,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
-                    add_qkvbias=add_qkvbias
+                    add_qkvbias=add_qkvbias,
+                    layer_norm=layer_norm
                 )
                 for i in range(num_layers)
             ]
         )
 
     def detach_state(self):
         self.state["src"] = self.state["src"].detach()
@@ -438,17 +464,21 @@
         """
         if enc_out is None:
             enc_out = self.embeddings(tgt)
         if step == 0:
             self._init_cache(enc_out)
         elif step is None:
             for layer in self.transformer_layers:
-                layer.self_attn.layer_cache = (
-                    False, {'keys': torch.tensor([]),
-                            'values': torch.tensor([])})
+                if isinstance(layer.self_attn, AverageAttention):
+                    layer.self_attn.layer_cache =\
+                        False, {'prev_g': torch.tensor([])}
+                else:
+                    layer.self_attn.layer_cache = (
+                        False, {'keys': torch.tensor([]),
+                                'values': torch.tensor([])})
                 layer.context_attn.layer_cache = (
                     False, {'keys': torch.tensor([]),
                             'values': torch.tensor([])})
 
         tgt_words = tgt[:, :, 0]
 
         emb = self.embeddings(tgt, step=step)
@@ -596,18 +626,19 @@
         embeddings,
         max_relative_positions,
         aan_useffn,
         full_context_alignment=None,
         alignment_layer=None,
         alignment_heads=None,
         pos_ffn_activation_fn=ActivationFunction.relu,
-        add_qkvbias=False
+        add_qkvbias=False,
+        layer_norm='standard'
     ):
         super(TransformerLMDecoder, self).__init__(
-            d_model, copy_attn, embeddings, None
+            d_model, copy_attn, embeddings, alignment_layer, layer_norm
         )
         self.transformer_layers = nn.ModuleList(
             [
                 TransformerLMDecoderLayer(
                     d_model,
                     heads,
                     d_ff,
@@ -615,15 +646,16 @@
                     attention_dropout,
                     self_attn_type=self_attn_type,
                     max_relative_positions=max_relative_positions,
                     aan_useffn=aan_useffn,
                     full_context_alignment=None,
                     alignment_heads=None,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
-                    add_qkvbias=add_qkvbias
+                    add_qkvbias=add_qkvbias,
+                    layer_norm=layer_norm
                 )
                 for i in range(num_layers)
             ]
         )
 
     def init_state(self, src=None, enc_out=None, enc_final_hs=None):
         super(TransformerLMDecoder, self).init_state(None, None, None)
@@ -640,14 +672,15 @@
                 layer.self_attn.layer_cache = (
                     False, {'keys': torch.tensor([]),
                             'values': torch.tensor([])})
 
         tgt_words = tgt[:, :, 0]
 
         dec_out = self.embeddings(tgt, step=step)
+
         assert dec_out.dim() == 3  # batch x len x embedding_dim
 
         pad_idx = self.embeddings.word_padding_idx
         tgt_pad_mask = tgt_words.data.eq(pad_idx).unsqueeze(1)  # [B, 1, T_tgt]
 
         with_align = kwargs.pop("with_align", False)
         assert not with_align, "TransformerLMDecoder does not support align"
```

### Comparing `OpenNMT-py-3.1.1/onmt/encoders/__init__.py` & `OpenNMT-py-3.1.2/onmt/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/encoders/cnn_encoder.py` & `OpenNMT-py-3.1.2/onmt/encoders/cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/encoders/encoder.py` & `OpenNMT-py-3.1.2/onmt/encoders/encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/encoders/ggnn_encoder.py` & `OpenNMT-py-3.1.2/onmt/encoders/ggnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/encoders/mean_encoder.py` & `OpenNMT-py-3.1.2/onmt/encoders/mean_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/encoders/rnn_encoder.py` & `OpenNMT-py-3.1.2/onmt/encoders/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/encoders/transformer.py` & `OpenNMT-py-3.1.2/onmt/encoders/transformer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/inputters/__init__.py` & `OpenNMT-py-3.1.2/onmt/inputters/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/inputters/dynamic_iterator.py` & `OpenNMT-py-3.1.2/onmt/inputters/dynamic_iterator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/inputters/inputter.py` & `OpenNMT-py-3.1.2/onmt/inputters/inputter.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     src_specials = [item for item in (default_specials + specials['src'])
                     if item not in src_vocab]
     src_vocab = pyonmttok.build_vocab_from_tokens(
         src_vocab,
         maximum_size=opt.src_vocab_size,
         special_tokens=src_specials)
     src_vocab.default_id = src_vocab[DefaultTokens.UNK]
+
     if opt.vocab_size_multiple > 1:
         src_vocab = _pad_vocab_to_multiple(src_vocab, opt.vocab_size_multiple)
     vocabs['src'] = src_vocab
     if opt.share_vocab:
         vocabs['tgt'] = src_vocab
     else:
         tgt_vocab = _read_vocab_file(opt.tgt_vocab,
@@ -118,24 +119,24 @@
     """
 
     if not os.path.exists(vocab_path):
         raise RuntimeError(
             "Vocabulary not found at {}".format(vocab_path))
     else:
         with codecs.open(vocab_path, 'rb', 'utf-8') as f:
-            lines = [line.strip() for line in f if line.strip()]
+            lines = [line.strip('\n') for line in f if line.strip('\n')]
             first_line = lines[0].split(None, 1)
             has_count = (len(first_line) == 2 and first_line[-1].isdigit())
             if has_count:
                 vocab = []
                 for line in lines:
                     if int(line.split(None, 1)[1]) >= min_count:
                         vocab.append(line.split(None, 1)[0])
             else:
-                vocab = [line.strip().split()[0] for line in lines]
+                vocab = lines
             return vocab
 
 
 def vocabs_to_dict(vocabs):
     """
     Convert a dict of pyonmttok vocabs
     into a plain text dict to be saved in the checkpoint
```

### Comparing `OpenNMT-py-3.1.1/onmt/inputters/text_corpus.py` & `OpenNMT-py-3.1.2/onmt/inputters/text_corpus.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,22 +255,23 @@
             bucket = []
             for i, ex in enumerate(c_iter):
                 if i > n_sample:
                     break
                 else:
                     bucket.append(ex)
             pro_bucket = process(CorpusTask.TRAIN, bucket)
-            for maybe_example in pro_bucket:
-                if maybe_example is not None:
-                    src_line, tgt_line = (maybe_example['src']['src'],
-                                          maybe_example['tgt']['tgt'])
+            if pro_bucket is not None:
+                for maybe_example in pro_bucket:
+                    if maybe_example is not None:
+                        src_line, tgt_line = (maybe_example['src']['src'],
+                                              maybe_example['tgt']['tgt'])
 
-                    if 'feats' in maybe_example['src']:
-                        src_feats_lines = maybe_example['src']['feats']
-                    else:
-                        src_feats_lines = []
+                        if 'feats' in maybe_example['src']:
+                            src_feats_lines = maybe_example['src']['feats']
+                        else:
+                            src_feats_lines = []
 
-                    src_pretty_line = append_features_to_text(
-                        src_line, src_feats_lines)
+                        src_pretty_line = append_features_to_text(
+                            src_line, src_feats_lines)
 
-                    f_src.write(src_pretty_line + '\n')
-                    f_tgt.write(tgt_line + '\n')
+                        f_src.write(src_pretty_line + '\n')
+                        f_tgt.write(tgt_line + '\n')
```

### Comparing `OpenNMT-py-3.1.1/onmt/inputters/text_utils.py` & `OpenNMT-py-3.1.2/onmt/inputters/text_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             numeric['tgt']['tgt_ids'] = \
                 vocabs['tgt']([decoder_start_token] + tgt_text
                               + [DefaultTokens.EOS])
 
     elif vocabs['data_task'] == ModelTask.LANGUAGE_MODEL:
         src_text = example['src']['src'].split()
         numeric['src']['src_ids'] = \
-            vocabs['src']([DefaultTokens.BOS] + src_text)
+            vocabs['src']([decoder_start_token] + src_text)
         if example['tgt'] is not None:
             numeric['tgt']['tgt_ids'] = []
             tgt_text = example['tgt']['tgt'].split()
             numeric['tgt']['tgt_ids'] = \
                 vocabs['tgt'](tgt_text + [DefaultTokens.EOS])
     else:
         raise ValueError(
```

### Comparing `OpenNMT-py-3.1.1/onmt/model_builder.py` & `OpenNMT-py-3.1.2/onmt/model_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,34 @@
 from onmt.utils.misc import use_gpu
 from onmt.utils.logging import logger
 from onmt.utils.parse import ArgumentParser
 from onmt.constants import DefaultTokens, ModelTask
 from onmt.modules import Linear, Embedding, mark_only_lora_as_trainable
 
 
+def replace_8bit_linear(model, threshold=6.0, module_to_convert=""):
+    try:
+        import bitsandbytes as bnb
+    except ImportError:
+        raise ImportError("Install bitsandbytes to use 8bit compression")
+    for name, module in model.named_children():
+        if len(list(module.children())) > 0:
+            replace_8bit_linear(module, threshold, module_to_convert)
+
+        if isinstance(module, nn.Linear) and name == module_to_convert:
+            model._modules[name] = bnb.nn.Linear8bitLt(
+                module.in_features,
+                module.out_features,
+                module.bias is not None,
+                has_fp16_weights=False,
+                threshold=threshold,
+            )
+    return model
+
+
 def replace_lora_linear(model, r=2, lora_alpha=1,
                         lora_dropout=0, layer=""):
     """
     Function replacing layers with LoRa layers recursively.
     Args:
         model:
         r: rank of matrix of the Low Rank layer
@@ -29,21 +49,23 @@
         lora_dropout: cf paper
         layer: layer name of the model to be replaced
     """
     for name, module in model.named_children():
         if len(list(module.children())) > 0:
             replace_lora_linear(module, r, lora_alpha,
                                 lora_dropout, layer)
+
         if isinstance(module, nn.Linear) and name == layer:
             model._modules[name] = Linear(
                 module.in_features,
                 module.out_features,
                 r=r,
                 lora_alpha=lora_alpha,
-                lora_dropout=lora_dropout)
+                lora_dropout=lora_dropout,
+                bias=module.bias is not None)
     return model
 
 
 def replace_lora_embedding(model, r=2, lora_alpha=1):
     """
     Function replacing Embeddings with LoRa ones recursively.
     Args:
@@ -134,36 +156,37 @@
 def load_test_model(opt, model_path=None):
     if model_path is None:
         model_path = opt.models[0]
     checkpoint = torch.load(model_path,
                             map_location=lambda storage, loc: storage)
 
     model_opt = ArgumentParser.ckpt_model_opts(checkpoint['opt'])
-    # Patch for NLLB200 model loading
-    if ('encoder.embeddings.make_embedding.pe.pe' not in
-            checkpoint['model'].keys()):
-        model_opt.position_encoding_type = 'SinusoidalConcat'
 
     ArgumentParser.update_model_opts(model_opt)
     ArgumentParser.validate_model_opts(model_opt)
     vocabs = dict_to_vocabs(checkpoint['vocab'])
 
     # Avoid functionality on inference
     model_opt.update_vocab = False
 
-    model = build_base_model(model_opt, vocabs, use_gpu(opt), checkpoint,
-                             opt.gpu)
-    if opt.fp32:
+    model = build_base_model(model_opt, vocabs, checkpoint)
+
+    if opt.precision == 'fp32':
         model.float()
-    elif opt.int8:
+    elif opt.precision == 'fp16':
+        model.half()
+    elif opt.precision == 'int8':
         if opt.gpu >= 0:
             raise ValueError(
                 "Dynamic 8-bit quantization is not supported on GPU")
         torch.quantization.quantize_dynamic(model, inplace=True)
 
+    if use_gpu(opt) and opt.gpu >= 0:
+        model.to(torch.device("cuda", opt.gpu))
+
     model.eval()
     model.generator.eval()
     return vocabs, model, model_opt
 
 
 def build_src_emb(model_opt, vocabs):
     # Build embeddings.
@@ -256,61 +279,59 @@
         # Remove old vocabulary associated embeddings
         del checkpoint['model'][emb_name]
     del checkpoint['generator']['weight'], checkpoint['generator']['bias']
     model.load_state_dict(model_dict)
     generator.load_state_dict(generator_dict)
 
 
-def build_base_model(model_opt, vocabs, gpu, checkpoint=None, gpu_id=None):
+def build_base_model(model_opt, vocabs, checkpoint=None):
     """Build a model from opts.
 
     Args:
         model_opt: the option loaded from checkpoint. It's important that
             the opts have been updated and validated. See
             :class:`onmt.utils.parse.ArgumentParser`.
         vocabs (dict[str, Vocab]):
             `Field` objects for the model.
-        gpu (bool): whether to use gpu.
         checkpoint: the model generated by train phase, or a resumed snapshot
                     model from a stopped training.
-        gpu_id (int or NoneType): Which GPU to use.
 
     Returns:
         the NMTModel.
     """
 
     # for back compat when attention_dropout was not defined
     try:
         model_opt.attention_dropout
     except AttributeError:
         model_opt.attention_dropout = model_opt.dropout
 
     # Build Model
-    if gpu and gpu_id is not None:
-        device = torch.device("cuda", gpu_id)
-    elif gpu and not gpu_id:
-        device = torch.device("cuda")
-    elif not gpu:
-        device = torch.device("cpu")
-
     model = build_task_specific_model(model_opt, vocabs)
 
+    if hasattr(model_opt, 'quant_layers') and len(model_opt.quant_layers) > 0:
+        for layer in model_opt.quant_layers:
+            logger.info("8bit compression of layer %s" % layer)
+            model = replace_8bit_linear(model, module_to_convert=layer)
+
     mark_lora = False
     if hasattr(model_opt, 'lora_layers') and len(model_opt.lora_layers) > 0:
         if model_opt.freeze_encoder or model_opt.freeze_decoder:
             raise ValueError("Cannot use LoRa with Enc/Dec-oder freezing")
         for layer in model_opt.lora_layers:
+            logger.info("Adding LoRa layers for %s" % layer)
             model = replace_lora_linear(model, r=model_opt.lora_rank,
                                         lora_alpha=model_opt.lora_alpha,
                                         lora_dropout=model_opt.lora_dropout,
                                         layer=layer)
         mark_lora = True
     if hasattr(model_opt, 'lora_embedding') and model_opt.lora_embedding:
         if model_opt.freeze_encoder or model_opt.freeze_decoder:
             raise ValueError("Cannot use LoRa with Enc/Dec-oder freezing")
+        logger.info("Adding LoRa Embeddings")
         model = replace_lora_embedding(model, r=model_opt.lora_rank,
                                        lora_alpha=model_opt.lora_alpha)
         mark_lora = True
 
     if mark_lora:
         mark_only_lora_as_trainable(model, bias='lora_only')
 
@@ -363,43 +384,49 @@
 
         if '0.weight' in checkpoint['generator']:
             checkpoint['generator']['weight'] =\
                 checkpoint['generator'].pop('0.weight')
         if '0.bias' in checkpoint['generator']:
             checkpoint['generator']['bias'] =\
                 checkpoint['generator'].pop('0.bias')
-
         # end of patch for backward compatibility
+
         if model_opt.update_vocab:
             # Update model embeddings with those from the checkpoint
             # after initialization
             use_embeddings_from_checkpoint(vocabs, model, generator,
                                            checkpoint)
 
-        model.load_state_dict(checkpoint['model'], strict=False)
-
-        generator.load_state_dict(checkpoint['generator'], strict=False)
+        # when using LoRa or updating the vocab (no more embeddings in ckpt)
+        # => strict=False when loading state_dict
+        strict = (not model_opt.update_vocab) and (not mark_lora)
+        model.load_state_dict(checkpoint['model'],
+                              strict=strict)
+        generator.load_state_dict(checkpoint['generator'],
+                                  strict=strict)
 
     model.generator = generator
 
+    return model
+
+
+def build_model(model_opt, opt, vocabs, checkpoint):
+    logger.info('Building model...')
+    model = build_base_model(model_opt, vocabs, checkpoint)
+
     if model_opt.freeze_encoder:
         model.encoder.requires_grad_(False)
         model.encoder.embeddings.requires_grad_()
 
     if model_opt.freeze_decoder:
         model.decoder.requires_grad_(False)
         model.decoder.embeddings.requires_grad_()
 
-    model.to(device)
     if model_opt.model_dtype == 'fp16' and \
             model_opt.apex_opt_level not in ['O0', 'O1', 'O2', 'O3'] and \
             model_opt.optim == 'fusedadam':
-        model.half()
-
-    return model
+        model.half()   # with amp pytorch requires NOT to half the model
 
-
-def build_model(model_opt, opt, vocabs, checkpoint):
-    logger.info('Building model...')
-    model = build_base_model(model_opt, vocabs, use_gpu(opt), checkpoint)
+    if use_gpu(opt):
+        model.to(torch.device("cuda"))
     logger.info(model)
     return model
```

### Comparing `OpenNMT-py-3.1.1/onmt/models/model.py` & `OpenNMT-py-3.1.2/onmt/models/model.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/__init__.py` & `OpenNMT-py-3.1.2/onmt/modules/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from onmt.modules.copy_generator import CopyGenerator, CopyGeneratorLoss
 from onmt.modules.multi_headed_attn import MultiHeadedAttention
 from onmt.modules.embeddings import Embeddings, PositionalEncoding
 from onmt.modules.weight_norm import WeightNormConv2d
 from onmt.modules.average_attn import AverageAttention
 from onmt.modules.lora import LoRALayer, Embedding, Linear, MergedLinear
 from onmt.modules.lora import mark_only_lora_as_trainable, lora_state_dict
+from onmt.modules.rmsnorm import RMSNorm
 
 __all__ = ["Elementwise", "context_gate_factory", "ContextGate",
            "GlobalAttention", "ConvMultiStepAttention", "CopyGenerator",
            "CopyGeneratorLoss", "CopyGeneratorLMLossCompute",
            "MultiHeadedAttention", "Embeddings", "PositionalEncoding",
-           "WeightNormConv2d", "AverageAttention",
+           "WeightNormConv2d", "AverageAttention", "RMSNorm",
            "LoRALayer", "Embedding", "Linear", "MergedLinear",
            "mark_only_lora_as_trainable", "lora_state_dict"]
```

### Comparing `OpenNMT-py-3.1.1/onmt/modules/average_attn.py` & `OpenNMT-py-3.1.2/onmt/modules/average_attn.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/conv_multi_step_attention.py` & `OpenNMT-py-3.1.2/onmt/modules/conv_multi_step_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/copy_generator.py` & `OpenNMT-py-3.1.2/onmt/modules/copy_generator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/embeddings.py` & `OpenNMT-py-3.1.2/onmt/modules/embeddings.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/gate.py` & `OpenNMT-py-3.1.2/onmt/modules/gate.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/global_attention.py` & `OpenNMT-py-3.1.2/onmt/modules/global_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/lora.py` & `OpenNMT-py-3.1.2/onmt/modules/lora.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #  --------------------------------------------------------------------------
-#  MOstly copied from https://github.com/microsoft/LoRA/
+#  Mostly copied from https://github.com/microsoft/LoRA/
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT).
+#
 #  --------------------------------------------------------------------------
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 import math
 from typing import List, Dict
@@ -62,38 +63,42 @@
             # initialize A the same way as the default
             # for nn.Linear and B to zero
             nn.init.zeros_(self.lora_A)
             nn.init.normal_(self.lora_B)
 
     def train(self, mode: bool = True):
         nn.Embedding.train(self, mode)
-        if self.merge_weights and self.merged:
-            # Make sure that the weights are not merged
-            if self.r > 0:
-                self.weight.data -= \
-                    (self.lora_B @ self.lora_A).T * self.scaling
-            self.merged = False
-
-    def eval(self):
-        nn.Embedding.eval(self)
-        if self.merge_weights and not self.merged:
-            # Merge the weights and mark it
-            if self.r > 0:
-                self.weight.data += (self.lora_B @ self.lora_A) * self.scaling
-            self.merged = True
+        if mode:
+            if self.merge_weights and self.merged:
+                # Make sure that the weights are not merged
+                if self.r > 0:
+                    self.weight.data -= \
+                        (self.lora_B @
+                         self.lora_A).transpose(0, 1) * self.scaling
+                self.merged = False
+        else:
+            if self.merge_weights and not self.merged:
+                # Merge the weights and mark it
+                if self.r > 0:
+                    self.weight.data += \
+                        (self.lora_B @
+                         self.lora_A).transpose(0, 1) * self.scaling
+                self.merged = True
 
     def forward(self, x: torch.Tensor):
         if self.r > 0 and not self.merged:
             result = nn.Embedding.forward(self, x)
             if self.r > 0:
                 after_A = F.embedding(
-                    x, self.lora_A.T, self.padding_idx, self.max_norm,
+                    x, self.lora_A.transpose(0, 1),
+                    self.padding_idx, self.max_norm,
                     self.norm_type, self.scale_grad_by_freq, self.sparse
                 )
-                result += (after_A @ self.lora_B.T) * self.scaling
+                result += (after_A @
+                           self.lora_B.transpose(0, 1)) * self.scaling
             return result
         else:
             return nn.Embedding.forward(self, x)
 
 
 class Linear(nn.Linear, LoRALayer):
     # LoRA implemented in a dense layer
@@ -123,55 +128,52 @@
             self.lora_B = \
                 nn.Parameter(self.weight.new_zeros((out_features, r)))
             self.scaling = self.lora_alpha / self.r
             # Freezing the pre-trained weight matrix
             self.weight.requires_grad = False
         self.reset_parameters()
         if fan_in_fan_out:
-            self.weight.data = self.weight.data.T
+            self.weight.data = self.weight.data.transpose(0, 1)
 
     def reset_parameters(self):
         nn.Linear.reset_parameters(self)
         if hasattr(self, 'lora_A'):
             # initialize A the same way as the default
             # for nn.Linear and B to zero
             nn.init.kaiming_uniform_(self.lora_A, a=math.sqrt(5))
             nn.init.zeros_(self.lora_B)
 
     def train(self, mode: bool = True):
         def T(w):
-            return w.T if self.fan_in_fan_out else w
+            return w.transpose(0, 1) if self.fan_in_fan_out else w
         nn.Linear.train(self, mode)
-        if self.merge_weights and self.merged:
-            # Make sure that the weights are not merged
-            if self.r > 0:
-                self.weight.data -= \
-                    T(self.lora_B @ self.lora_A) * self.scaling
-            self.merged = False
-
-    def eval(self):
-        def T(w):
-            return w.T if self.fan_in_fan_out else w
-        nn.Linear.eval(self)
-        if self.merge_weights and not self.merged:
-            # Merge the weights and mark it
-            if self.r > 0:
-                self.weight.data += \
-                    T(self.lora_B @ self.lora_A) * self.scaling
-            self.merged = True
+        if mode:
+            if self.merge_weights and self.merged:
+                # Make sure that the weights are not merged
+                if self.r > 0:
+                    self.weight.data -= \
+                        T(self.lora_B @ self.lora_A) * self.scaling
+                self.merged = False
+        else:
+            if self.merge_weights and not self.merged:
+                # Merge the weights and mark it
+                if self.r > 0:
+                    self.weight.data += \
+                        T(self.lora_B @ self.lora_A) * self.scaling
+                self.merged = True
 
     def forward(self, x: torch.Tensor):
         def T(w):
-            return w.T if self.fan_in_fan_out else w
+            return w.transpose(0, 1) if self.fan_in_fan_out else w
         if self.r > 0 and not self.merged:
             result = F.linear(x, T(self.weight), bias=self.bias)
             if self.r > 0:
                 result += \
-                    (self.lora_dropout(x) @ self.lora_A.T
-                     @ self.lora_B.T) * self.scaling
+                    (self.lora_dropout(x) @ self.lora_A.transpose(0, 1)
+                     @ self.lora_B.transpose(0, 1)) * self.scaling
             return result
         else:
             return F.linear(x, T(self.weight), bias=self.bias)
 
 
 class MergedLinear(nn.Linear, LoRALayer):
     # LoRA implemented in a dense layer
@@ -210,15 +212,15 @@
             self.lora_ind = self.weight.new_zeros(
                 (out_features, ), dtype=torch.bool
             ).view(len(enable_lora), -1)
             self.lora_ind[enable_lora, :] = True
             self.lora_ind = self.lora_ind.view(-1)
         self.reset_parameters()
         if fan_in_fan_out:
-            self.weight.data = self.weight.data.T
+            self.weight.data = self.weight.data.transpose(0, 1)
 
     def reset_parameters(self):
         nn.Linear.reset_parameters(self)
         if hasattr(self, 'lora_A'):
             # initialize A the same way as the default
             # for nn.Linear and B to zero
             nn.init.kaiming_uniform_(self.lora_A, a=math.sqrt(5))
@@ -231,45 +233,44 @@
             -1, self.out_features
             // len(self.enable_lora) * sum(self.enable_lora)
         )
         return result.view((*x.shape[:-1], self.out_features))
 
     def train(self, mode: bool = True):
         def T(w):
-            return w.T if self.fan_in_fan_out else w
+            return w.transpose(0, 1) if self.fan_in_fan_out else w
         nn.Linear.train(self, mode)
-        if self.merge_weights and self.merged:
-            # Make sure that the weights are not merged
-            if self.r > 0 and any(self.enable_lora):
-                delta_w = F.conv1d(
-                    self.lora_A.data.unsqueeze(0),
-                    self.lora_B.data.unsqueeze(-1),
-                    groups=sum(self.enable_lora)
-                ).squeeze(0)
-                self.weight.data -= self.zero_pad(T(delta_w * self.scaling))
-            self.merged = False
-
-    def eval(self):
-        def T(w):
-            return w.T if self.fan_in_fan_out else w
-        nn.Linear.eval(self)
-        if self.merge_weights and not self.merged:
-            # Merge the weights and mark it
-            if self.r > 0 and any(self.enable_lora):
-                delta_w = F.conv1d(
-                    self.lora_A.data.unsqueeze(0),
-                    self.lora_B.data.unsqueeze(-1),
-                    groups=sum(self.enable_lora)
-                ).squeeze(0)
-                self.weight.data += self.zero_pad(T(delta_w * self.scaling))
-            self.merged = True
+        if mode:
+            if self.merge_weights and self.merged:
+                # Make sure that the weights are not merged
+                if self.r > 0 and any(self.enable_lora):
+                    delta_w = F.conv1d(
+                        self.lora_A.data.unsqueeze(0),
+                        self.lora_B.data.unsqueeze(-1),
+                        groups=sum(self.enable_lora)
+                    ).squeeze(0)
+                    self.weight.data -= self.zero_pad(T(delta_w *
+                                                        self.scaling))
+                self.merged = False
+        else:
+            if self.merge_weights and not self.merged:
+                # Merge the weights and mark it
+                if self.r > 0 and any(self.enable_lora):
+                    delta_w = F.conv1d(
+                        self.lora_A.data.unsqueeze(0),
+                        self.lora_B.data.unsqueeze(-1),
+                        groups=sum(self.enable_lora)
+                    ).squeeze(0)
+                    self.weight.data += self.zero_pad(T(delta_w *
+                                                        self.scaling))
+                self.merged = True
 
     def forward(self, x: torch.Tensor):
         def T(w):
-            return w.T if self.fan_in_fan_out else w
+            return w.transpose(0, 1) if self.fan_in_fan_out else w
         if self.merged:
             return F.linear(x, T(self.weight), bias=self.bias)
         else:
             result = F.linear(x, T(self.weight), bias=self.bias)
             if self.r > 0:
                 after_A = F.linear(self.lora_dropout(x), self.lora_A)
                 after_B = F.conv1d(
```

### Comparing `OpenNMT-py-3.1.1/onmt/modules/multi_headed_attn.py` & `OpenNMT-py-3.1.2/onmt/modules/multi_headed_attn.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,43 @@
 import math
 import torch
 from torch import Tensor
 from typing import Optional, Tuple
 import torch.nn as nn
 
 
+# Help functions for Rotary Embeddings
+# https://arxiv.org/pdf/2104.09864.pdf
+# too convoluted to make maxseqlen a parameter.
+# we suppose src_seq_len at training and max_length at inference
+# are both < 2048 tokens.
+
+def rotaryembeddings(dim: int, maxseqlen=4096, base=10000):
+    inv_freq = 1.0 / (base ** (torch.arange(0, dim, 2).float() / dim))
+    tmax = torch.arange(maxseqlen, device=inv_freq.device)
+    rope = torch.outer(tmax, inv_freq).float()
+    # rope is now matrix [maxseqlen, dim/2]
+    rope = torch.polar(torch.ones_like(rope), rope)
+    return rope
+
+
+def apply_rotary_emb(query, key, rope):
+    query_ = query.float().reshape(*query.shape[:-1], -1, 2)
+    query_ = torch.view_as_complex(query_)
+    key_ = key.float().reshape(*key.shape[:-1], -1, 2)
+    key_ = torch.view_as_complex(key_)
+    rope = rope.view(1, query_.size(1), 1, query_.size(3))
+    query_out = torch.view_as_real(query_ * rope).flatten(3)
+    key_out = torch.view_as_real(key_ * rope).flatten(3)
+    return query_out.type_as(query), key_out.type_as(key)
+
+
+# Help functions for max_relative positions
+# https://arxiv.org/abs/1803.02155
+
 def relative_matmul(x: Tensor, z: Tensor,
                     transpose: bool) -> Tensor:
     """
     Helper function for relative positions attention.
     https://arxiv.org/pdf/1803.02155.pdf
     x shape [batch_size x heads x q_len x k_len]
     """
@@ -44,14 +73,16 @@
                                        min=-max_relative_positions,
                                        max=max_relative_positions)
     # Shift values to be >= 0
     final_mat = distance_mat_clipped + max_relative_positions
     return final_mat
 
 
+# Help functions to split model dim per head
+
 def shape(x: Tensor, dim_per_head: int) -> Tensor:
     """
     Projection.
     [batchsize x length x modeldim]
     -> [batchsize x heads x length x dimperhead]
     """
     return x.view(x.size(0), x.size(1), -1, dim_per_head) \
@@ -139,61 +170,84 @@
             # for both.
             vocab_size = max_relative_positions * 2 + 1
             self.relative_positions_embeddings = nn.Embedding(
                 vocab_size, self.dim_per_head)
         else:
             self.relative_positions_embeddings = None
 
+            if max_relative_positions == -1:  # rotary embeddings
+                self.rope = rotaryembeddings(self.dim_per_head)
+
     def update_dropout(self, dropout: float) -> None:
         self.dropout.p = dropout
 
     # @torch.jit.script_method
     def forward(self, key: Tensor, value: Tensor,
-                query: Tensor, mask: Optional[Tensor] = None
+                query: Tensor, mask: Optional[Tensor] = None,
+                step: Optional[int] = 0
                 ) -> Tuple[Tensor, Tensor]:
         """
         Compute the context vector and the attention vectors.
 
         Args:
            key (Tensor): set of `key_len`
                key vectors ``(batch, key_len, dim)``
            value (Tensor): set of `key_len`
                value vectors ``(batch, key_len, dim)``
            query (Tensor): set of `query_len`
                query vectors  ``(batch, query_len, dim)``
            mask: binary mask 1/0 indicating which keys have
                zero / non-zero attention ``(batch, query_len, key_len)``
+           step (int): decoding step (used for Rotary embedding)
         Returns:
            (Tensor, Tensor):
 
            * output context vectors ``(batch, query_len, dim)``
            * Attention vector in heads ``(batch, head, query_len, key_len)``.
         """
         # 1) Project key, value, and query.
         # as a reminder at training layer_cache[0] remains False
         if self.layer_cache[0]:
             if self.attn_type == "self":
                 query, key, value = self.linear_query(query),\
                                     self.linear_keys(query),\
                                     self.linear_values(query)
+                query = shape(query, self.dim_per_head)
                 key = shape(key, self.dim_per_head)
                 value = shape(value, self.dim_per_head)
+
+                if self.max_relative_positions == -1:  # Rotary Embeddings
+                    start_pos = step
+                    seqlen = query.size(2)
+                    rope = self.rope[start_pos:
+                                     start_pos +
+                                     seqlen].to(query.device)
+
+                    query = query.transpose(1, 2)
+                    key = key.transpose(1, 2)
+                    query, key = apply_rotary_emb(query,
+                                                  key,
+                                                  rope=rope)
+                    query = query.transpose(1, 2)
+                    key = key.transpose(1, 2)
+
                 if self.layer_cache[1]['keys'].numel() != 0:
                     key = torch.cat(
                         (self.layer_cache[1]['keys'], key),
                         dim=2)
 
                 if self.layer_cache[1]['values'].numel() != 0:
                     value = torch.cat(
                         (self.layer_cache[1]['values'], value),
                         dim=2)
                 self.layer_cache[1]['keys'] = key
                 self.layer_cache[1]['values'] = value
             elif self.attn_type == "context":
                 query = self.linear_query(query)
+                query = shape(query, self.dim_per_head)
                 if self.layer_cache[1]['keys'].numel() == 0:
                     key, value = self.linear_keys(key),\
                                  self.linear_values(value)
                     key = shape(key, self.dim_per_head)
                     value = shape(value, self.dim_per_head)
                 else:
                     key, value = self.layer_cache[1]['keys'],\
@@ -202,17 +256,30 @@
                 self.layer_cache[1]['values'] = value
         else:
             key = self.linear_keys(key)
             value = self.linear_values(value)
             query = self.linear_query(query)
             key = shape(key, self.dim_per_head)
             value = shape(value, self.dim_per_head)
+            query = shape(query, self.dim_per_head)
 
-        query = shape(query, self.dim_per_head)
-
+            if self.max_relative_positions == -1:  # Rotary Embeddings
+                start_pos = 0
+                seqlen = query.size(2)
+                rope = self.rope[start_pos:
+                                 start_pos +
+                                 seqlen].to(query.device)
+
+                query = query.transpose(1, 2)
+                key = key.transpose(1, 2)
+                query, key = apply_rotary_emb(query,
+                                              key,
+                                              rope=rope)
+                query = query.transpose(1, 2)
+                key = key.transpose(1, 2)
         # 2) Calculate and scale scores.
         query = query / math.sqrt(self.dim_per_head)
         # batch x num_heads x query_len x key_len
         query_key = torch.matmul(query, key.transpose(2, 3))
 
         if self.relative_positions_embeddings is not None:
             key_len = key.size(2)
```

### Comparing `OpenNMT-py-3.1.1/onmt/modules/position_ffn.py` & `OpenNMT-py-3.1.2/onmt/modules/stacked_rnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,65 @@
-"""Position feed-forward network from "Attention is All You Need"."""
-
+""" Implementation of ONMT RNN for Input Feeding Decoding """
+import torch
 import torch.nn as nn
-import torch.nn.functional as F
 
 
-class ActivationFunction(object):
-    relu = "relu"
-    gelu = "gelu"
+class StackedLSTM(nn.Module):
+    """
+    Our own implementation of stacked LSTM.
+    Needed for the decoder, because we do input feeding.
+    """
 
+    def __init__(self, num_layers, input_size, hidden_size, dropout):
+        super(StackedLSTM, self).__init__()
+        self.dropout = nn.Dropout(dropout)
+        self.num_layers = num_layers
+        self.layers = nn.ModuleList()
+
+        for _ in range(num_layers):
+            self.layers.append(nn.LSTMCell(input_size, hidden_size))
+            input_size = hidden_size
+
+    def forward(self, input_feed, hidden):
+        h_0, c_0 = hidden
+        h_1, c_1 = [], []
+        for i, layer in enumerate(self.layers):
+            h_1_i, c_1_i = layer(input_feed, (h_0[i], c_0[i]))
+            input_feed = h_1_i
+            if i + 1 != self.num_layers:
+                input_feed = self.dropout(input_feed)
+            h_1 += [h_1_i]
+            c_1 += [c_1_i]
 
-ACTIVATION_FUNCTIONS = {
-    ActivationFunction.relu: F.relu,
-    ActivationFunction.gelu: F.gelu,
-}
+        h_1 = torch.stack(h_1)
+        c_1 = torch.stack(c_1)
 
+        return input_feed, (h_1, c_1)
 
-class PositionwiseFeedForward(nn.Module):
-    """ A two-layer Feed-Forward-Network with residual layer norm.
 
-    Args:
-        d_model (int): the size of input for the first-layer of the FFN.
-        d_ff (int): the hidden layer size of the second-layer
-            of the FNN.
-        dropout (float): dropout probability in :math:`[0, 1)`.
-        activation_fn (ActivationFunction): activation function used.
+class StackedGRU(nn.Module):
     """
+    Our own implementation of stacked GRU.
+    Needed for the decoder, because we do input feeding.
+    """
+
+    def __init__(self, num_layers, input_size, hidden_size, dropout):
+        super(StackedGRU, self).__init__()
+        self.dropout = nn.Dropout(dropout)
+        self.num_layers = num_layers
+        self.layers = nn.ModuleList()
+
+        for _ in range(num_layers):
+            self.layers.append(nn.GRUCell(input_size, hidden_size))
+            input_size = hidden_size
+
+    def forward(self, input_feed, hidden):
+        h_1 = []
+        for i, layer in enumerate(self.layers):
+            h_1_i = layer(input_feed, hidden[0][i])
+            input_feed = h_1_i
+            if i + 1 != self.num_layers:
+                input_feed = self.dropout(input_feed)
+            h_1 += [h_1_i]
 
-    def __init__(self, d_model, d_ff, dropout=0.1,
-                 activation_fn=ActivationFunction.relu):
-        super(PositionwiseFeedForward, self).__init__()
-        self.w_1 = nn.Linear(d_model, d_ff)
-        self.w_2 = nn.Linear(d_ff, d_model)
-        self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
-        self.dropout_1 = nn.Dropout(dropout)
-        self.activation = ACTIVATION_FUNCTIONS[activation_fn]
-        self.dropout_2 = nn.Dropout(dropout)
-
-    def forward(self, x):
-        """Layer definition.
-
-        Args:
-            x: ``(batch_size, input_len, model_dim)``
-
-        Returns:
-            (FloatTensor): Output ``(batch_size, input_len, model_dim)``.
-        """
-
-        inter = self.dropout_1(self.activation(self.w_1(self.layer_norm(x))))
-        output = self.dropout_2(self.w_2(inter))
-        return output + x
-
-    def update_dropout(self, dropout):
-        self.dropout_1.p = dropout
-        self.dropout_2.p = dropout
+        h_1 = torch.stack(h_1)
+        return input_feed, (h_1,)
```

### Comparing `OpenNMT-py-3.1.1/onmt/modules/sparse_activations.py` & `OpenNMT-py-3.1.2/onmt/modules/sparse_activations.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/sparse_losses.py` & `OpenNMT-py-3.1.2/onmt/modules/sparse_losses.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/sru.py` & `OpenNMT-py-3.1.2/onmt/modules/sru.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/structured_attention.py` & `OpenNMT-py-3.1.2/onmt/modules/structured_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/util_class.py` & `OpenNMT-py-3.1.2/onmt/modules/util_class.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/modules/weight_norm.py` & `OpenNMT-py-3.1.2/onmt/modules/weight_norm.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/opts.py` & `OpenNMT-py-3.1.2/onmt/opts.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,19 @@
                   " -save_data should be set as saving prefix.")
     else:
         group.add('-dump_samples', '--dump_samples', action='store_true',
                   help="Dump samples when building vocab. "
                   "Warning: this may slow down the process.")
         group.add('-num_threads', '--num_threads', type=int, default=1,
                   help="Number of parallel threads to build the vocab.")
+        group.add('-learn_subwords', '--learn_subwords', action='store_true',
+                  help="Learn subwords prior to building vocab")
+        group.add('-learn_subwords_size', '--learn_subwords_size', type=int,
+                  default=32000,
+                  help="Learn subwords operations")
         group.add('-vocab_sample_queue_size', '--vocab_sample_queue_size',
                   type=int, default=20,
                   help="Size of queues used in the build_vocab dump path.")
 
 
 def _add_features_opts(parser):
     group = parser.add_argument_group("Features")
@@ -334,14 +339,20 @@
               help="Size of encoder rnn hidden states.")
     group.add('--dec_hid_size', '-dec_hid_size', type=int, default=500,
               help="Size of decoder rnn hidden states.")
     group.add('--cnn_kernel_width', '-cnn_kernel_width', type=int, default=3,
               help="Size of windows in the cnn, the kernel_size is "
                    "(cnn_kernel_width, 1) in conv layer")
 
+    group.add('--layer_norm', '-layer_norm',
+              type=str, default='standard',
+              choices=['standard', 'rms'], help='The type of layer'
+              ' normalization in the transformer architecture. Choices are'
+              ' standard or rms. Default to standard')
+
     group.add('--pos_ffn_activation_fn', '-pos_ffn_activation_fn',
               type=str, default=ActivationFunction.relu,
               choices=ACTIVATION_FUNCTIONS.keys(), help='The activation'
               ' function to use in PositionwiseFeedForward layer. Choices are'
               f' {ACTIVATION_FUNCTIONS.keys()}. Default to'
               f' {ActivationFunction.relu}.')
 
@@ -390,18 +401,22 @@
               type=str, default="softmax", choices=["softmax", "sparsemax"])
     group.add('--self_attn_type', '-self_attn_type',
               type=str, default="scaled-dot",
               help='Self attention type in Transformer decoder '
                    'layer -- currently "scaled-dot" or "average" ')
     group.add('--max_relative_positions', '-max_relative_positions',
               type=int, default=0,
-              help="Maximum distance between inputs in relative "
+              help="This setting enable relative position encoding"
+                   "We support two types of encodings:"
+                   "set this -1 to enable Rotary Embeddings"
+                   "more info: https://arxiv.org/abs/2104.09864"
+                   "set this to > 0 (ex: 16, 32) to use"
+                   "Maximum distance between inputs in relative "
                    "positions representations. "
-                   "For more detailed information, see: "
-                   "https://arxiv.org/pdf/1803.02155.pdf")
+                   "more info: https://arxiv.org/pdf/1803.02155.pdf")
     group.add('--heads', '-heads', type=int, default=8,
               help='Number of heads for transformer self-attention')
     group.add('--transformer_ff', '-transformer_ff', type=int, default=2048,
               help='Size of hidden transformer feed-forward')
     group.add('--aan_useffn', '-aan_useffn', action="store_true",
               help='Turn on the FFN layer in the AAN decoder')
     group.add('--add_qkvbias', '-add_qkvbias', action="store_true",
@@ -492,27 +507,30 @@
               help="Gives more info on each process per GPU.")
     group.add('--master_ip', '-master_ip', default="localhost", type=str,
               help="IP of master for torch.distributed training.")
     group.add('--master_port', '-master_port', default=10000, type=int,
               help="Port of master for torch.distributed training.")
 
     # LoRa
-    group.add('--lora_layers', '-lora_layers', default=[], nargs='*', type=str,
+    group.add('--lora_layers', '-lora_layers', default=[], nargs='+', type=str,
               help="list of layers to be replaced by LoRa layers."
                    " ex: ['linear_values', 'linear_query'] "
                    " cf paper §4.2 https://arxiv.org/abs/2106.09685")
     group.add("--lora_embedding", "-lora_embedding", action='store_true',
               help="replace embeddings with LoRa Embeddings see §5.1")
     group.add('--lora_rank', '-lora_rank', type=int, default=2,
               help="r=2 successfully tested with NLLB-200 3.3B")
     group.add('--lora_alpha', '-lora_alpha', type=int, default=1,
               help="§4.1 https://arxiv.org/abs/2106.09685")
     group.add('--lora_dropout', '-lora_dropout', type=float, default=0.0,
               help="rule of thumb: same value as in main model")
 
+    group.add('--quant_layers', '-quant_layers', default=[], nargs='+',
+              type=str, help="list of layers to be compressed in 8bit.")
+
     _add_reproducibility_opts(parser)
 
     # Init options
     group = parser.add_argument_group('Initialization')
     group.add('--param_init', '-param_init', type=float, default=0.1,
               help="Parameters are initialized over uniform distribution "
                    "with support (-param_init, param_init). "
@@ -785,19 +803,25 @@
     """ Translation / inference options """
     group = parser.add_argument_group('Model')
     group.add('--model', '-model', dest='models', metavar='MODEL',
               nargs='+', type=str, default=[], required=True,
               help="Path to model .pt file(s). "
                    "Multiple models can be specified, "
                    "for ensemble decoding.")
-    group.add('--fp32', '-fp32', action='store_true',
-              help="Force the model to be in FP32 "
-                   "because FP16 is very slow on GTX1080(ti).")
-    group.add('--int8', '-int8', action='store_true',
-              help="Enable dynamic 8-bit quantization (CPU only).")
+    group.add('--precision', '-precision', default='',
+              choices=["", "fp32", "fp16", "int8"],
+              help="Precision to run inference."
+                   "default is model.dtype"
+                   "fp32 to force slow FP16 model on GTX1080"
+                   "int8 enables pytorch native 8-bit quantization"
+                   "(cpu only)")
+    group.add('--fp32', '-fp32', action=DeprecateAction,
+              help="Deprecated use 'precision' instead")
+    group.add('--int8', '-int8', action=DeprecateAction,
+              help="Deprecated use 'precision' instead")
     group.add('--avg_raw_probs', '-avg_raw_probs', action='store_true',
               help="If this is set, during ensembling scores from "
                    "different models will be combined by averaging their "
                    "raw probabilities and then taking the log. Otherwise, "
                    "the log probabilities will be averaged directly. "
                    "Necessary for models whose output layers can assign "
                    "zero probability.")
```

### Comparing `OpenNMT-py-3.1.1/onmt/scorers/__init__.py` & `OpenNMT-py-3.1.2/onmt/scorers/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/scorers/scorer.py` & `OpenNMT-py-3.1.2/onmt/scorers/scorer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_attention.py` & `OpenNMT-py-3.1.2/onmt/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_beam_search.py` & `OpenNMT-py-3.1.2/onmt/tests/test_beam_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_copy_generator.py` & `OpenNMT-py-3.1.2/onmt/tests/test_copy_generator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_data_prepare.py` & `OpenNMT-py-3.1.2/onmt/tests/test_data_prepare.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_embeddings.py` & `OpenNMT-py-3.1.2/onmt/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_events.py` & `OpenNMT-py-3.1.2/onmt/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_greedy_search.py` & `OpenNMT-py-3.1.2/onmt/tests/test_greedy_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_models.py` & `OpenNMT-py-3.1.2/onmt/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_subword_marker.py` & `OpenNMT-py-3.1.2/onmt/tests/test_subword_marker.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_text_utils.py` & `OpenNMT-py-3.1.2/onmt/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_transform.py` & `OpenNMT-py-3.1.2/onmt/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_translation_server.py` & `OpenNMT-py-3.1.2/onmt/tests/test_translation_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,26 +138,30 @@
     def test_run(self):
         model_id = 0
         opt = {"models": ["test_model.pt"]}
         model_root = TEST_DIR
         sm = ServerModel(opt, model_id, model_root=model_root, load=True)
         inp = [{"src": "hello how are you today"},
                {"src": "good morning to you ."}]
-        results, scores, n_best, time, aligns = sm.run(inp)
+        results, scores, n_best, time, aligns, align_scores = sm.run(inp)
         self.assertIsInstance(results, list)
         for sentence_string in results:
             self.assertIsInstance(sentence_string, str)
         self.assertIsInstance(scores, list)
         for elem in scores:
             self.assertIsInstance(elem, float)
         self.assertIsInstance(aligns, list)
         for align_list in aligns:
             for align_string in align_list:
                 if align_string is not None:
                     self.assertIsInstance(align_string, str)
+        for align_scores_list in align_scores:
+            for score_string in align_scores_list:
+                if score_string is not None:
+                    self.assertIsInstance(align_string, str)
         self.assertEqual(len(results), len(scores))
         self.assertEqual(len(scores), len(inp) * n_best)
         self.assertEqual(len(time), 1)
         self.assertIsInstance(time, dict)
         self.assertIn("translation", time)
```

### Comparing `OpenNMT-py-3.1.1/onmt/tests/test_translator.py` & `OpenNMT-py-3.1.2/onmt/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/train_single.py` & `OpenNMT-py-3.1.2/onmt/train_single.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,15 +98,25 @@
         torch.cuda.set_device(device_id)
     set_random_seed(opt.seed, device_id >= 0)
 
 
 def _get_model_opts(opt, checkpoint=None):
     """Get `model_opt` to build model, may load from `checkpoint` if any."""
     if checkpoint is not None:
+        model_opt = ArgumentParser.ckpt_model_opts(checkpoint["opt"])
         if opt.override_opts:
+            logger.info("Over-ride model option set to true - use with care")
+            args = list(opt.__dict__.keys())
+            model_args = list(model_opt.__dict__.keys())
+            for arg in args:
+                if arg in model_args and \
+                        getattr(opt, arg) != getattr(model_opt, arg):
+                    logger.info("Option: %s , value: %s overiding model: %s"
+                                % (arg, getattr(opt, arg),
+                                   getattr(model_opt, arg)))
             model_opt = opt
         else:
             model_opt = ArgumentParser.ckpt_model_opts(checkpoint["opt"])
             ArgumentParser.update_model_opts(model_opt)
             ArgumentParser.validate_model_opts(model_opt)
             if (opt.tensorboard_log_dir == model_opt.tensorboard_log_dir and
                     hasattr(model_opt, 'tensorboard_log_dir_dated')):
```

### Comparing `OpenNMT-py-3.1.1/onmt/trainer.py` & `OpenNMT-py-3.1.2/onmt/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -223,30 +223,24 @@
                 batches = []
                 normalization = 0
         if batches:
             yield batches, normalization
 
     def _update_average(self, step):
         if self.moving_average is None:
-            copy_params = [params.detach().half()
-                           if params.dtype == torch.float16
-                           else params.detach().float()
+            copy_params = [params.detach().float()
                            for params in self.model.parameters()]
             self.moving_average = copy_params
         else:
             average_decay = max(self.average_decay,
                                 1 - (step + 1) / (step + 10))
             for (i, avg), cpt in zip(enumerate(self.moving_average),
                                      self.model.parameters()):
                 self.moving_average[i] = \
                     (1 - average_decay) * avg + \
-                    cpt.detach().half() * average_decay \
-                    if avg.dtype == torch.float16 \
-                    else \
-                    (1 - average_decay) * avg + \
                     cpt.detach().float() * average_decay
 
     def train(self,
               train_iter,
               train_steps,
               save_checkpoint_steps=5000,
               valid_iter=None,
@@ -502,16 +496,14 @@
                                     metric, self.train_scorers[
                                         metric]["value"]))
                             computed_metrics[
                                 metric] = self.train_scorers[metric]["value"]
                         batch_stats.computed_metrics = computed_metrics
 
                     if loss is not None:
-                        # in theory we should divide by accum_count and bptt
-                        # to rescale for each sub batch
                         loss /= normalization
                         self.optim.backward(loss)
 
                     total_stats.update(batch_stats)
                     report_stats.update(batch_stats)
 
                 except Exception as exc:
@@ -520,39 +512,27 @@
                         logger.info("Step %d, cuda OOM - batch removed",
                                     self.optim.training_step)
                         torch.cuda.empty_cache()
                     else:
                         traceback.print_exc()
                         raise exc
 
-                # 4. Update the parameters and statistics.
-                if self.accum_count == 1:
-                    # Multi GPU gradient gather
-                    if self.n_gpu > 1:
-                        grads = [p.grad.data for p in self.model.parameters()
-                                 if p.requires_grad
-                                 and p.grad is not None]
-                        onmt.utils.distributed.all_reduce_and_rescale_tensors(
-                            grads, float(self.n_gpu))
-                    self.optim.step()
-
                 # If truncated, don't backprop fully.
                 if self.model.decoder.state != {}:
                     self.model.decoder.detach_state()
 
         # in case of multi step gradient accumulation,
         # update only after accum batches
-        if self.accum_count > 1:
-            if self.n_gpu > 1:
-                grads = [p.grad.data for p in self.model.parameters()
-                         if p.requires_grad
-                         and p.grad is not None]
-                onmt.utils.distributed.all_reduce_and_rescale_tensors(
-                    grads, float(self.n_gpu))
-            self.optim.step()
+        if self.n_gpu > 1:
+            grads = [p.grad.data for p in self.model.parameters()
+                     if p.requires_grad
+                     and p.grad is not None]
+            onmt.utils.distributed.all_reduce_and_rescale_tensors(
+                grads, float(self.n_gpu))
+        self.optim.step()
 
     def _start_report_manager(self, start_time=None):
         """Simple function to start report manager (if any)"""
 
         if self.report_manager is not None:
             if start_time is None:
                 self.report_manager.start()
```

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/__init__.py` & `OpenNMT-py-3.1.2/onmt/transforms/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def get_transforms_cls(transform_names):
     """Return valid transform class indicated in `transform_names`."""
     transforms_cls = {}
     for name in transform_names:
         if name not in AVAILABLE_TRANSFORMS:
-            raise ValueError("specified tranform not supported!")
+            raise ValueError("%s transform not supported!" % name)
         transforms_cls[name] = AVAILABLE_TRANSFORMS[name]
     return transforms_cls
 
 
 __all__ = ["get_transforms_cls", "get_specials", "make_transforms",
            "load_transforms", "save_transforms", "TransformPipe",
            "prepare_transforms"]
```

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/bart.py` & `OpenNMT-py-3.1.2/onmt/transforms/bart.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/docify.py` & `OpenNMT-py-3.1.2/onmt/transforms/docify.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/features.py` & `OpenNMT-py-3.1.2/onmt/transforms/features.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/fuzzymatch.py` & `OpenNMT-py-3.1.2/onmt/transforms/fuzzymatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,20 @@
                 # Filter out very short or very long sentences
                 # from the TM for better performance
                 if len(source) < self.tm_unit_min_length or \
                         len(source) > self.tm_unit_max_length:
                     continue
                 src_segments.append(source.strip())
                 tgt_segments.append(target.strip())
-        logger.info(f'Translation Memory size for FuzzyMatch transform: '
-                    f'{len(src_segments)}')
+        logger.debug(f'Translation Memory size for FuzzyMatch transform: '
+                     f'{len(src_segments)}')
         return [src_segments, tgt_segments]
 
     def _get_batch_matches(self, batch):
-        logger.info(f'Starting fuzzy matching on {len(batch)} examples')
+        logger.debug(f'Starting fuzzy matching on {len(batch)} examples')
         fuzzy_count = 0
         start = time.time()
         augmented = list()
 
         # We split the `batch` and perform fuzzy matching
         # in smaller chunks of 10.000 examples in order to
         # reduce memory usage.
@@ -90,16 +90,16 @@
                         break
                     plist[idx] = s + self.fuzzy_token + \
                         self.internal_tm[1][argmax[idx]]
                     fuzzy_count += 1
             augmented.extend(plist)
 
         end = time.time()
-        logger.info(f'FuzzyMatch Transform: Added {fuzzy_count} '
-                    f'fuzzies in {end-start} secs')
+        logger.debug(f'FuzzyMatch Transform: Added {fuzzy_count} '
+                     f'fuzzies in {end-start} secs')
 
         return augmented
 
 
 @register_transform(name='fuzzymatch')
 class FuzzyMatchTransform(Transform):
     """Perform fuzzy matching against a translation memory and
```

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/inlinetags.py` & `OpenNMT-py-3.1.2/onmt/transforms/inlinetags.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     def __init__(self, tags_dictionary_path, max_tags,
                  paired_start_tag,
                  paired_end_tag,
                  isolated_tag,
                  src_delimiter,
                  tag_corpus_ratio=0.1):
         self.max_tags = max_tags
-        self.tagged_examples = 0
-        self.processed_examples = 0
         self.tag_corpus_ratio = tag_corpus_ratio
         self.src_delimiter = src_delimiter
         self.internal_dictionary = self._create_internal_dictionary(
             tags_dictionary_path
         )
         self.paired_stag_prefix, self.paired_stag_suffix = \
             map(str, paired_start_tag.split("#"))
@@ -38,22 +36,22 @@
             map(str, paired_end_tag.split("#"))
         self.isolated_tag_prefix, self.isolated_tag_suffix = \
             map(str, isolated_tag.split("#"))
 
         self.automaton = self._create_automaton()
 
     def _create_internal_dictionary(self, tags_dictionary_path):
-        logger.info('Creating tag dictionary for tagging transform...')
+        logger.debug('Creating tag dictionary for tagging transform...')
         dictionary = list()
         with open(tags_dictionary_path, mode='r', encoding='utf-8') as file:
             pairs = file.readlines()
             for pair in pairs:
                 src_term, tgt_term = map(str, pair.split('\t'))
                 dictionary.append((src_term.strip(), tgt_term.strip()))
-        logger.info(f'Created tag dictionary with {len(dictionary)} entries.')
+        logger.debug(f'Created tag dictionary with {len(dictionary)} entries.')
         return dictionary
 
     def _create_automaton(self):
         automaton = ahocorasick.Automaton()
         for entry in self.internal_dictionary:
             automaton.add_word(entry[0], (entry[0], entry[1]))
 
@@ -144,36 +142,40 @@
                 )
                 tgt_term = ' '.join(
                     tokenized_target_string[
                         target_index: target_index + len(pair[1].split())
                     ]
                 )
 
+                # Create all possible tag forms. We inject a special
+                # unicode char (∥) as a placeholder for whitespace in order
+                # to keep the indices unaltered. This char is replaced with
+                # spaces before we return the augmented examples.
                 src_single_tags = (
                     f'{source_only[src_offset: src_match_start]}'
                     f'{self.isolated_tag_prefix}{single_tag_start_num}'
-                    f'{self.isolated_tag_suffix}{src_term}'
+                    f'{self.isolated_tag_suffix}∥{src_term}∥'
                 )
                 src_paired_tags = (
                     f'{source_only[src_offset: src_match_start]}'
                     f'{self.paired_stag_prefix}{paired_tag_start_num}'
-                    f'{self.paired_stag_suffix}{src_term}'
+                    f'{self.paired_stag_suffix}∥{src_term}∥'
                     f'{self.paired_etag_prefix}{paired_tag_start_num}'
                     f'{self.paired_etag_suffix}'
                 )
 
                 tgt_single_tags = (
                     f'{tgt_example[tgt_offset: tgt_match_start]}'
                     f'{self.isolated_tag_prefix}{single_tag_start_num}'
-                    f'{self.isolated_tag_suffix}{tgt_term}'
+                    f'{self.isolated_tag_suffix}∥{tgt_term}∥'
                 )
                 tgt_paired_tags = (
                     f'{tgt_example[tgt_offset: tgt_match_start]}'
                     f'{self.paired_stag_prefix}{paired_tag_start_num}'
-                    f'{self.paired_stag_suffix}{tgt_term}'
+                    f'{self.paired_stag_suffix}∥{tgt_term}∥'
                     f'{self.paired_etag_prefix}{paired_tag_start_num}'
                     f'{self.paired_etag_suffix}'
                 )
 
                 # Make a weighted choice between paired tags or single tags.
                 # We usually encounter, and thus here we favor, paired tags
                 # with a ratio 1/3.
@@ -190,29 +192,27 @@
                 else:
                     tgt_with_tags.append(tgt_paired_tags)
                     paired_tag_start_num += 1
 
                 tgt_offset = tgt_match_end + 1
                 tag_counter += 1
                 is_match = True
-        self.processed_examples += 1
         if is_match:
-            self.tagged_examples += 1
             if augmented_part is not None:
                 src_with_tags.append(source_only[src_offset:] +
                                      self.src_delimiter +
                                      augmented_part)
             else:
                 src_with_tags.append(source_only[src_offset:])
 
             tgt_with_tags.append(tgt_example[tgt_offset:])
 
             return (
-                ''.join(src_with_tags).split(),
-                ''.join(tgt_with_tags).split(),
+                ''.join(src_with_tags).replace('∥', ' ').split(),
+                ''.join(tgt_with_tags).replace('∥', ' ').split(),
             )
         else:
             return (src_example.split(), tgt_example.split())
 
 
 @register_transform(name='inlinetags')
 class InlineTagsTransform(Transform):
@@ -251,14 +251,17 @@
                   "FuzzyMatch transform.")
 
     def _parse_opts(self):
         self.tags_dictionary_path = self.opts.tags_dictionary_path
         self.tags_corpus_ratio = self.opts.tags_corpus_ratio
         self.max_tags = self.opts.max_tags
         self.src_delimiter = self.opts.src_delimiter
+        self.paired_stag = self.opts.paired_stag,
+        self.paired_etag = self.opts.paired_etag,
+        self.isolated_tag = self.opts.isolated_tag,
 
     @classmethod
     def get_specials(cls, opts):
         """Add up to self.max_tags * 2 placeholders to src and tgt vocabs."""
 
         # Check if the tags include the
         # mandatory "#" number placeholder"
@@ -291,26 +294,24 @@
 
     def warm_up(self, vocabs=None):
         """Create the tagger."""
 
         super().warm_up(None)
         self.tagger = InlineTagger(self.tags_dictionary_path,
                                    self.max_tags,
-                                   self.opts.paired_stag,
-                                   self.opts.paired_etag,
-                                   self.opts.isolated_tag,
+                                   self.paired_stag,
+                                   self.paired_etag,
+                                   self.isolated_tag,
                                    self.src_delimiter,
                                    self.tags_corpus_ratio)
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Add tags (placeholders) to source and target segments."""
 
-        if self.tagger.processed_examples > 0 and \
-                self.tagger.tagged_examples/self.tagger.processed_examples \
-                > self.tags_corpus_ratio:
+        if random.random() > self.tags_corpus_ratio:
             return example
 
         src_tgt_pair = self.tagger._tagged_src_tgt(
             ' '.join(example['src']), ' '.join(example['tgt'])
         )
         example['src'] = src_tgt_pair[0]
         example['tgt'] = src_tgt_pair[1]
```

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/misc.py` & `OpenNMT-py-3.1.2/onmt/transforms/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,27 +91,27 @@
         """Get all needed prefix correspond to corpus in `opts`."""
         prefix_dict = {}
         # prefix src/tgt for each dataset
         if hasattr(opts, 'data'):
             for c_name, corpus in opts.data.items():
                 prefix = cls._get_prefix(corpus)
                 if prefix is not None:
-                    logger.info(f"Get prefix for {c_name}: {prefix}")
+                    logger.debug(f"Get prefix for {c_name}: {prefix}")
                     prefix_dict[c_name] = prefix
         # prefix as general option for inference
         if hasattr(opts, 'src_prefix'):
             if 'infer' not in prefix_dict.keys():
                 prefix_dict['infer'] = {}
             prefix_dict['infer']['src'] = opts.src_prefix
-            logger.info(f"Get prefix for src infer: {opts.src_prefix}")
+            logger.debug(f"Get prefix for src infer: {opts.src_prefix}")
         if hasattr(opts, 'tgt_prefix'):
             if 'infer' not in prefix_dict.keys():
                 prefix_dict['infer'] = {}
             prefix_dict['infer']['tgt'] = opts.tgt_prefix
-            logger.info(f"Get prefix for tgt infer: {opts.tgt_prefix}")
+            logger.debug(f"Get prefix for tgt infer: {opts.tgt_prefix}")
 
         return prefix_dict
 
     @classmethod
     def get_specials(cls, opts):
         """Get special vocabs added by prefix transform."""
         prefix_dict = cls.get_prefix_dict(opts)
@@ -197,27 +197,27 @@
         """Get all needed suffix correspond to corpus in `opts`."""
         suffix_dict = {}
         # suffix src/tgt for each dataset
         if hasattr(opts, 'data'):
             for c_name, corpus in opts.data.items():
                 suffix = cls._get_suffix(corpus)
                 if suffix is not None:
-                    logger.info(f"Get suffix for {c_name}: {suffix}")
+                    logger.debug(f"Get suffix for {c_name}: {suffix}")
                     suffix_dict[c_name] = suffix
         # suffix as general option for inference
         if hasattr(opts, 'src_suffix'):
             if 'infer' not in suffix_dict.keys():
                 suffix_dict['infer'] = {}
             suffix_dict['infer']['src'] = opts.src_suffix
-            logger.info(f"Get suffix for src infer: {opts.src_suffix}")
+            logger.debug(f"Get suffix for src infer: {opts.src_suffix}")
         if hasattr(opts, 'tgt_suffix'):
             if 'infer' not in suffix_dict.keys():
                 suffix_dict['infer'] = {}
             suffix_dict['infer']['tgt'] = opts.tgt_suffix
-            logger.info(f"Get suffix for tgt infer: {opts.tgt_suffix}")
+            logger.debug(f"Get suffix for tgt infer: {opts.tgt_suffix}")
 
         return suffix_dict
 
     @classmethod
     def get_specials(cls, opts):
         """Get special vocabs added by suffix transform."""
         suffix_dict = cls.get_suffix_dict(opts)
```

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/sampling.py` & `OpenNMT-py-3.1.2/onmt/transforms/sampling.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/tokenize.py` & `OpenNMT-py-3.1.2/onmt/transforms/tokenize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Transforms relate to tokenization/subword."""
 import re
 from onmt.utils.logging import logger
 from onmt.transforms import register_transform
 from .transform import Transform, ObservableStats
+from onmt.constants import DefaultTokens
 
 
 class TokenizerTransform(Transform):
     """Tokenizer transform abstract class."""
 
     def __init__(self, opts):
         """Initialize necessary options for Tokenizer."""
@@ -166,34 +167,39 @@
                 'src': load_src_model,
                 'tgt': load_tgt_model
             }
 
     def _tokenize(self, tokens, side='src', is_train=False):
         """Do sentencepiece subword tokenize."""
         sp_model = self.load_models[side]
-        sentence = ' '.join(tokens)
-        nbest_size = self.tgt_subword_nbest if side == 'tgt' else \
-            self.src_subword_nbest
-        if is_train is False or nbest_size in [0, 1]:
-            # derterministic subwording
-            segmented = sp_model.encode(sentence, out_type=str)
-        else:
-            # subword sampling when nbest_size > 1 or -1
-            # alpha should be 0.0 < alpha < 1.0
-            alpha = self.tgt_subword_alpha if side == 'tgt' else \
-                self.src_subword_alpha
-            segmented = sp_model.encode(
-                sentence, out_type=str, enable_sampling=True,
-                alpha=alpha, nbest_size=nbest_size)
-        return segmented
+        sentence = ' '.join(tokens).replace(DefaultTokens.SEP, '\n')
+        sent_list = sentence.split(DefaultTokens.EOS)
+        segmented = []
+        for sentence in sent_list:
+            nbest_size = self.tgt_subword_nbest if side == 'tgt' else \
+                self.src_subword_nbest
+            if is_train is False or nbest_size in [0, 1]:
+                # derterministic subwording
+                segmented += sp_model.encode(sentence, out_type=str)
+            else:
+                # subword sampling when nbest_size > 1 or -1
+                # alpha should be 0.0 < alpha < 1.0
+                alpha = self.tgt_subword_alpha if side == 'tgt' else \
+                    self.src_subword_alpha
+                segmented += sp_model.encode(
+                    sentence, out_type=str, enable_sampling=True,
+                    alpha=alpha, nbest_size=nbest_size)
+            segmented += [DefaultTokens.EOS]
+
+        return segmented[:-1]
 
     def _detokenize(self, tokens, side="src"):
         """Apply SentencePiece Detokenizer"""
         sp_model = self.load_models[side]
-        return sp_model.DecodePieces(tokens)
+        return sp_model.DecodePieces(tokens).replace('\n', DefaultTokens.SEP)
 
     def apply(self, example, is_train=False, stats=None, **kwargs):
         """Apply sentencepiece subword encode to src & tgt."""
         src_out = self._tokenize(example['src'], 'src', is_train)
         if example['tgt'] is not None:
             tgt_out = self._tokenize(example['tgt'], 'tgt', is_train)
             if stats is not None:
@@ -358,17 +364,17 @@
         opts.src_onmttok_kwargs = src_kwargs_dict
         opts.tgt_onmttok_kwargs = tgt_kwargs_dict
 
     def _parse_opts(self):
         super()._parse_opts()
         self.src_subword_type = self.opts.src_subword_type
         self.tgt_subword_type = self.opts.tgt_subword_type
-        logger.info("Parsed pyonmttok kwargs for src: {}".format(
+        logger.debug("Parsed pyonmttok kwargs for src: {}".format(
             self.opts.src_onmttok_kwargs))
-        logger.info("Parsed pyonmttok kwargs for tgt: {}".format(
+        logger.debug("Parsed pyonmttok kwargs for tgt: {}".format(
             self.opts.tgt_onmttok_kwargs))
         self.src_other_kwargs = self.opts.src_onmttok_kwargs
         self.tgt_other_kwargs = self.opts.tgt_onmttok_kwargs
 
     @classmethod
     def get_specials(cls, opts):
         src_specials, tgt_specials = [], []
@@ -401,15 +407,15 @@
             kwopts['bpe_model_path'] = subword_model
             kwopts['bpe_dropout'] = subword_alpha
         elif subword_type == 'sentencepiece':
             kwopts['sp_model_path'] = subword_model
             kwopts['sp_nbest_size'] = subword_nbest
             kwopts['sp_alpha'] = subword_alpha
         else:
-            logger.warning('No subword method will be applied.')
+            logger.debug('No subword method will be applied.')
         vocabulary_threshold = self.tgt_vocab_threshold if side == 'tgt' \
             else self.src_vocab_threshold
         vocabulary_path = self.tgt_subword_vocab if side == 'tgt' \
             else self.src_subword_vocab
         if vocabulary_threshold > 0 and vocabulary_path != "":
             kwopts['vocabulary_path'] = vocabulary_path
             kwopts['vocabulary_threshold'] = vocabulary_threshold
```

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/transform.py` & `OpenNMT-py-3.1.2/onmt/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/transforms/uppercase.py` & `OpenNMT-py-3.1.2/onmt/transforms/uppercase.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/translate/__init__.py` & `OpenNMT-py-3.1.2/onmt/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/translate/beam_search.py` & `OpenNMT-py-3.1.2/onmt/translate/beam_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/translate/decode_strategy.py` & `OpenNMT-py-3.1.2/onmt/translate/decode_strategy.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/translate/greedy_search.py` & `OpenNMT-py-3.1.2/onmt/translate/greedy_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/translate/penalties.py` & `OpenNMT-py-3.1.2/onmt/translate/penalties.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/translate/process_zh.py` & `OpenNMT-py-3.1.2/onmt/translate/process_zh.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/translate/translation.py` & `OpenNMT-py-3.1.2/onmt/translate/translation.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/translate/translation_server.py` & `OpenNMT-py-3.1.2/onmt/translate/translation_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,23 +165,26 @@
         predictions = [[" ".join(item["tokens"]) for item in ex]
                        for ex in preds]
         if self.report_align:
             attentions = [[torch.Tensor(item["attention"]) for item in ex]
                           for ex in preds]
             align_pharaohs = [[build_align_pharaoh(item) for item in ex]
                               for ex in attentions]
-            aligns = [[' '.join(item) for item in ex]
+            aligns = [[' '.join(item[0]) for item in ex]
                       for ex in align_pharaohs]
+            align_scores = [[' '.join(item[1]) for item in ex]
+                            for ex in align_pharaohs]
             predictions = [
                 [
                     pred + DefaultTokens.ALIGNMENT_SEPARATOR + align
-                    for pred, align in zip(*item)
+                    + DefaultTokens.ALIGNMENT_SEPARATOR + align_score
+                    for pred, align, align_score in zip(*item)
                 ]
                 for item in zip(
-                    predictions, aligns
+                    predictions, aligns, align_scores
                 )
             ]
         return scores, predictions
 
     def to_cpu(self):
         self.translator.unload_model(to_cpu=True)
 
@@ -610,62 +613,76 @@
         def maybe_item(x): return x.item() if type(x) is torch.Tensor else x
         scores = [maybe_item(score_tensor)
                   for score_tensor in flatten_list(scores)]
 
         results = [self.maybe_detokenize_with_align(result, src)
                    for result, src in zip(results, tiled_texts)]
 
-        aligns = [align for _, align in results]
+        aligns = [align[0] if align is not None else None
+                  for _, align in results]
+        align_scores = [align[1] if align is not None else None
+                        for _, align in results]
         results = [tokens for tokens, _ in results]
 
         # build back results with empty texts
         for i in empty_indices:
             j = i * self.opt.n_best
             results = results[:j] + [""] * self.opt.n_best + results[j:]
             aligns = aligns[:j] + [None] * self.opt.n_best + aligns[j:]
+            align_scores = (align_scores[:j] + [None] *
+                            self.opt.n_best + align_scores[j:])
             scores = scores[:j] + [0] * self.opt.n_best + scores[j:]
 
-        rebuilt_segs, scores, aligns = self.rebuild_seg_packages(
-            all_preprocessed, results, scores, aligns, self.opt.n_best)
+        rebuilt_segs, scores, aligns, align_scores = self.rebuild_seg_packages(
+            all_preprocessed, results, scores,
+            aligns, align_scores, self.opt.n_best)
 
         results = [self.maybe_postprocess(seg) for seg in rebuilt_segs]
 
         head_spaces = [h for h in head_spaces for i in range(self.opt.n_best)]
         tail_spaces = [h for h in tail_spaces for i in range(self.opt.n_best)]
         results = ["".join(items)
                    for items in zip(head_spaces, results, tail_spaces)]
 
         self.logger.info("Translation Results: %d", len(results))
 
-        return results, scores, self.opt.n_best, timer.times, aligns
+        return (results, scores, self.opt.n_best, timer.times,
+                aligns, align_scores)
 
     def rebuild_seg_packages(self, all_preprocessed, results,
-                             scores, aligns, n_best):
+                             scores, aligns, align_scores, n_best):
         """Rebuild proper segment packages based on initial n_seg."""
 
         offset = 0
         rebuilt_segs = []
         avg_scores = []
         merged_aligns = []
+        merged_align_scores = []
         for i, seg_dict in enumerate(all_preprocessed):
             n_seg = seg_dict["n_seg"]
             sub_results = results[n_best * offset: (offset + n_seg) * n_best]
             sub_scores = scores[n_best * offset: (offset + n_seg) * n_best]
             sub_aligns = aligns[n_best * offset: (offset + n_seg) * n_best]
+            sub_align_scores = align_scores[
+                n_best * offset: (offset + n_seg) * n_best
+            ]
             for j in range(n_best):
                 _seg_dict = deepcopy(seg_dict)
                 _seg_dict["seg"] = list(islice(sub_results, j, None, n_best))
                 rebuilt_segs.append(_seg_dict)
                 sub_sub_scores = list(islice(sub_scores, j, None, n_best))
                 avg_score = sum(sub_sub_scores)/n_seg if n_seg != 0 else 0
                 avg_scores.append(avg_score)
                 sub_sub_aligns = list(islice(sub_aligns, j, None, n_best))
                 merged_aligns.append(sub_sub_aligns)
+                sub_sub_align_scores = list(islice(sub_align_scores, j,
+                                                   None, n_best))
+                merged_align_scores.append(sub_sub_align_scores)
             offset += n_seg
-        return rebuilt_segs, avg_scores, merged_aligns
+        return rebuilt_segs, avg_scores, merged_aligns, merged_align_scores
 
     def do_timeout(self):
         """Timeout function that frees GPU memory.
 
         Moves the model to CPU or unloads it; depending on
         attr ``self.on_timemout`` value"""
 
@@ -875,17 +892,19 @@
             sequence (str): The detokenized sequence.
             align (str): The alignment correspand to detokenized src/tgt
             sorted or None if no alignment in output."""
 
         align = None
         if self.opt.report_align:
             # output contain alignment
-            sequence, align = sequence.split(DefaultTokens.ALIGNMENT_SEPARATOR)
+            sequence, align, align_scores = sequence.split(
+                DefaultTokens.ALIGNMENT_SEPARATOR)
             if align != '':
-                align = self.maybe_convert_align(src, sequence, align)
+                align = self.maybe_convert_align(src, sequence,
+                                                 align, align_scores)
         sequence = self.maybe_detokenize(sequence, side)
         return (sequence, align)
 
     def maybe_detokenize(self, sequence, side='tgt'):
         """De-tokenize the sequence (or not)
         Same args/returns as :func:``tokenize()``"""
 
@@ -904,15 +923,15 @@
         if self.tokenizers_opt[side]["type"] == "sentencepiece":
             detok = self.tokenizers[side].DecodePieces(sequence.split())
         elif self.tokenizers_opt[side]["type"] == "pyonmttok":
             detok = self.tokenizers[side].detokenize(sequence.split())
 
         return detok
 
-    def maybe_convert_align(self, src, tgt, align):
+    def maybe_convert_align(self, src, tgt, align, align_scores):
         """Convert alignment to match detokenized src/tgt (or not).
 
         Args:
             src (str): The tokenized source sequence.
             tgt (str): The tokenized target sequence.
             align (str): The alignment correspand to src/tgt pair.
 
@@ -923,15 +942,16 @@
         if self.tokenizers_opt is not None:
             src_marker = self.tokenizer_marker(side='src')
             tgt_marker = self.tokenizer_marker(side='tgt')
             if src_marker is None or tgt_marker is None:
                 raise ValueError("To get decoded alignment, joiner/spacer "
                                  "should be used in both side's tokenizer.")
             elif ''.join(tgt.split()) != '':
-                align = to_word_align(src, tgt, align, src_marker, tgt_marker)
+                align = to_word_align(src, tgt, align, align_scores,
+                                      src_marker, tgt_marker)
         return align
 
     def maybe_postprocess(self, sequence):
         """Postprocess the sequence (or not)"""
 
         if self.postprocess_opt is not None:
             return self.postprocess(sequence)
```

### Comparing `OpenNMT-py-3.1.1/onmt/translate/translator.py` & `OpenNMT-py-3.1.2/onmt/translate/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,31 +344,24 @@
         gold_score_total, gold_words_total = 0, 0
 
         all_scores = []
         all_predictions = []
 
         start_time = time.time()
 
-        for batch in infer_iter:
-
-            batch_data = self.translate_batch(
-                batch, attn_debug
-            )
-
-            translations = xlation_builder.from_batch(batch_data)
-
-            # Here we handle the cases of mismatch in number of segments
-            # between source and target. We re-translate seg by seg.
+        def _maybe_retranslate(translations, batch):
+            """Here we handle the cases of mismatch in number of segments
+               between source and target. We re-translate seg by seg."""
             inds, perm = torch.sort(batch['indices'])
             trans_copy = deepcopy(translations)
             inserted_so_far = 0
             for j, trans in enumerate(translations):
                 if (trans.src_raw.count(DefaultTokens.SEP) !=
                         trans.pred_sents[0].count(DefaultTokens.SEP)):
-                    self._log("Mismatch in ((newline)) retranslating")
+                    self._log("Mismatch in number of ((newline))")
                     # those two should be the same except feat dim
                     # batch['src'][perm[j], :, :])
                     # trans.src
 
                     # we rebuild a small batch made of the sub-segments
                     # in the long segment.
                     idx = (trans.src == self._tgt_sep_idx).nonzero()
@@ -395,27 +388,37 @@
                     t_sub_src_ind = torch.tensor([i for i in
                                                   range(len(sub_src))],
                                                  dtype=torch.int16)
                     device = batch['src'].device
                     t_sub_batch = {'src': t_sub_src.to(device),
                                    'srclen': t_sub_src_len.to(device),
                                    'indices': t_sub_src_ind.to(device)}
-
                     # new sub-batch ready to be translated
                     sub_data = self.translate_batch(t_sub_batch, attn_debug)
                     sub_trans = xlation_builder.from_batch(sub_data)
 
                     # we re-insert the sub-batch in the initial translations
                     trans_copy[j + inserted_so_far] = sub_trans[0]
                     for i in range(1, len(sub_src)):
                         trans_copy.insert(j + i + inserted_so_far,
                                           sub_trans[i])
                     inserted_so_far += len(sub_src) - 1
+            return trans_copy
 
-            for j, trans in enumerate(trans_copy):
+        for batch in infer_iter:
+
+            batch_data = self.translate_batch(
+                batch, attn_debug
+            )
+
+            translations = xlation_builder.from_batch(batch_data)
+            if not isinstance(self, GeneratorLM):
+                translations = _maybe_retranslate(translations, batch)
+
+            for j, trans in enumerate(translations):
                 all_scores += [trans.pred_scores[: self.n_best]]
                 pred_score_total += trans.pred_scores[0]
                 pred_words_total += len(trans.pred_sents[0])
                 if 'tgt' in batch.keys():
                     gold_score_total += trans.gold_score
                     gold_words_total += len(trans.gold_sent) + 1
```

### Comparing `OpenNMT-py-3.1.1/onmt/utils/__init__.py` & `OpenNMT-py-3.1.2/onmt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/utils/alignment.py` & `OpenNMT-py-3.1.2/onmt/utils/alignment.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,25 +70,31 @@
 
 
 def build_align_pharaoh(valid_alignment):
     """Convert valid alignment matrix to i-j (from 0) Pharaoh format pairs,
     or empty list if it's None.
     """
     align_pairs = []
+    align_scores = []
     if isinstance(valid_alignment, torch.Tensor):
         tgt_align_src_id = valid_alignment.argmax(dim=-1)
-
+        align_scores = torch.divide(valid_alignment.max(dim=-1).values,
+                                    valid_alignment.sum(dim=-1))
         for tgt_id, src_id in enumerate(tgt_align_src_id.tolist()):
             align_pairs.append(str(src_id) + "-" + str(tgt_id))
+        align_scores = ["{0}-{1:.5f}".format(i, s)
+                        for i, s in enumerate(align_scores.tolist())]
         align_pairs.sort(key=lambda x: int(x.split('-')[-1]))  # sort by tgt_id
         align_pairs.sort(key=lambda x: int(x.split('-')[0]))  # sort by src_id
-    return align_pairs
+        print(align_scores)
+    return align_pairs, align_scores
 
 
-def to_word_align(src, tgt, subword_align, m_src='joiner', m_tgt='joiner'):
+def to_word_align(src, tgt, subword_align, subword_align_scores,
+                  m_src='joiner', m_tgt='joiner'):
     """Convert subword alignment to word alignment.
 
     Args:
         src (string): tokenized sentence in source language.
         tgt (string): tokenized sentence in target language.
         subword_align (string): align_pharaoh correspond to src-tgt.
         m_src (string): tokenization mode used in src,
@@ -103,25 +109,38 @@
     assert m_src in ["joiner", "spacer"], "Invalid value for argument m_src!"
     assert m_tgt in ["joiner", "spacer"], "Invalid value for argument m_tgt!"
 
     src, tgt = src.strip().split(), tgt.strip().split()
     subword_align = {(int(a), int(b)) for a, b in (x.split("-")
                      for x in subword_align.split())}
 
+    subword_align_scores = dict((int(a), float(b)) for a, b in (x.split("-")
+                                for x in subword_align_scores.split()))
+
     src_map = (subword_map_by_spacer(src) if m_src == 'spacer'
                else subword_map_by_joiner(src))
 
     tgt_map = (subword_map_by_spacer(tgt) if m_tgt == 'spacer'
                else subword_map_by_joiner(tgt))
 
     word_align = list({"{}-{}".format(src_map[a], tgt_map[b])
                        for a, b in subword_align})
+
+    word_align_scores = list(
+        {"{}-{}".format(tgt_map[a],
+                        subword_align_scores[a])
+         for a in subword_align_scores.keys()}
+    )
+
     word_align.sort(key=lambda x: int(x.split('-')[-1]))  # sort by tgt_id
     word_align.sort(key=lambda x: int(x.split('-')[0]))  # sort by src_id
-    return " ".join(word_align)
+
+    word_align_scores.sort(key=lambda x: int(x.split('-')[0]))
+
+    return " ".join(word_align), " ".join(word_align_scores)
 
 
 # Helper functions
 def begin_uppercase(token):
     return token == SubwordMarker.BEGIN_UPPERCASE
```

### Comparing `OpenNMT-py-3.1.1/onmt/utils/cnn_factory.py` & `OpenNMT-py-3.1.2/onmt/utils/cnn_factory.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/utils/distributed.py` & `OpenNMT-py-3.1.2/onmt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/utils/earlystopping.py` & `OpenNMT-py-3.1.2/onmt/utils/earlystopping.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/utils/logging.py` & `OpenNMT-py-3.1.2/onmt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/utils/loss.py` & `OpenNMT-py-3.1.2/onmt/utils/loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,16 +265,20 @@
             A tuple with the loss and a :obj:`onmt.utils.Statistics` instance.
         """
         if trunc_size is None:
             trunc_size = batch['tgt'].size(1) - trunc_start
         # take into account here the tgt_shift_index (0 / 1 = LM/NMT)
         trunc_range = (trunc_start + self.tgt_shift_index,
                        trunc_start + trunc_size)
+
         target = batch['tgt'][:, trunc_range[0]:trunc_range[1],
                               :]
+        output = output[:, trunc_start:trunc_range[1],
+                        :].contiguous()
+
         flat_tgt = target[:, :, 0].contiguous().view(-1)
 
         if self.copy_attn:
             align = batch['alignment'][
                 :, trunc_range[0]:trunc_range[1]
                 ].contiguous().view(-1)
             loss, scores = self._compute_copy_loss(batch, output, flat_tgt,
@@ -328,15 +332,16 @@
             lm_loss = self._compute_lm_loss_ct2(output, batch['tgt'])
             loss = loss + lm_loss * self.lm_prior_lambda
 
         if self.lm_prior_model is not None:
             lm_loss = self._compute_lm_loss(output, batch['tgt'])
             loss = loss + lm_loss * self.lm_prior_lambda
 
-        stats = self._stats(len(batch['srclen']), loss.sum().item(),
+        n_sents = len(batch['srclen']) if trunc_start == 0 else 0
+        stats = self._stats(n_sents, loss.sum().item(),
                             scores, flat_tgt)
 
         return loss, stats
 
     def _stats(self, bsz, loss, scores, target):
         """
         Args:
@@ -347,14 +352,15 @@
         Returns:
             :obj:`onmt.utils.Statistics` : statistics for this batch.
         """
         pred = scores.max(1)[1]
         non_padding = target.ne(self.padding_idx)
         num_correct = pred.eq(target).masked_select(non_padding).sum().item()
         num_non_padding = non_padding.sum().item()
+        n_batchs = 1 if bsz else 0
         # in the case criterion reduction is None then we need
         # to sum the loss of each sentence in the batch
         return onmt.utils.Statistics(loss=loss,
-                                     n_batchs=1,
+                                     n_batchs=n_batchs,
                                      n_sents=bsz,
                                      n_words=num_non_padding,
                                      n_correct=num_correct)
```

### Comparing `OpenNMT-py-3.1.1/onmt/utils/misc.py` & `OpenNMT-py-3.1.2/onmt/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     """Check if `path` exists, makedirs if not else warning/IOError."""
     if os.path.exists(path):
         if exist_ok:
             log(f"path {path} exists, may overwrite...")
         else:
             raise IOError(f"path {path} exists, stop.")
     else:
-        os.makedirs(os.path.dirname(path), exist_ok=True)
+        if os.path.dirname(path) != '':
+            os.makedirs(os.path.dirname(path), exist_ok=True)
 
 
 def sequence_mask(lengths, max_len=None):
     """
     Creates a boolean mask from sequence lengths.
     """
     batch_size = lengths.numel()
```

### Comparing `OpenNMT-py-3.1.1/onmt/utils/optimizers.py` & `OpenNMT-py-3.1.2/onmt/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/utils/parse.py` & `OpenNMT-py-3.1.2/onmt/utils/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             if path_src is None:
                 raise ValueError(f'Corpus {cname} src path is required.'
                                  'tgt path is also required for non language'
                                  ' modeling tasks.')
             else:
                 opt.data_task = ModelTask.SEQ2SEQ
                 if path_tgt is None:
-                    logger.warning(
+                    logger.debug(
                         "path_tgt is None, it should be set unless the task"
                         " is language modeling"
                     )
                     opt.data_task = ModelTask.LANGUAGE_MODEL
                     # tgt is src for LM task
                     corpus["path_tgt"] = path_src
                     corpora[cname] = corpus
@@ -266,14 +266,23 @@
             assert (
                 (model_opt.feat_vec_size * model_opt.n_src_feats)
                 + model_opt.src_word_vec_size == model_opt.hidden_size), \
                 "(feat_vec_size * n_src_feats) + " \
                 "src_word_vec_size should be equal to hidden_size with " \
                 "-feat_merge concat mode."
 
+        if model_opt.position_encoding and \
+                model_opt.max_relative_positions != 0:
+            raise ValueError(
+                "Cannot use absolute and relative position encoding at the"
+                "same time. Use either --position_encoding=true for legacy"
+                "absolute position encoding or --max_realtive_positions with"
+                " -1 for Rotary, or > 0 for Relative Position Representations"
+                "as in https://arxiv.org/pdf/1803.02155.pdf")
+
     @classmethod
     def ckpt_model_opts(cls, ckpt_opt):
         # Load default opt values, then overwrite with the opts in
         # the checkpoint. That way, if there are new options added,
         # the defaults are used.
         opt = cls.defaults(opts.model_opts)
         opt.__dict__.update(ckpt_opt.__dict__)
```

### Comparing `OpenNMT-py-3.1.1/onmt/utils/report_manager.py` & `OpenNMT-py-3.1.2/onmt/utils/report_manager.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/utils/scoring_utils.py` & `OpenNMT-py-3.1.2/onmt/utils/scoring_utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/onmt/utils/statistics.py` & `OpenNMT-py-3.1.2/onmt/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.1/setup.py` & `OpenNMT-py-3.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 setup(
     name='OpenNMT-py',
     description='A python implementation of OpenNMT',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='3.1.1',
+    version='3.1.2',
     packages=find_packages(),
     project_urls={
         "Documentation": "http://opennmt.net/OpenNMT-py/",
         "Forum": "http://forum.opennmt.net/",
         "Gitter": "https://gitter.im/OpenNMT/OpenNMT-py",
         "Source": "https://github.com/OpenNMT/OpenNMT-py/"
     },
@@ -27,15 +27,16 @@
         "tensorboard>=2.3",
         "flask",
         "waitress",
         "pyonmttok>=1.35,<2",
         "pyyaml",
         "sacrebleu",
         "rapidfuzz",
-        "pyahocorasick"
+        "pyahocorasick",
+        "gcld3"
     ],
     entry_points={
         "console_scripts": [
             "onmt_server=onmt.bin.server:main",
             "onmt_train=onmt.bin.train:main",
             "onmt_translate=onmt.bin.translate:main",
             "onmt_translate_dynamic=onmt.bin.translate_dynamic:main",
```

