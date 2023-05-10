# Comparing `tmp/treform-1.1.8.tar.gz` & `tmp/treform-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\treform-1.1.8.tar", last modified: Sun Apr 25 12:48:28 2021, max compression
+gzip compressed data, was "dist\treform-1.1.9.tar", last modified: Tue May  4 02:49:43 2021, max compression
```

## Comparing `treform-1.1.8.tar` & `treform-1.1.9.tar`

### file list

```diff
@@ -1,147 +1,144 @@
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/
--rw-rw-rw-   0        0        0     1037 2021-04-25 12:48:28.000000 treform-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      506 2020-07-14 14:44:01.000000 treform-1.1.8/README.md
--rw-rw-rw-   0        0        0       42 2021-04-25 12:48:28.000000 treform-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1816 2021-04-25 12:48:14.000000 treform-1.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/spelling_training/
--rw-rw-rw-   0        0        0     4521 2021-03-14 04:56:09.000000 treform-1.1.8/spelling_training/config.py
--rw-rw-rw-   0        0        0    28880 2021-03-14 12:24:14.000000 treform-1.1.8/spelling_training/spelling_error_correction.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/
--rw-rw-rw-   0        0        0     9399 2021-04-18 06:32:34.000000 treform-1.1.8/treform/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/abbreviations/
--rw-rw-rw-   0        0        0    12836 2021-03-07 03:11:52.000000 treform-1.1.8/treform/abbreviations/__init__.py
--rw-rw-rw-   0        0        0      230 2021-03-07 02:34:08.000000 treform-1.1.8/treform/abbreviations/candidate.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/chunker/
--rw-rw-rw-   0        0        0      568 2021-03-01 04:35:22.000000 treform-1.1.8/treform/chunker/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/collector/
--rw-rw-rw-   0        0        0      307 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/__init__.py
--rw-rw-rw-   0        0        0     2076 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/colAmericanNewsContent.py
--rw-rw-rw-   0        0        0    10828 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/colAmericanNewsURL.py
--rw-rw-rw-   0        0        0     4052 2021-03-20 14:04:58.000000 treform-1.1.8/treform/collector/colBasic.py
--rw-rw-rw-   0        0        0     2217 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/colBigkinds.py
--rw-rw-rw-   0        0        0     1408 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/colChosun.py
--rw-rw-rw-   0        0        0     1453 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/colDonga.py
--rw-rw-rw-   0        0        0     1543 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/colJoongang.py
--rw-rw-rw-   0        0        0     5516 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/colNaverBlog.py
--rw-rw-rw-   0        0        0     1365 2021-03-01 04:35:22.000000 treform-1.1.8/treform/collector/colNaverNews.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/cooccurrence/
--rw-rw-rw-   0        0        0     5670 2021-04-14 02:14:17.000000 treform-1.1.8/treform/cooccurrence/__init__.py
--rw-rw-rw-   0        0        0     2743 2021-03-01 04:35:22.000000 treform-1.1.8/treform/cooccurrence/cooccurrence.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/counter/
--rw-rw-rw-   0        0        0      217 2021-03-01 04:35:22.000000 treform-1.1.8/treform/counter/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/document_classification/
--rw-rw-rw-   0        0        0       45 2021-03-01 04:35:22.000000 treform-1.1.8/treform/document_classification/__init__.py
--rw-rw-rw-   0        0        0     6610 2021-03-01 04:35:22.000000 treform-1.1.8/treform/document_classification/lasso_term_extraction.py
--rw-rw-rw-   0        0        0    10994 2021-03-01 04:35:22.000000 treform-1.1.8/treform/document_classification/ml_textclassification.py
--rw-rw-rw-   0        0        0     3216 2021-03-01 04:35:22.000000 treform-1.1.8/treform/document_classification/test_ml_text_classfier.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/document_clustering/
--rw-rw-rw-   0        0        0       41 2021-03-01 04:35:22.000000 treform-1.1.8/treform/document_clustering/__init__.py
--rw-rw-rw-   0        0        0    10982 2021-03-01 04:35:22.000000 treform-1.1.8/treform/document_clustering/documentclustering.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/graphml/
--rw-rw-rw-   0        0        0    12588 2021-04-09 05:14:18.000000 treform-1.1.8/treform/graphml/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/helper/
--rw-rw-rw-   0        0        0     1463 2021-03-01 04:35:22.000000 treform-1.1.8/treform/helper/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/keyword/
--rw-rw-rw-   0        0        0     3339 2021-04-04 03:25:14.000000 treform-1.1.8/treform/keyword/__init__.py
--rw-rw-rw-   0        0        0     9543 2021-04-03 23:37:35.000000 treform-1.1.8/treform/keyword/ml_keyword_builder.py
--rw-rw-rw-   0        0        0     2134 2021-04-04 00:34:28.000000 treform-1.1.8/treform/keyword/ml_keyword_extractor.py
--rw-rw-rw-   0        0        0     9489 2021-03-01 04:35:22.000000 treform-1.1.8/treform/keyword/textrank.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/lemmatizer/
--rw-rw-rw-   0        0        0    10029 2021-03-01 04:35:22.000000 treform-1.1.8/treform/lemmatizer/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/ngram/
--rw-rw-rw-   0        0        0      758 2021-03-01 04:35:22.000000 treform-1.1.8/treform/ngram/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/noun_extractor/
--rw-rw-rw-   0        0        0      430 2021-03-01 04:35:22.000000 treform-1.1.8/treform/noun_extractor/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/pmi/
--rw-rw-rw-   0        0        0     1658 2021-03-01 04:35:22.000000 treform-1.1.8/treform/pmi/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/segmentation/
--rw-rw-rw-   0        0        0      905 2021-03-01 04:35:22.000000 treform-1.1.8/treform/segmentation/WordSemgmentationModelBuilder.py
--rw-rw-rw-   0        0        0     9135 2021-04-15 13:50:09.000000 treform-1.1.8/treform/segmentation/__init__.py
--rw-rw-rw-   0        0        0     9676 2021-04-25 12:21:10.000000 treform-1.1.8/treform/segmentation/cnnWordSegmentationModel.py
--rw-rw-rw-   0        0        0     9032 2021-04-15 13:51:55.000000 treform-1.1.8/treform/segmentation/cnnWordSegmentationModelBuilder.py
--rw-rw-rw-   0        0        0     1916 2021-03-01 04:35:22.000000 treform-1.1.8/treform/segmentation/lstmWordSegmentationModel.py
--rw-rw-rw-   0        0        0     5140 2021-03-13 10:04:52.000000 treform-1.1.8/treform/segmentation/lstmWordSegmentationModelBuilder.py
--rw-rw-rw-   0        0        0     8176 2021-03-13 10:03:01.000000 treform-1.1.8/treform/segmentation/wordSegmentationModelUtil.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/sentiment/
--rw-rw-rw-   0        0        0     3865 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/DLSentimentModel.py
--rw-rw-rw-   0        0        0     2812 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/DLSentimentPredictor.py
--rw-rw-rw-   0        0        0     5256 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/LSTMSentimentManager.py
--rw-rw-rw-   0        0        0    16828 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/MLSentimentManager.py
--rw-rw-rw-   0        0        0       31 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/__init__.py
--rw-rw-rw-   0        0        0     2260 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/englishDictionarySentimentAnalyzer.py
--rw-rw-rw-   0        0        0     8524 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/koreanDictionarySentimentAnalyzer.py
--rw-rw-rw-   0        0        0     3705 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/sentimentDataManager.py
--rw-rw-rw-   0        0        0     8069 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/test_MLSentimentManager.py
--rw-rw-rw-   0        0        0      639 2021-03-01 04:35:22.000000 treform-1.1.8/treform/sentiment/test_MLSentimentPrediction.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/spelling/
--rw-rw-rw-   0        0        0     5914 2021-04-25 09:37:56.000000 treform-1.1.8/treform/spelling/__init__.py
--rw-rw-rw-   0        0        0     5726 2021-04-25 02:40:17.000000 treform-1.1.8/treform/spelling/config.py
--rw-rw-rw-   0        0        0    28712 2021-04-24 14:32:06.000000 treform-1.1.8/treform/spelling/spelling_error_correction.py
--rw-rw-rw-   0        0        0    27489 2021-04-25 02:24:34.000000 treform-1.1.8/treform/spelling/spelling_error_correction_upgraded.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/splitter/
--rw-rw-rw-   0        0        0      795 2021-03-01 04:35:22.000000 treform-1.1.8/treform/splitter/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/stemmer/
--rw-rw-rw-   0        0        0      503 2021-03-01 04:35:22.000000 treform-1.1.8/treform/stemmer/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/synonym/
--rw-rw-rw-   0        0        0      640 2021-03-07 04:37:11.000000 treform-1.1.8/treform/synonym/__init__.py
--rw-rw-rw-   0        0        0     5325 2021-03-08 04:15:32.000000 treform-1.1.8/treform/synonym/generate_data.py
--rw-rw-rw-   0        0        0      953 2021-03-07 15:07:59.000000 treform-1.1.8/treform/synonym/train.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/syntactic_parser/
--rw-rw-rw-   0        0        0     1413 2021-03-31 03:12:15.000000 treform-1.1.8/treform/syntactic_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/tagger/
--rw-rw-rw-   0        0        0      421 2021-03-01 04:35:22.000000 treform-1.1.8/treform/tagger/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/tokenizer/
--rw-rw-rw-   0        0        0     3529 2021-03-17 02:00:04.000000 treform-1.1.8/treform/tokenizer/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/topic_model/
--rw-rw-rw-   0        0        0     9535 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/MalletWrapper.py
--rw-rw-rw-   0        0        0       33 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/__init__.py
--rw-rw-rw-   0        0        0     3071 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/gdmr_plot.py
--rw-rw-rw-   0        0        0     4807 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/lda.py
--rw-rw-rw-   0        0        0      771 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/ldaInference.py
--rw-rw-rw-   0        0        0     3024 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/ldaSeqModel.py
--rw-rw-rw-   0        0        0      469 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/ldaVisualizer.py
--rw-rw-rw-   0        0        0    32102 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/pyTextMinerTopicModel.py
--rw-rw-rw-   0        0        0     2046 2021-03-01 04:35:22.000000 treform-1.1.8/treform/topic_model/tfidf.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/utility/
--rw-rw-rw-   0        0        0     3525 2021-03-14 05:28:53.000000 treform-1.1.8/treform/utility/__init__.py
--rw-rw-rw-   0        0        0     2972 2021-03-14 02:47:53.000000 treform-1.1.8/treform/utility/base_util.py
--rw-rw-rw-   0        0        0     3798 2021-03-14 03:03:11.000000 treform-1.1.8/treform/utility/char_one_hot_vector.py
--rw-rw-rw-   0        0        0      741 2021-03-14 02:48:47.000000 treform-1.1.8/treform/utility/datafile_util.py
--rw-rw-rw-   0        0        0     7510 2021-03-14 04:51:05.000000 treform-1.1.8/treform/utility/dataset.py
--rw-rw-rw-   0        0        0    12112 2021-03-14 03:34:43.000000 treform-1.1.8/treform/utility/date_util.py
--rw-rw-rw-   0        0        0     4824 2021-03-14 04:35:16.000000 treform-1.1.8/treform/utility/file_util.py
--rw-rw-rw-   0        0        0    24805 2021-03-14 04:35:25.000000 treform-1.1.8/treform/utility/hangul_util.py
--rw-rw-rw-   0        0        0     8230 2021-03-14 04:35:47.000000 treform-1.1.8/treform/utility/log_util.py
--rw-rw-rw-   0        0        0    12349 2021-03-14 02:57:22.000000 treform-1.1.8/treform/utility/mult_proc_timed_rotating_file_handler.py
--rw-rw-rw-   0        0        0     5108 2021-03-14 02:55:26.000000 treform-1.1.8/treform/utility/num_util.py
--rw-rw-rw-   0        0        0     6205 2021-03-14 03:18:35.000000 treform-1.1.8/treform/utility/string_util.py
--rw-rw-rw-   0        0        0     4160 2021-03-14 04:36:27.000000 treform-1.1.8/treform/utility/watch_util.py
--rw-rw-rw-   0        0        0      215 2021-04-25 12:47:43.000000 treform-1.1.8/treform/version.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/weighting/
--rw-rw-rw-   0        0        0     4676 2021-04-18 09:04:53.000000 treform-1.1.8/treform/weighting/__init__.py
--rw-rw-rw-   0        0        0     1492 2021-04-18 07:41:42.000000 treform-1.1.8/treform/weighting/iqf_qf_icf.py
--rw-rw-rw-   0        0        0      489 2021-04-18 07:23:43.000000 treform-1.1.8/treform/weighting/one_hot.py
--rw-rw-rw-   0        0        0    30683 2021-04-20 12:44:46.000000 treform-1.1.8/treform/weighting/term_burstiness.py
--rw-rw-rw-   0        0        0     1379 2021-04-18 07:22:59.000000 treform-1.1.8/treform/weighting/tf_bdc.py
--rw-rw-rw-   0        0        0     1881 2021-04-18 07:46:28.000000 treform-1.1.8/treform/weighting/tf_chi.py
--rw-rw-rw-   0        0        0     1364 2021-04-18 07:48:40.000000 treform-1.1.8/treform/weighting/tf_dc.py
--rw-rw-rw-   0        0        0     2109 2021-04-18 07:54:39.000000 treform-1.1.8/treform/weighting/tf_eccd.py
--rw-rw-rw-   0        0        0     1001 2021-04-18 07:07:08.000000 treform-1.1.8/treform/weighting/tf_idf.py
--rw-rw-rw-   0        0        0     1816 2021-04-18 09:11:08.000000 treform-1.1.8/treform/weighting/tf_ig.py
--rw-rw-rw-   0        0        0     1837 2021-04-18 08:00:10.000000 treform-1.1.8/treform/weighting/tf_rf.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform/word2vec/
--rw-rw-rw-   0        0        0       32 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/__init__.py
--rw-rw-rw-   0        0        0     3440 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/avgDocumentByW2V.py
--rw-rw-rw-   0        0        0      264 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/gloveWikiKoreanTrainer.py
--rw-rw-rw-   0        0        0     2152 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/utils.py
--rw-rw-rw-   0        0        0     8359 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/visualizeW2V.py
--rw-rw-rw-   0        0        0     2779 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/visualizeW2VPlot.py
--rw-rw-rw-   0        0        0     8045 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/word2vecFilteringFunction.py
--rw-rw-rw-   0        0        0     5460 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/word2veclite.py
--rw-rw-rw-   0        0        0    17905 2021-03-01 04:35:22.000000 treform-1.1.8/treform/word2vec/word_embeddings.py
-drwxrwxrwx   0        0        0        0 2021-04-25 12:48:28.000000 treform-1.1.8/treform.egg-info/
--rw-rw-rw-   0        0        0     1037 2021-04-25 12:48:28.000000 treform-1.1.8/treform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3984 2021-04-25 12:48:28.000000 treform-1.1.8/treform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-25 12:48:28.000000 treform-1.1.8/treform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      421 2021-04-25 12:48:28.000000 treform-1.1.8/treform.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-04-25 12:48:28.000000 treform-1.1.8/treform.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/
+-rw-rw-rw-   0        0        0     1037 2021-05-04 02:49:43.000000 treform-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2020-07-14 14:44:01.000000 treform-1.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-05-04 02:49:43.000000 treform-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1816 2021-04-25 12:48:14.000000 treform-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/spelling_training/
+-rw-rw-rw-   0        0        0     4521 2021-03-14 04:56:09.000000 treform-1.1.9/spelling_training/config.py
+-rw-rw-rw-   0        0        0    28880 2021-03-14 12:24:14.000000 treform-1.1.9/spelling_training/spelling_error_correction.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/
+-rw-rw-rw-   0        0        0     9399 2021-04-18 06:32:34.000000 treform-1.1.9/treform/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/abbreviations/
+-rw-rw-rw-   0        0        0    12836 2021-03-07 03:11:52.000000 treform-1.1.9/treform/abbreviations/__init__.py
+-rw-rw-rw-   0        0        0      230 2021-03-07 02:34:08.000000 treform-1.1.9/treform/abbreviations/candidate.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/chunker/
+-rw-rw-rw-   0        0        0      568 2021-03-01 04:35:22.000000 treform-1.1.9/treform/chunker/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/collector/
+-rw-rw-rw-   0        0        0      307 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/__init__.py
+-rw-rw-rw-   0        0        0     2076 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/colAmericanNewsContent.py
+-rw-rw-rw-   0        0        0    10828 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/colAmericanNewsURL.py
+-rw-rw-rw-   0        0        0     4052 2021-03-20 14:04:58.000000 treform-1.1.9/treform/collector/colBasic.py
+-rw-rw-rw-   0        0        0     2217 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/colBigkinds.py
+-rw-rw-rw-   0        0        0     1408 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/colChosun.py
+-rw-rw-rw-   0        0        0     1453 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/colDonga.py
+-rw-rw-rw-   0        0        0     1543 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/colJoongang.py
+-rw-rw-rw-   0        0        0     5516 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/colNaverBlog.py
+-rw-rw-rw-   0        0        0     1365 2021-03-01 04:35:22.000000 treform-1.1.9/treform/collector/colNaverNews.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/cooccurrence/
+-rw-rw-rw-   0        0        0     5670 2021-04-14 02:14:17.000000 treform-1.1.9/treform/cooccurrence/__init__.py
+-rw-rw-rw-   0        0        0     2743 2021-03-01 04:35:22.000000 treform-1.1.9/treform/cooccurrence/cooccurrence.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/counter/
+-rw-rw-rw-   0        0        0      217 2021-03-01 04:35:22.000000 treform-1.1.9/treform/counter/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/document_classification/
+-rw-rw-rw-   0        0        0       45 2021-03-01 04:35:22.000000 treform-1.1.9/treform/document_classification/__init__.py
+-rw-rw-rw-   0        0        0     6610 2021-03-01 04:35:22.000000 treform-1.1.9/treform/document_classification/lasso_term_extraction.py
+-rw-rw-rw-   0        0        0    11455 2021-04-30 03:05:16.000000 treform-1.1.9/treform/document_classification/ml_textclassification.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/document_clustering/
+-rw-rw-rw-   0        0        0       41 2021-03-01 04:35:22.000000 treform-1.1.9/treform/document_clustering/__init__.py
+-rw-rw-rw-   0        0        0    11123 2021-04-28 09:28:14.000000 treform-1.1.9/treform/document_clustering/documentclustering.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/graphml/
+-rw-rw-rw-   0        0        0    12588 2021-04-09 05:14:18.000000 treform-1.1.9/treform/graphml/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/helper/
+-rw-rw-rw-   0        0        0     1463 2021-03-01 04:35:22.000000 treform-1.1.9/treform/helper/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/keyword/
+-rw-rw-rw-   0        0        0     3339 2021-04-04 03:25:14.000000 treform-1.1.9/treform/keyword/__init__.py
+-rw-rw-rw-   0        0        0     9543 2021-04-03 23:37:35.000000 treform-1.1.9/treform/keyword/ml_keyword_builder.py
+-rw-rw-rw-   0        0        0     2134 2021-04-04 00:34:28.000000 treform-1.1.9/treform/keyword/ml_keyword_extractor.py
+-rw-rw-rw-   0        0        0     9489 2021-03-01 04:35:22.000000 treform-1.1.9/treform/keyword/textrank.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/lemmatizer/
+-rw-rw-rw-   0        0        0    10029 2021-03-01 04:35:22.000000 treform-1.1.9/treform/lemmatizer/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/ngram/
+-rw-rw-rw-   0        0        0      758 2021-03-01 04:35:22.000000 treform-1.1.9/treform/ngram/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/noun_extractor/
+-rw-rw-rw-   0        0        0      430 2021-03-01 04:35:22.000000 treform-1.1.9/treform/noun_extractor/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/pmi/
+-rw-rw-rw-   0        0        0     1658 2021-03-01 04:35:22.000000 treform-1.1.9/treform/pmi/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/segmentation/
+-rw-rw-rw-   0        0        0      905 2021-03-01 04:35:22.000000 treform-1.1.9/treform/segmentation/WordSemgmentationModelBuilder.py
+-rw-rw-rw-   0        0        0     9058 2021-04-29 11:37:12.000000 treform-1.1.9/treform/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     9263 2021-04-29 12:43:56.000000 treform-1.1.9/treform/segmentation/cnnWordSegmentationModel.py
+-rw-rw-rw-   0        0        0     9032 2021-04-15 13:51:55.000000 treform-1.1.9/treform/segmentation/cnnWordSegmentationModelBuilder.py
+-rw-rw-rw-   0        0        0     1916 2021-03-01 04:35:22.000000 treform-1.1.9/treform/segmentation/lstmWordSegmentationModel.py
+-rw-rw-rw-   0        0        0     5140 2021-03-13 10:04:52.000000 treform-1.1.9/treform/segmentation/lstmWordSegmentationModelBuilder.py
+-rw-rw-rw-   0        0        0     8176 2021-03-13 10:03:01.000000 treform-1.1.9/treform/segmentation/wordSegmentationModelUtil.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/sentiment/
+-rw-rw-rw-   0        0        0     3865 2021-03-01 04:35:22.000000 treform-1.1.9/treform/sentiment/DLSentimentModel.py
+-rw-rw-rw-   0        0        0     2812 2021-03-01 04:35:22.000000 treform-1.1.9/treform/sentiment/DLSentimentPredictor.py
+-rw-rw-rw-   0        0        0     5256 2021-03-01 04:35:22.000000 treform-1.1.9/treform/sentiment/LSTMSentimentManager.py
+-rw-rw-rw-   0        0        0    16828 2021-03-01 04:35:22.000000 treform-1.1.9/treform/sentiment/MLSentimentManager.py
+-rw-rw-rw-   0        0        0       31 2021-03-01 04:35:22.000000 treform-1.1.9/treform/sentiment/__init__.py
+-rw-rw-rw-   0        0        0     2260 2021-03-01 04:35:22.000000 treform-1.1.9/treform/sentiment/englishDictionarySentimentAnalyzer.py
+-rw-rw-rw-   0        0        0     8524 2021-03-01 04:35:22.000000 treform-1.1.9/treform/sentiment/koreanDictionarySentimentAnalyzer.py
+-rw-rw-rw-   0        0        0     3705 2021-03-01 04:35:22.000000 treform-1.1.9/treform/sentiment/sentimentDataManager.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/spelling/
+-rw-rw-rw-   0        0        0     5914 2021-04-25 09:37:56.000000 treform-1.1.9/treform/spelling/__init__.py
+-rw-rw-rw-   0        0        0     5726 2021-04-25 02:40:17.000000 treform-1.1.9/treform/spelling/config.py
+-rw-rw-rw-   0        0        0    28712 2021-04-24 14:32:06.000000 treform-1.1.9/treform/spelling/spelling_error_correction.py
+-rw-rw-rw-   0        0        0    27489 2021-04-25 02:24:34.000000 treform-1.1.9/treform/spelling/spelling_error_correction_upgraded.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/splitter/
+-rw-rw-rw-   0        0        0      795 2021-03-01 04:35:22.000000 treform-1.1.9/treform/splitter/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/stemmer/
+-rw-rw-rw-   0        0        0      503 2021-03-01 04:35:22.000000 treform-1.1.9/treform/stemmer/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/synonym/
+-rw-rw-rw-   0        0        0      640 2021-03-07 04:37:11.000000 treform-1.1.9/treform/synonym/__init__.py
+-rw-rw-rw-   0        0        0     5325 2021-03-08 04:15:32.000000 treform-1.1.9/treform/synonym/generate_data.py
+-rw-rw-rw-   0        0        0      953 2021-03-07 15:07:59.000000 treform-1.1.9/treform/synonym/train.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/syntactic_parser/
+-rw-rw-rw-   0        0        0     1413 2021-03-31 03:12:15.000000 treform-1.1.9/treform/syntactic_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/tagger/
+-rw-rw-rw-   0        0        0      421 2021-03-01 04:35:22.000000 treform-1.1.9/treform/tagger/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/tokenizer/
+-rw-rw-rw-   0        0        0     3529 2021-03-17 02:00:04.000000 treform-1.1.9/treform/tokenizer/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/topic_model/
+-rw-rw-rw-   0        0        0     9535 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/MalletWrapper.py
+-rw-rw-rw-   0        0        0       33 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/__init__.py
+-rw-rw-rw-   0        0        0     3071 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/gdmr_plot.py
+-rw-rw-rw-   0        0        0     4807 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/lda.py
+-rw-rw-rw-   0        0        0      771 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/ldaInference.py
+-rw-rw-rw-   0        0        0     3024 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/ldaSeqModel.py
+-rw-rw-rw-   0        0        0      469 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/ldaVisualizer.py
+-rw-rw-rw-   0        0        0    32102 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/pyTextMinerTopicModel.py
+-rw-rw-rw-   0        0        0     2046 2021-03-01 04:35:22.000000 treform-1.1.9/treform/topic_model/tfidf.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/utility/
+-rw-rw-rw-   0        0        0     3525 2021-03-14 05:28:53.000000 treform-1.1.9/treform/utility/__init__.py
+-rw-rw-rw-   0        0        0     2972 2021-03-14 02:47:53.000000 treform-1.1.9/treform/utility/base_util.py
+-rw-rw-rw-   0        0        0     3798 2021-03-14 03:03:11.000000 treform-1.1.9/treform/utility/char_one_hot_vector.py
+-rw-rw-rw-   0        0        0      741 2021-03-14 02:48:47.000000 treform-1.1.9/treform/utility/datafile_util.py
+-rw-rw-rw-   0        0        0     7510 2021-03-14 04:51:05.000000 treform-1.1.9/treform/utility/dataset.py
+-rw-rw-rw-   0        0        0    12112 2021-03-14 03:34:43.000000 treform-1.1.9/treform/utility/date_util.py
+-rw-rw-rw-   0        0        0     4824 2021-03-14 04:35:16.000000 treform-1.1.9/treform/utility/file_util.py
+-rw-rw-rw-   0        0        0    24805 2021-03-14 04:35:25.000000 treform-1.1.9/treform/utility/hangul_util.py
+-rw-rw-rw-   0        0        0     8230 2021-03-14 04:35:47.000000 treform-1.1.9/treform/utility/log_util.py
+-rw-rw-rw-   0        0        0    12349 2021-03-14 02:57:22.000000 treform-1.1.9/treform/utility/mult_proc_timed_rotating_file_handler.py
+-rw-rw-rw-   0        0        0     5108 2021-03-14 02:55:26.000000 treform-1.1.9/treform/utility/num_util.py
+-rw-rw-rw-   0        0        0     6205 2021-03-14 03:18:35.000000 treform-1.1.9/treform/utility/string_util.py
+-rw-rw-rw-   0        0        0     4160 2021-03-14 04:36:27.000000 treform-1.1.9/treform/utility/watch_util.py
+-rw-rw-rw-   0        0        0      215 2021-05-04 02:46:44.000000 treform-1.1.9/treform/version.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/weighting/
+-rw-rw-rw-   0        0        0     4812 2021-04-28 09:23:12.000000 treform-1.1.9/treform/weighting/__init__.py
+-rw-rw-rw-   0        0        0     1492 2021-04-18 07:41:42.000000 treform-1.1.9/treform/weighting/iqf_qf_icf.py
+-rw-rw-rw-   0        0        0      489 2021-04-18 07:23:43.000000 treform-1.1.9/treform/weighting/one_hot.py
+-rw-rw-rw-   0        0        0    30683 2021-04-20 12:44:46.000000 treform-1.1.9/treform/weighting/term_burstiness.py
+-rw-rw-rw-   0        0        0     1379 2021-04-18 07:22:59.000000 treform-1.1.9/treform/weighting/tf_bdc.py
+-rw-rw-rw-   0        0        0     1881 2021-04-18 07:46:28.000000 treform-1.1.9/treform/weighting/tf_chi.py
+-rw-rw-rw-   0        0        0     1364 2021-04-18 07:48:40.000000 treform-1.1.9/treform/weighting/tf_dc.py
+-rw-rw-rw-   0        0        0     2109 2021-04-18 07:54:39.000000 treform-1.1.9/treform/weighting/tf_eccd.py
+-rw-rw-rw-   0        0        0     1001 2021-04-18 07:07:08.000000 treform-1.1.9/treform/weighting/tf_idf.py
+-rw-rw-rw-   0        0        0     1816 2021-04-18 09:11:08.000000 treform-1.1.9/treform/weighting/tf_ig.py
+-rw-rw-rw-   0        0        0     1837 2021-04-18 08:00:10.000000 treform-1.1.9/treform/weighting/tf_rf.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform/word2vec/
+-rw-rw-rw-   0        0        0       32 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/__init__.py
+-rw-rw-rw-   0        0        0     3440 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/avgDocumentByW2V.py
+-rw-rw-rw-   0        0        0      264 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/gloveWikiKoreanTrainer.py
+-rw-rw-rw-   0        0        0     2152 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/utils.py
+-rw-rw-rw-   0        0        0     8359 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/visualizeW2V.py
+-rw-rw-rw-   0        0        0     2779 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/visualizeW2VPlot.py
+-rw-rw-rw-   0        0        0     8045 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/word2vecFilteringFunction.py
+-rw-rw-rw-   0        0        0     5460 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/word2veclite.py
+-rw-rw-rw-   0        0        0    17905 2021-03-01 04:35:22.000000 treform-1.1.9/treform/word2vec/word_embeddings.py
+drwxrwxrwx   0        0        0        0 2021-05-04 02:49:43.000000 treform-1.1.9/treform.egg-info/
+-rw-rw-rw-   0        0        0     1037 2021-05-04 02:49:43.000000 treform-1.1.9/treform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3833 2021-05-04 02:49:43.000000 treform-1.1.9/treform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-04 02:49:43.000000 treform-1.1.9/treform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      421 2021-05-04 02:49:43.000000 treform-1.1.9/treform.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-05-04 02:49:43.000000 treform-1.1.9/treform.egg-info/top_level.txt
```

### Comparing `treform-1.1.8/PKG-INFO` & `treform-1.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treform
-Version: 1.1.8
+Version: 1.1.9
 Summary: A text mining tool for Korean and English
 Home-page: https://github.com/MinSong2/treform
 Author: Min Song
 Author-email: min.song@yonsei.ac.kr
 License: UNKNOWN
 Description: Welcome to the package of pyTextMiner. The current version of pyTextMiner is 1.1.116.
         For those who are interested in contributing to the development of pyTextMiner, please contact at min.song.njit@gmail.com.
```

### Comparing `treform-1.1.8/setup.py` & `treform-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/spelling_training/config.py` & `treform-1.1.9/spelling_training/config.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/spelling_training/spelling_error_correction.py` & `treform-1.1.9/spelling_training/spelling_error_correction.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/__init__.py` & `treform-1.1.9/treform/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/abbreviations/__init__.py` & `treform-1.1.9/treform/abbreviations/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/chunker/__init__.py` & `treform-1.1.9/treform/chunker/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colAmericanNewsContent.py` & `treform-1.1.9/treform/collector/colAmericanNewsContent.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colAmericanNewsURL.py` & `treform-1.1.9/treform/collector/colAmericanNewsURL.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colBasic.py` & `treform-1.1.9/treform/collector/colBasic.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colBigkinds.py` & `treform-1.1.9/treform/collector/colBigkinds.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colChosun.py` & `treform-1.1.9/treform/collector/colChosun.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colDonga.py` & `treform-1.1.9/treform/collector/colDonga.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colJoongang.py` & `treform-1.1.9/treform/collector/colJoongang.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colNaverBlog.py` & `treform-1.1.9/treform/collector/colNaverBlog.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/collector/colNaverNews.py` & `treform-1.1.9/treform/collector/colNaverNews.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/cooccurrence/__init__.py` & `treform-1.1.9/treform/cooccurrence/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/cooccurrence/cooccurrence.py` & `treform-1.1.9/treform/cooccurrence/cooccurrence.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/document_classification/lasso_term_extraction.py` & `treform-1.1.9/treform/document_classification/lasso_term_extraction.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/document_classification/ml_textclassification.py` & `treform-1.1.9/treform/document_classification/ml_textclassification.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.feature_selection import chi2
 from sklearn.model_selection import train_test_split
 from sklearn.feature_extraction.text import CountVectorizer
 from sklearn.feature_extraction.text import TfidfTransformer
 from sklearn.naive_bayes import MultinomialNB
 from sklearn.linear_model import LogisticRegression, SGDClassifier
-from sklearn.ensemble import RandomForestClassifier
+from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
 from sklearn.svm import LinearSVC
 from sklearn.model_selection import cross_val_score
 from sklearn.metrics import confusion_matrix
 import seaborn as sns
 from sklearn import metrics
 from joblib import dump, load
 from sklearn.neighbors import KNeighborsClassifier
 
 import sklearn
+from sklearn.tree import DecisionTreeClassifier
+
 
 class documentClassifier:
     def __init__(self):
         name='document_classifier'
         self.documents=[]
         self.features=None
         self.labels=None
@@ -33,15 +35,15 @@
         self.id_to_category=None
         self.category_to_id=None
 
         self.features=None
         self.labels=None
         self.class_number=0
 
-    def preprocess(self, documents, class_list):
+    def preprocess(self, documents, class_list, id_category_json=''):
 
         #1. we assume that pyTextMiner pre-processing module was applied to the list of documents
         print(str(len(documents)) + " : " + str(len(class_list)))
         #create a list of rows consisting of text and class label by DataFrame
         self.df = pd.DataFrame({'text': documents, 'label': class_list})
         self.df = sklearn.utils.shuffle(self.df, n_samples=500, random_state=100)
         self.df.reset_index(inplace=True, drop=True)
@@ -56,15 +58,15 @@
         self.df.columns = ['text', 'label']
         self.df['category_id'] = self.df['label'].factorize()[0]
         self.category_id_df = self.df[['label', 'category_id']].drop_duplicates().sort_values('category_id')
         self.category_to_id = dict(self.category_id_df.values)
         self.id_to_category = dict(self.category_id_df[['category_id', 'label']].values)
 
         # To save the dictionary into a file:
-        json.dump(self.id_to_category, open("./model/id_to_category.json", 'w'))
+        json.dump(self.id_to_category, open(id_category_json, 'w', encoding='utf-8'))
 
         print(self.df.head())
 
         #number of classes
         self.class_number=self.df.label.unique()
 
         #visualize the distribution of classes
@@ -97,21 +99,26 @@
         # We are now ready to experiment with different machine learning models,
         # evaluate their accuracy and find the source of any potential issues.
         # We will benchmark the following four models:
         # Logistic Regression
         # (Multinomial) Naive Bayes
         # Linear Support Vector Machine
         # Random Forest
+        # DecisionTree
+        # AdaBoostClassifier
+        # etc...
         models = [
             RandomForestClassifier(n_estimators=200, max_depth=3, random_state=0),
             LinearSVC(),
             MultinomialNB(),
             LogisticRegression(random_state=0),
             KNeighborsClassifier(n_neighbors=10, weights='uniform', algorithm='auto', leaf_size=30, p=2, metric='minkowski', metric_params=None, n_jobs=None),
-            SGDClassifier(loss='hinge', penalty='l2', alpha=0.0001)
+            SGDClassifier(loss='hinge', penalty='l2', alpha=0.0001),
+            DecisionTreeClassifier(),
+            AdaBoostClassifier(DecisionTreeClassifier(max_depth=1), algorithm="SAMME", n_estimators=200),
         ]
 
         CV = 5
         cv_df = pd.DataFrame(index=range(CV * len(models)))
         entries = []
         for model in models:
             model_name = model.__class__.__name__
@@ -162,15 +169,18 @@
                     print('')
 
         # As you can see, some of the misclassified complaints are complaints that touch on more than one subjects
         # (for example, complaints involving both credit card and credit report). This sort of errors will always happen.
         # Again, we use the chi-squared test to find the terms that are the most correlated with each of the categories:
         model.fit(self.features, self.labels)
         N = 2
-        if 'kneighbors' not in model.__class__.__name__.lower():
+
+        #print(model.__class__.__name__.lower())
+
+        if 'kneighbors' and 'decisiontreeclassifier' not in model.__class__.__name__.lower():
             for label, category_id in sorted(self.category_to_id.items()):
                 indices = np.argsort(model.coef_[category_id])
                 feature_names = np.array(self.tfidf.get_feature_names())[indices]
                 unigrams = [v for v in reversed(feature_names) if len(v.split(' ')) == 1][:N]
                 bigrams = [v for v in reversed(feature_names) if len(v.split(' ')) == 2][:N]
                 print("# '{}':".format(label))
                 print("  . Top unigrams:\n       . {}".format('\n       . '.join(unigrams)))
@@ -190,33 +200,33 @@
 
     def load(self, model_name):
         return load(model_name)
 
     def loadVectorizer(self, model_name='vectorizer.model'):
         return load(model_name)
 
-    def predict(self, model, vectorizer_model):
+    def predict(self, model, vectorizer_model, id_category_json=''):
         #7. prediction
         docs = ["한국 경제 글로벌 위기 수요 위축 시장 경제 붕귀 자동차 수출 빨간불 내수 촉진 증진 방향성 제고",
                 "밝기 5등급 정도 도심 밖 맨눈 충분히 관측 가능 새해 미국인 8월 행운 기대",
                 "최순실 민간인 국정농단 의혹 사건 진상규명 국정조사 특별위원회 1차 청문회 이재용 삼성전자 부회장 재벌 총수 9명 증인 출석"]
 
-        with open("./model/id_to_category.json") as handle:
+        with open(id_category_json, 'r', encoding='utf-8') as handle:
             id_to_category = json.loads(handle.read())
 
         text_features = vectorizer_model.transform(docs)
         predictions = model.predict(text_features)
         for text, predicted in zip(docs, predictions):
             print('"{}"'.format(text))
             print("  - Predicted as: '{}'".format(id_to_category[str(predicted)]))
             print("")
 
-    def predict_realtime(self, model, vectorizer_model, docs):
+    def predict_realtime(self, model, vectorizer_model, docs, id_category_json=''):
 
-        with open("./model/id_to_category.json") as handle:
+        with open(id_category_json, 'r', encoding='utf-8') as handle:
             id_to_category = json.loads(handle.read())
 
         text_features = vectorizer_model.transform(docs)
         predictions = model.predict(text_features)
         for text, predicted in zip(docs, predictions):
             print('"{}"'.format(text))
             print("  - Predicted as: '{}'".format(id_to_category[str(predicted)]))
```

### Comparing `treform-1.1.8/treform/document_clustering/documentclustering.py` & `treform-1.1.9/treform/document_clustering/documentclustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,18 @@
 
     def visualize(self):
         # The output is a one-dimensional array of N documents corresponding to the clusters
         # assigned to our N data points.
         if self.name == 'spectral_cocluster':
             pca_t = None
             if self.doc2vec_matrix == False:
-                pca_t = PCA().fit_transform(self.X.toarray())
+                if type(self.X) is np.ndarray:
+                    pca_t = PCA().fit_transform(self.X.tolist())
+                else:
+                    pca_t = PCA().fit_transform(self.X.toarray())
             else:
                 pca_t = PCA().fit_transform(self.X)
             #pca_t = PCA().fit_transform(self.X)
             # print(self.clustering.labels_)
             plt.scatter(pca_t[:, 0], pca_t[:, 1], c=self.clustering.row_labels_, cmap='rainbow')
             plt.show()
         elif self.name == 'agglo':
```

### Comparing `treform-1.1.8/treform/graphml/__init__.py` & `treform-1.1.9/treform/graphml/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/helper/__init__.py` & `treform-1.1.9/treform/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/keyword/__init__.py` & `treform-1.1.9/treform/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/keyword/ml_keyword_builder.py` & `treform-1.1.9/treform/keyword/ml_keyword_builder.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/keyword/ml_keyword_extractor.py` & `treform-1.1.9/treform/keyword/ml_keyword_extractor.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/keyword/textrank.py` & `treform-1.1.9/treform/keyword/textrank.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/lemmatizer/__init__.py` & `treform-1.1.9/treform/lemmatizer/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/ngram/__init__.py` & `treform-1.1.9/treform/ngram/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/pmi/__init__.py` & `treform-1.1.9/treform/pmi/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/segmentation/WordSemgmentationModelBuilder.py` & `treform-1.1.9/treform/segmentation/WordSemgmentationModelBuilder.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/segmentation/__init__.py` & `treform-1.1.9/treform/segmentation/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,100 +138,98 @@
 
 class CNNSegmentationKorean(BaseSegmentation):
     def __init__(self, model_file='./model', training_config='', char_file=''):
         self.model_file = model_file
         self.training_config = training_config
         self.char_file = char_file
 
-    def load(self, model_file='', training_config='', char_file=''):
-        tf.config.run_functions_eagerly(True)
+        #self.model, self.vocab_table = self.load(model_file=model_file, training_config=training_config, char_file=char_file)
 
-        print(tf.executing_eagerly())
 
-        with open(self.training_config, encoding='utf-8') as f:
+    def load(self, model_file='', training_config='', char_file=''):
+        with open(training_config, encoding='utf-8') as f:
             config = json.load(f)
 
-        with open(self.char_file, encoding='utf=8') as f:
+        with open(char_file, encoding='utf=8') as f:
             content = f.read()
             keys = ["<pad>", "<s>", "</s>", "<unk>"] + list(content)
             values = list(range(len(keys)))
 
-            vocab_initializer = tf.lookup.KeyValueTensorInitializer(keys, values, key_dtype=tf.string,
-                                                                    value_dtype=tf.int32)
+            vocab_initializer = tf.lookup.KeyValueTensorInitializer(keys, values, key_dtype=tf.string, value_dtype=tf.int32)
             vocab_table = tf.lookup.StaticHashTable(vocab_initializer, default_value=3)
 
         model = SpacingModel(
             config["vocab_size"],
             config["hidden_size"],
             conv_activation=config["conv_activation"],
             dense_activation=config["dense_activation"],
             conv_kernel_and_filter_sizes=config["conv_kernel_and_filter_sizes"],
             dropout_rate=config["dropout_rate"],
         )
 
-        model.load_weights(self.model_file)
+        model.load_weights(model_file)
         model(tf.keras.Input([None], dtype=tf.int32))
         model.summary()
 
         return model, vocab_table
 
     def predict(self, model, vocab_table, input_str):
         inference = self.get_inference_fn(model, vocab_table)
         input_str = tf.constant(input_str)
-        result1 = inference(input_str)
-        sess = tf.compat.v1.Session()
-        init = tf.compat.v1.global_variables_initializer()
-        sess.run(init)
-        sess.run(tf.compat.v1.tables_initializer())
-
-        result = sess.run(inference(input_str))
-        print(result)
-
-        print(b"".join(result).decode("utf8"))
+        result = inference(input_str).numpy()
+        #print(b"".join(result).decode("utf8"))
         return b"".join(result).decode("utf8")
 
     def get_inference_fn(self, model, vocab_table):
         @tf.function
         def inference(tensors):
             byte_array = tf.concat(
-                [["<s>"], tf.strings.unicode_split(tf.strings.regex_replace(tensors, " +", " "), "UTF-8"), ["</s>"]],
-                axis=0
+                [["<s>"], tf.strings.unicode_split(tf.strings.regex_replace(tensors, " +", " "), "UTF-8"), ["</s>"]], axis=0
             )
             strings = vocab_table.lookup(byte_array)[tf.newaxis, :]
 
             model_output = tf.argmax(model(strings), axis=-1)[0]
-            return self.convert_output_to_string(byte_array, model_output)
+            return convert_output_to_string(byte_array, model_output)
 
         return inference
 
-    def convert_output_to_string(self, byte_array, model_output):
-        sequence_length = tf.size(model_output)
-        while_condition = lambda i, *_: i < sequence_length
-
-        #@tf.function
-        def while_body(i, o):
-            a = tf.math.equal(model_output[i],2)
-            b = tf.math.equal(byte_array[i],' ')
-            c = tf.math.equal(model_output[i],1)
-
-            o = tf.cond(
-                tf.cast(c, tf.bool),
-                lambda: tf.concat([o, [byte_array[i], " "]], axis=0),
-                lambda: tf.cond(
-                    tf.cast(tf.logical_and(a, b),tf.bool),
-                    lambda: o,
-                    lambda: tf.concat([o, [byte_array[i]]], axis=0),
+
+    #def __call__(self, *args, **kwargs):
+    #    return self.predict(self.model, self.vocab_table, args[0])
+
+def convert_output_to_string(byte_array, model_output):
+    sequence_length = tf.size(model_output)
+    while_condition = lambda i, *_: i < sequence_length
+
+    def while_body(i, o):
+        o = tf.cond(
+            model_output[i] == 1,
+            lambda: tf.concat([o, [byte_array[i], " "]], axis=0),
+            lambda: tf.cond(
+                (model_output[i] == 2) and (byte_array[i] == " "),
+                lambda: o,
+                lambda: tf.concat([o, [byte_array[i]]], axis=0),
                 ),
             )
-            return i + 1, o
-
-        _, strings_result = tf.while_loop(
-            while_condition,
-            while_body,
-            (tf.constant(0), tf.constant([], dtype=tf.string)),
-            shape_invariants=(tf.TensorShape([]), tf.TensorShape([None])),
-        )
-        return strings_result
+        return i + 1, o
 
-    def __call__(self, *args, **kwargs):
-        model, vocab_table = self.load(self.model_file, self.training_config, self.char_file)
-        return self.predict(model, vocab_table, args[0])
+    _, strings_result = tf.while_loop(
+        while_condition,
+        while_body,
+        (tf.constant(0), tf.constant([], dtype=tf.string)),
+        shape_invariants=(tf.TensorShape([]), tf.TensorShape([None])),
+    )
+    return strings_result
+
+if __name__ == "__main__":
+    model_file = '../../models/checkpoint-12.ckpt'
+    training_config = '../../resources/config.json'
+    char_file = '../../resources/chars-4996'
+
+    spacing = CNNSegmentationKorean()
+
+    model, vocab_table = spacing.load(model_file=model_file, training_config=training_config, char_file=char_file)
+    input_str = '오늘은우울한날이야...ㅜㅜ'
+    result = spacing.predict(model, vocab_table, input_str)
+    result = result.replace('<s>','')
+    result = result.replace('</s>', '')
+    print(result)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `treform-1.1.8/treform/segmentation/cnnWordSegmentationModel.py` & `treform-1.1.9/treform/segmentation/cnnWordSegmentationModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from argparse import ArgumentParser
 from typing import List, Tuple
 
 import tensorflow as tf
 
-
 class SpacingModel(tf.keras.Model):
     def __init__(
             self,
             vocab_size: int,
             hidden_size: int,
             num_classes: int = 3,
             conv_activation: str = "relu",
@@ -54,15 +53,14 @@
             tf.concat([pool(conv(embeddings)) for conv, pool in zip(self.convs, self.pools)], axis=-1)
         )
         # projected: (Batch Size, Sequence Length, Hidden Size)
         projected = self.dropout2(self.output_dense1(features))
         # (Batch Size, Sequence Length, 2)
         return self.output_dense2(projected)
 
-
 def string_to_example(
         vocab_table: tf.lookup.StaticHashTable,
         encoding: str = "UTF-8",
         max_length: int = 256,
         delete_prob: float = 0.5,
         add_prob: float = 0.15,
 ):
@@ -71,34 +69,28 @@
         bytes_array = tf.strings.unicode_split(tf.strings.regex_replace(tensors, " +", " "), encoding)
         space_positions = bytes_array == " "
         sequence_length = tf.shape(space_positions)[0]
 
         while_condition = lambda i, *_: i < sequence_length
 
         def while_body(i, strings, labels):
-            # 다음 char가 space가 아니고, 문장 끝이 아닐 때 add_prob의 확률로 space 추가
-            # 이번 char가 space일 때
             is_next_char_space = tf.cond(i < sequence_length - 1, lambda: bytes_array[i + 1] == " ", lambda: False)
 
             state = tf.cond(
                 is_next_char_space,
                 lambda: tf.cond(tf.random.uniform([]) < delete_prob, lambda: 2, lambda: 0),
                 lambda: tf.cond(bytes_array[i] != " " and tf.random.uniform([]) < add_prob, lambda: 1, lambda: 0),
             )
-            # 0: 그대로 진행
-            # 1: 다음 인덱스에 space 추가
-            # 2: 다음 space 삭제
+
             strings = tf.cond(
                 state != 1,
                 lambda: tf.concat([strings, [bytes_array[i]]], axis=0),
                 lambda: tf.concat([strings, [bytes_array[i], " "]], axis=0),
             )
-            # label 0: 변화 x
-            # label 1: 다음 인덱스에 space 추가
-            # label 2: 현재 space 삭제
+
             labels = tf.cond(
                 state == 0,
                 lambda: tf.concat([labels, [0]], axis=0),
                 lambda: tf.cond(
                     state == 1,
                     lambda: tf.concat([labels, [0, 2]], axis=0),
                     lambda: tf.concat([labels, [1]], axis=0),
@@ -147,15 +139,14 @@
     positions = tf.where(y_true != ignore_id)
 
     y_true = tf.gather_nd(y_true, positions)
     y_pred = tf.gather_nd(y_pred, positions)
 
     return tf.keras.metrics.sparse_categorical_accuracy(y_true, y_pred)
 
-
 class SparseCategoricalCrossentropyWithIgnore(tf.python.keras.losses.LossFunctionWrapper):
     def __init__(
             self,
             from_logits=False,
             reduction=tf.keras.losses.Reduction.AUTO,
             ignore_id=-1,
             name="sparse_categorical_crossentropy_with_ignore",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `treform-1.1.8/treform/segmentation/cnnWordSegmentationModelBuilder.py` & `treform-1.1.9/treform/segmentation/cnnWordSegmentationModelBuilder.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/segmentation/lstmWordSegmentationModel.py` & `treform-1.1.9/treform/segmentation/lstmWordSegmentationModel.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/segmentation/lstmWordSegmentationModelBuilder.py` & `treform-1.1.9/treform/segmentation/lstmWordSegmentationModelBuilder.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/segmentation/wordSegmentationModelUtil.py` & `treform-1.1.9/treform/segmentation/wordSegmentationModelUtil.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/sentiment/DLSentimentModel.py` & `treform-1.1.9/treform/sentiment/DLSentimentModel.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/sentiment/DLSentimentPredictor.py` & `treform-1.1.9/treform/sentiment/DLSentimentPredictor.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/sentiment/LSTMSentimentManager.py` & `treform-1.1.9/treform/sentiment/LSTMSentimentManager.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/sentiment/MLSentimentManager.py` & `treform-1.1.9/treform/sentiment/MLSentimentManager.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/sentiment/englishDictionarySentimentAnalyzer.py` & `treform-1.1.9/treform/sentiment/englishDictionarySentimentAnalyzer.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/sentiment/koreanDictionarySentimentAnalyzer.py` & `treform-1.1.9/treform/sentiment/koreanDictionarySentimentAnalyzer.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/sentiment/sentimentDataManager.py` & `treform-1.1.9/treform/sentiment/sentimentDataManager.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/spelling/__init__.py` & `treform-1.1.9/treform/spelling/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/spelling/config.py` & `treform-1.1.9/treform/spelling/config.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/spelling/spelling_error_correction.py` & `treform-1.1.9/treform/spelling/spelling_error_correction.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/spelling/spelling_error_correction_upgraded.py` & `treform-1.1.9/treform/spelling/spelling_error_correction_upgraded.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/splitter/__init__.py` & `treform-1.1.9/treform/splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/synonym/__init__.py` & `treform-1.1.9/treform/synonym/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/synonym/generate_data.py` & `treform-1.1.9/treform/synonym/generate_data.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/synonym/train.py` & `treform-1.1.9/treform/synonym/train.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/syntactic_parser/__init__.py` & `treform-1.1.9/treform/syntactic_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/tokenizer/__init__.py` & `treform-1.1.9/treform/tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/topic_model/MalletWrapper.py` & `treform-1.1.9/treform/topic_model/MalletWrapper.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/topic_model/gdmr_plot.py` & `treform-1.1.9/treform/topic_model/gdmr_plot.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/topic_model/lda.py` & `treform-1.1.9/treform/topic_model/lda.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/topic_model/ldaInference.py` & `treform-1.1.9/treform/topic_model/ldaInference.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/topic_model/ldaSeqModel.py` & `treform-1.1.9/treform/topic_model/ldaSeqModel.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/topic_model/pyTextMinerTopicModel.py` & `treform-1.1.9/treform/topic_model/pyTextMinerTopicModel.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/topic_model/tfidf.py` & `treform-1.1.9/treform/topic_model/tfidf.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/__init__.py` & `treform-1.1.9/treform/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/base_util.py` & `treform-1.1.9/treform/utility/base_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/char_one_hot_vector.py` & `treform-1.1.9/treform/utility/char_one_hot_vector.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/datafile_util.py` & `treform-1.1.9/treform/utility/datafile_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/dataset.py` & `treform-1.1.9/treform/utility/dataset.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/date_util.py` & `treform-1.1.9/treform/utility/date_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/file_util.py` & `treform-1.1.9/treform/utility/file_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/hangul_util.py` & `treform-1.1.9/treform/utility/hangul_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/log_util.py` & `treform-1.1.9/treform/utility/log_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/mult_proc_timed_rotating_file_handler.py` & `treform-1.1.9/treform/utility/mult_proc_timed_rotating_file_handler.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/num_util.py` & `treform-1.1.9/treform/utility/num_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/string_util.py` & `treform-1.1.9/treform/utility/string_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/utility/watch_util.py` & `treform-1.1.9/treform/utility/watch_util.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/__init__.py` & `treform-1.1.9/treform/weighting/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,20 +31,22 @@
         doccount = {}
 
         label = 'UNI'
         for i, _doc in enumerate(input):
             document = {}
             if len(label_list) > 0:
                 document["label"] = label_list[i]
+                label = label_list[i]
             else:
                 document["label"] = label
             if label not in doccount:
                 doccount[label] = 0
             doccount[label] += 1
-            docname = label + str(doccount[label])
+            docname = document["label"] + str(doccount[label])  # label + str(doccount[label])
+            #docname = label + str(doccount[label])
             document["document"] = docname
 
             document["split_sentence"] = _doc
 
             if label not in labelset:
                 labelset.append(label)
```

### Comparing `treform-1.1.8/treform/weighting/iqf_qf_icf.py` & `treform-1.1.9/treform/weighting/iqf_qf_icf.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/term_burstiness.py` & `treform-1.1.9/treform/weighting/term_burstiness.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/tf_bdc.py` & `treform-1.1.9/treform/weighting/tf_bdc.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/tf_chi.py` & `treform-1.1.9/treform/weighting/tf_chi.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/tf_dc.py` & `treform-1.1.9/treform/weighting/tf_dc.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/tf_eccd.py` & `treform-1.1.9/treform/weighting/tf_eccd.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/tf_idf.py` & `treform-1.1.9/treform/weighting/tf_idf.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/tf_ig.py` & `treform-1.1.9/treform/weighting/tf_ig.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/weighting/tf_rf.py` & `treform-1.1.9/treform/weighting/tf_rf.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/word2vec/avgDocumentByW2V.py` & `treform-1.1.9/treform/word2vec/avgDocumentByW2V.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/word2vec/utils.py` & `treform-1.1.9/treform/word2vec/utils.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/word2vec/visualizeW2V.py` & `treform-1.1.9/treform/word2vec/visualizeW2V.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/word2vec/visualizeW2VPlot.py` & `treform-1.1.9/treform/word2vec/visualizeW2VPlot.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/word2vec/word2vecFilteringFunction.py` & `treform-1.1.9/treform/word2vec/word2vecFilteringFunction.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/word2vec/word2veclite.py` & `treform-1.1.9/treform/word2vec/word2veclite.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform/word2vec/word_embeddings.py` & `treform-1.1.9/treform/word2vec/word_embeddings.py`

 * *Files identical despite different names*

### Comparing `treform-1.1.8/treform.egg-info/PKG-INFO` & `treform-1.1.9/treform.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: treform
-Version: 1.1.8
+Version: 1.1.9
 Summary: A text mining tool for Korean and English
 Home-page: https://github.com/MinSong2/treform
 Author: Min Song
 Author-email: min.song@yonsei.ac.kr
 License: UNKNOWN
 Description: Welcome to the package of pyTextMiner. The current version of pyTextMiner is 1.1.116.
         For those who are interested in contributing to the development of pyTextMiner, please contact at min.song.njit@gmail.com.
```

### Comparing `treform-1.1.8/treform.egg-info/SOURCES.txt` & `treform-1.1.9/treform.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 treform/collector/colNaverNews.py
 treform/cooccurrence/__init__.py
 treform/cooccurrence/cooccurrence.py
 treform/counter/__init__.py
 treform/document_classification/__init__.py
 treform/document_classification/lasso_term_extraction.py
 treform/document_classification/ml_textclassification.py
-treform/document_classification/test_ml_text_classfier.py
 treform/document_clustering/__init__.py
 treform/document_clustering/documentclustering.py
 treform/graphml/__init__.py
 treform/helper/__init__.py
 treform/keyword/__init__.py
 treform/keyword/ml_keyword_builder.py
 treform/keyword/ml_keyword_extractor.py
@@ -52,16 +51,14 @@
 treform/sentiment/DLSentimentPredictor.py
 treform/sentiment/LSTMSentimentManager.py
 treform/sentiment/MLSentimentManager.py
 treform/sentiment/__init__.py
 treform/sentiment/englishDictionarySentimentAnalyzer.py
 treform/sentiment/koreanDictionarySentimentAnalyzer.py
 treform/sentiment/sentimentDataManager.py
-treform/sentiment/test_MLSentimentManager.py
-treform/sentiment/test_MLSentimentPrediction.py
 treform/spelling/__init__.py
 treform/spelling/config.py
 treform/spelling/spelling_error_correction.py
 treform/spelling/spelling_error_correction_upgraded.py
 treform/splitter/__init__.py
 treform/stemmer/__init__.py
 treform/synonym/__init__.py
```

