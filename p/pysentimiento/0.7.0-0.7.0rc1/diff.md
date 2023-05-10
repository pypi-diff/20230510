# Comparing `tmp/pysentimiento-0.7.0.tar.gz` & `tmp/pysentimiento-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysentimiento-0.7.0.tar", max compression
+gzip compressed data, was "pysentimiento-0.7.0rc1.tar", max compression
```

## Comparing `pysentimiento-0.7.0.tar` & `pysentimiento-0.7.0rc1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      338 2023-01-24 15:07:24.092098 pysentimiento-0.7.0/LICENSE.md
--rw-r--r--   0        0        0     6927 2023-05-10 12:06:24.571991 pysentimiento-0.7.0/README.md
--rw-r--r--   0        0        0     1025 2023-05-10 12:22:20.340027 pysentimiento-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       38 2023-03-30 11:51:24.383057 pysentimiento-0.7.0/pysentimiento/__init__.py
--rw-r--r--   0        0        0    20048 2023-04-19 19:02:33.630721 pysentimiento-0.7.0/pysentimiento/analyzer.py
--rw-r--r--   0        0        0       39 2023-01-24 15:07:24.172098 pysentimiento-0.7.0/pysentimiento/baselines/__init__.py
--rw-r--r--   0        0        0     4861 2023-01-24 15:07:24.172098 pysentimiento-0.7.0/pysentimiento/baselines/models.py
--rw-r--r--   0        0        0     5437 2023-01-31 20:16:06.893325 pysentimiento-0.7.0/pysentimiento/baselines/training.py
--rw-r--r--   0        0        0     1246 2023-01-24 15:07:24.172098 pysentimiento-0.7.0/pysentimiento/baselines/utils.py
--rw-r--r--   0        0        0      242 2023-02-24 14:38:20.566403 pysentimiento-0.7.0/pysentimiento/config.py
--rw-r--r--   0        0        0     3925 2023-03-03 13:56:08.310631 pysentimiento-0.7.0/pysentimiento/emotion.py
--rw-r--r--   0        0        0    11186 2023-02-27 12:26:28.317699 pysentimiento-0.7.0/pysentimiento/hate.py
--rw-r--r--   0        0        0     4330 2023-02-27 18:18:23.729976 pysentimiento-0.7.0/pysentimiento/irony.py
--rw-r--r--   0        0        0      119 2023-01-24 15:07:24.172098 pysentimiento-0.7.0/pysentimiento/lince/__init__.py
--rw-r--r--   0        0        0     7560 2023-02-24 14:38:20.566403 pysentimiento-0.7.0/pysentimiento/lince/ner.py
--rw-r--r--   0        0        0     3423 2023-02-24 14:38:20.570403 pysentimiento-0.7.0/pysentimiento/lince/pos.py
--rw-r--r--   0        0        0     1471 2023-02-24 14:38:20.570403 pysentimiento-0.7.0/pysentimiento/lince/sentiment.py
--rw-r--r--   0        0        0     1576 2023-01-24 15:07:24.172098 pysentimiento-0.7.0/pysentimiento/metrics.py
--rw-r--r--   0        0        0     6447 2023-03-29 23:37:11.649543 pysentimiento-0.7.0/pysentimiento/preprocessing.py
--rw-r--r--   0        0        0     2320 2023-02-24 14:38:20.570403 pysentimiento-0.7.0/pysentimiento/semeval.py
--rw-r--r--   0        0        0     2940 2023-02-27 11:52:33.917672 pysentimiento-0.7.0/pysentimiento/sentiment.py
--rw-r--r--   0        0        0      818 2023-02-24 14:39:51.342404 pysentimiento-0.7.0/pysentimiento/sentiment_pt.py
--rw-r--r--   0        0        0      825 2023-02-24 14:39:51.342404 pysentimiento-0.7.0/pysentimiento/sentipolc.py
--rw-r--r--   0        0        0     5356 2023-04-05 22:21:10.038814 pysentimiento-0.7.0/pysentimiento/targeted_sa.py
--rw-r--r--   0        0        0     2933 2023-02-24 14:38:20.570403 pysentimiento-0.7.0/pysentimiento/tass.py
--rw-r--r--   0        0        0     5854 2023-03-23 02:04:59.958986 pysentimiento-0.7.0/pysentimiento/training.py
--rw-r--r--   0        0        0     6585 2023-03-22 22:21:33.343555 pysentimiento-0.7.0/pysentimiento/tuning.py
--rw-r--r--   0        0        0      701 2023-01-24 15:07:24.172098 pysentimiento-0.7.0/pysentimiento/utils.py
--rw-r--r--   0        0        0     7921 1970-01-01 00:00:00.000000 pysentimiento-0.7.0/setup.py
--rw-r--r--   0        0        0     7733 1970-01-01 00:00:00.000000 pysentimiento-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      338 2023-01-24 15:07:24.092098 pysentimiento-0.7.0rc1/LICENSE.md
+-rw-r--r--   0        0        0     6799 2023-04-05 22:27:36.375881 pysentimiento-0.7.0rc1/README.md
+-rw-r--r--   0        0        0     1028 2023-04-19 19:32:39.218722 pysentimiento-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-03-30 11:51:24.383057 pysentimiento-0.7.0rc1/pysentimiento/__init__.py
+-rw-r--r--   0        0        0    20048 2023-04-19 19:02:33.630721 pysentimiento-0.7.0rc1/pysentimiento/analyzer.py
+-rw-r--r--   0        0        0       39 2023-01-24 15:07:24.172098 pysentimiento-0.7.0rc1/pysentimiento/baselines/__init__.py
+-rw-r--r--   0        0        0     4861 2023-01-24 15:07:24.172098 pysentimiento-0.7.0rc1/pysentimiento/baselines/models.py
+-rw-r--r--   0        0        0     5437 2023-01-31 20:16:06.893325 pysentimiento-0.7.0rc1/pysentimiento/baselines/training.py
+-rw-r--r--   0        0        0     1246 2023-01-24 15:07:24.172098 pysentimiento-0.7.0rc1/pysentimiento/baselines/utils.py
+-rw-r--r--   0        0        0      242 2023-02-24 14:38:20.566403 pysentimiento-0.7.0rc1/pysentimiento/config.py
+-rw-r--r--   0        0        0     3925 2023-03-03 13:56:08.310631 pysentimiento-0.7.0rc1/pysentimiento/emotion.py
+-rw-r--r--   0        0        0    11186 2023-02-27 12:26:28.317699 pysentimiento-0.7.0rc1/pysentimiento/hate.py
+-rw-r--r--   0        0        0     4330 2023-02-27 18:18:23.729976 pysentimiento-0.7.0rc1/pysentimiento/irony.py
+-rw-r--r--   0        0        0      119 2023-01-24 15:07:24.172098 pysentimiento-0.7.0rc1/pysentimiento/lince/__init__.py
+-rw-r--r--   0        0        0     7560 2023-02-24 14:38:20.566403 pysentimiento-0.7.0rc1/pysentimiento/lince/ner.py
+-rw-r--r--   0        0        0     3423 2023-02-24 14:38:20.570403 pysentimiento-0.7.0rc1/pysentimiento/lince/pos.py
+-rw-r--r--   0        0        0     1471 2023-02-24 14:38:20.570403 pysentimiento-0.7.0rc1/pysentimiento/lince/sentiment.py
+-rw-r--r--   0        0        0     1576 2023-01-24 15:07:24.172098 pysentimiento-0.7.0rc1/pysentimiento/metrics.py
+-rw-r--r--   0        0        0     6447 2023-03-29 23:37:11.649543 pysentimiento-0.7.0rc1/pysentimiento/preprocessing.py
+-rw-r--r--   0        0        0     2320 2023-02-24 14:38:20.570403 pysentimiento-0.7.0rc1/pysentimiento/semeval.py
+-rw-r--r--   0        0        0     2940 2023-02-27 11:52:33.917672 pysentimiento-0.7.0rc1/pysentimiento/sentiment.py
+-rw-r--r--   0        0        0      818 2023-02-24 14:39:51.342404 pysentimiento-0.7.0rc1/pysentimiento/sentiment_pt.py
+-rw-r--r--   0        0        0      825 2023-02-24 14:39:51.342404 pysentimiento-0.7.0rc1/pysentimiento/sentipolc.py
+-rw-r--r--   0        0        0     5356 2023-04-05 22:21:10.038814 pysentimiento-0.7.0rc1/pysentimiento/targeted_sa.py
+-rw-r--r--   0        0        0     2933 2023-02-24 14:38:20.570403 pysentimiento-0.7.0rc1/pysentimiento/tass.py
+-rw-r--r--   0        0        0     5854 2023-03-23 02:04:59.958986 pysentimiento-0.7.0rc1/pysentimiento/training.py
+-rw-r--r--   0        0        0     6585 2023-03-22 22:21:33.343555 pysentimiento-0.7.0rc1/pysentimiento/tuning.py
+-rw-r--r--   0        0        0      701 2023-01-24 15:07:24.172098 pysentimiento-0.7.0rc1/pysentimiento/utils.py
+-rw-r--r--   0        0        0     7799 1970-01-01 00:00:00.000000 pysentimiento-0.7.0rc1/setup.py
+-rw-r--r--   0        0        0     7608 1970-01-01 00:00:00.000000 pysentimiento-0.7.0rc1/PKG-INFO
```

### Comparing `pysentimiento-0.7.0/README.md` & `pysentimiento-0.7.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # pysentimiento: A Python toolkit for Sentiment Analysis and Social NLP tasks
 
-![Tests](https://github.com/finiteautomata/pysentimiento/workflows/run_tests/badge.svg) [![Test it in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)
-<a href="https://console.tiyaro.ai/explore?q=pysentimiento/robertuito-&pub=pysentimiento"> <img src="https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/try_on_tiyaro_badge.svg"></a>
+![Tests](https://github.com/finiteautomata/pysentimiento/workflows/run_tests/badge.svg)
+
+[![Test it in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)
 
+<p>
+<a href="https://console.tiyaro.ai/explore?q=pysentimiento/robertuito-&pub=pysentimiento"> <img src="https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/try_on_tiyaro_badge.svg"></a>
+</p>
 
 
 
 
 A Transformer-based library for SocialNLP tasks.
 
 Currently supports:
@@ -68,15 +72,14 @@
 See [TASKS](docs/TASKS.md) for more details on the supported tasks and languages, and also for reported performance for each benchmarked model.
 
 Also, check these notebooks with examples of how to use `pysentimiento` for each language:
 
 - [Spanish + English](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)
 - [Italian](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/sentiment_analysis_in_italian.ipynb)
 - [Portuguese](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/sentiment_analysis_in_portuguese.ipynb)
-- [Contextualized Hate Speech - Spanish](https://colab.research.google.com/drive/1nktGLswbVeEas2_xCU0S_BhmH8tPBJ02#scrollTo=Z5DeW-UrcI_E)
 
 ## Preprocessing
 
 `pysentimiento` features a tweet preprocessor specially suited for tweet classification with transformer-based models.
 
 ```python
 from pysentimiento.preprocessing import preprocess_tweet
```

#### html2text {}

```diff
@@ -1,56 +1,55 @@
 # pysentimiento: A Python toolkit for Sentiment Analysis and Social NLP tasks !
 [Tests](https://github.com/finiteautomata/pysentimiento/workflows/run_tests/
 badge.svg) [![Test it in Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/pysentimiento/
 pysentimiento/blob/master/notebooks/examples/
-pysentimiento_sentiment_analysis_in_spanish.ipynb) [https://tiyaro-public-
-docs.s3.us-west-2.amazonaws.com/assets/try_on_tiyaro_badge.svg] A Transformer-
-based library for SocialNLP tasks. Currently supports: | Task | Languages | |:-
--------------------- |:---------------------------------------| | Sentiment
-Analysis | es, en, it, pt | | Hate Speech Detection | es, en, it, pt | | Irony
-Detection | es, en, it, pt | | Emotion Analysis | es, en, it | | NER & POS
-tagging | es, en | | Contextualized Hate Speech Detection | es | | Targeted
-Sentiment Analysis | es | Just do `pip install pysentimiento` and start using
-it: ## Getting Started ```python from pysentimiento import create_analyzer
-analyzer = create_analyzer(task="sentiment", lang="es") analyzer.predict("QuÃ©
-gran jugador es Messi") # returns AnalyzerOutput(output=POS, probas={POS:
-0.998, NEG: 0.002, NEU: 0.000}) analyzer.predict("Esto es pÃ©simo") # returns
-AnalyzerOutput(output=NEG, probas={NEG: 0.999, POS: 0.001, NEU: 0.000})
-analyzer.predict("QuÃ© es esto?") # returns AnalyzerOutput(output=NEU, probas=
-{NEU: 0.993, NEG: 0.005, POS: 0.002}) analyzer.predict("jejeje no te creo
-mucho") # AnalyzerOutput(output=NEG, probas={NEG: 0.587, NEU: 0.408, POS:
-0.005}) """ Emotion Analysis in English """ emotion_analyzer = create_analyzer
-(task="emotion", lang="en") emotion_analyzer.predict("yayyy") # returns
-AnalyzerOutput(output=joy, probas={joy: 0.723, others: 0.198, surprise: 0.038,
-disgust: 0.011, sadness: 0.011, fear: 0.010, anger: 0.009})
-emotion_analyzer.predict("fuck off") # returns AnalyzerOutput(output=anger,
-probas={anger: 0.798, surprise: 0.055, fear: 0.040, disgust: 0.036, joy: 0.028,
-others: 0.023, sadness: 0.019}) """ Hate Speech (misogyny & racism) """
-hate_speech_analyzer = create_analyzer(task="hate_speech", lang="es")
-hate_speech_analyzer.predict("Esto es una mierda pero no es odio") # returns
-AnalyzerOutput(output=[], probas={hateful: 0.022, targeted: 0.009, aggressive:
-0.018}) hate_speech_analyzer.predict("Esto es odio porque los inmigrantes deben
-ser aniquilados") # returns AnalyzerOutput(output=['hateful'], probas={hateful:
-0.835, targeted: 0.008, aggressive: 0.476}) hate_speech_analyzer.predict("Vaya
-guarra barata y de poca monta es XXXX!") # returns AnalyzerOutput(output=
-['hateful', 'targeted', 'aggressive'], probas={hateful: 0.987, targeted: 0.978,
-aggressive: 0.969}) ``` See [TASKS](docs/TASKS.md) for more details on the
-supported tasks and languages, and also for reported performance for each
-benchmarked model. Also, check these notebooks with examples of how to use
-`pysentimiento` for each language: - [Spanish + English](https://
-colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/
-notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb) -
-[Italian](https://colab.research.google.com/github/pysentimiento/pysentimiento/
-blob/master/notebooks/examples/sentiment_analysis_in_italian.ipynb) -
-[Portuguese](https://colab.research.google.com/github/pysentimiento/
+pysentimiento_sentiment_analysis_in_spanish.ipynb)
+[https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/
+try_on_tiyaro_badge.svg]
+A Transformer-based library for SocialNLP tasks. Currently supports: | Task |
+Languages | |:--------------------- |:---------------------------------------
+| | Sentiment Analysis | es, en, it, pt | | Hate Speech Detection | es, en, it,
+pt | | Irony Detection | es, en, it, pt | | Emotion Analysis | es, en, it | |
+NER & POS tagging | es, en | | Contextualized Hate Speech Detection | es | |
+Targeted Sentiment Analysis | es | Just do `pip install pysentimiento` and
+start using it: ## Getting Started ```python from pysentimiento import
+create_analyzer analyzer = create_analyzer(task="sentiment", lang="es")
+analyzer.predict("QuÃ© gran jugador es Messi") # returns AnalyzerOutput
+(output=POS, probas={POS: 0.998, NEG: 0.002, NEU: 0.000}) analyzer.predict
+("Esto es pÃ©simo") # returns AnalyzerOutput(output=NEG, probas={NEG: 0.999,
+POS: 0.001, NEU: 0.000}) analyzer.predict("QuÃ© es esto?") # returns
+AnalyzerOutput(output=NEU, probas={NEU: 0.993, NEG: 0.005, POS: 0.002})
+analyzer.predict("jejeje no te creo mucho") # AnalyzerOutput(output=NEG,
+probas={NEG: 0.587, NEU: 0.408, POS: 0.005}) """ Emotion Analysis in English
+""" emotion_analyzer = create_analyzer(task="emotion", lang="en")
+emotion_analyzer.predict("yayyy") # returns AnalyzerOutput(output=joy, probas=
+{joy: 0.723, others: 0.198, surprise: 0.038, disgust: 0.011, sadness: 0.011,
+fear: 0.010, anger: 0.009}) emotion_analyzer.predict("fuck off") # returns
+AnalyzerOutput(output=anger, probas={anger: 0.798, surprise: 0.055, fear:
+0.040, disgust: 0.036, joy: 0.028, others: 0.023, sadness: 0.019}) """ Hate
+Speech (misogyny & racism) """ hate_speech_analyzer = create_analyzer
+(task="hate_speech", lang="es") hate_speech_analyzer.predict("Esto es una
+mierda pero no es odio") # returns AnalyzerOutput(output=[], probas={hateful:
+0.022, targeted: 0.009, aggressive: 0.018}) hate_speech_analyzer.predict("Esto
+es odio porque los inmigrantes deben ser aniquilados") # returns AnalyzerOutput
+(output=['hateful'], probas={hateful: 0.835, targeted: 0.008, aggressive:
+0.476}) hate_speech_analyzer.predict("Vaya guarra barata y de poca monta es
+XXXX!") # returns AnalyzerOutput(output=['hateful', 'targeted', 'aggressive'],
+probas={hateful: 0.987, targeted: 0.978, aggressive: 0.969}) ``` See [TASKS]
+(docs/TASKS.md) for more details on the supported tasks and languages, and also
+for reported performance for each benchmarked model. Also, check these
+notebooks with examples of how to use `pysentimiento` for each language: -
+[Spanish + English](https://colab.research.google.com/github/pysentimiento/
 pysentimiento/blob/master/notebooks/examples/
-sentiment_analysis_in_portuguese.ipynb) - [Contextualized Hate Speech -
-Spanish](https://colab.research.google.com/drive/
-1nktGLswbVeEas2_xCU0S_BhmH8tPBJ02#scrollTo=Z5DeW-UrcI_E) ## Preprocessing
+pysentimiento_sentiment_analysis_in_spanish.ipynb) - [Italian](https://
+colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/
+notebooks/examples/sentiment_analysis_in_italian.ipynb) - [Portuguese](https://
+colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/
+notebooks/examples/sentiment_analysis_in_portuguese.ipynb) ## Preprocessing
 `pysentimiento` features a tweet preprocessor specially suited for tweet
 classification with transformer-based models. ```python from
 pysentimiento.preprocessing import preprocess_tweet # Replaces user handles and
 URLs by special tokens preprocess_tweet("@perezjotaeme deberÃ­a cambiar esto
 http://bit.ly/sarasa") # "@usuario deberÃ­a cambiar esto url" # Shortens
 repeated characters preprocess_tweet("no entiendo naaaaaaaadaaaaaaaa",
 shorten=2) # "no entiendo naadaa" # Normalizes laughters preprocess_tweet
```

### Comparing `pysentimiento-0.7.0/pyproject.toml` & `pysentimiento-0.7.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysentimiento"
-version = "0.7.0"
+version = "0.7.0rc1"
 description = "A Transformer-based library for SocialNLP tasks"
 authors = ["Juan Manuel Pérez <jmperez@dc.uba.ar>", "Juan Carlos Giudici <jgiudici@dc.uba.ar>", ]
 readme = "README.md"
 repository = "https://github.com/pysentimiento/pysentimiento/"
 homepage = "https://github.com/pysentimiento/pysentimiento/"
 
 [tool.poetry.dependencies]
```

### Comparing `pysentimiento-0.7.0/pysentimiento/analyzer.py` & `pysentimiento-0.7.0rc1/pysentimiento/analyzer.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/baselines/models.py` & `pysentimiento-0.7.0rc1/pysentimiento/baselines/models.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/baselines/training.py` & `pysentimiento-0.7.0rc1/pysentimiento/baselines/training.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/baselines/utils.py` & `pysentimiento-0.7.0rc1/pysentimiento/baselines/utils.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/emotion.py` & `pysentimiento-0.7.0rc1/pysentimiento/emotion.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/hate.py` & `pysentimiento-0.7.0rc1/pysentimiento/hate.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/irony.py` & `pysentimiento-0.7.0rc1/pysentimiento/irony.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/lince/ner.py` & `pysentimiento-0.7.0rc1/pysentimiento/lince/ner.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/lince/pos.py` & `pysentimiento-0.7.0rc1/pysentimiento/lince/pos.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/lince/sentiment.py` & `pysentimiento-0.7.0rc1/pysentimiento/lince/sentiment.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/metrics.py` & `pysentimiento-0.7.0rc1/pysentimiento/metrics.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/preprocessing.py` & `pysentimiento-0.7.0rc1/pysentimiento/preprocessing.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/semeval.py` & `pysentimiento-0.7.0rc1/pysentimiento/semeval.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/sentiment.py` & `pysentimiento-0.7.0rc1/pysentimiento/sentiment.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/sentiment_pt.py` & `pysentimiento-0.7.0rc1/pysentimiento/sentiment_pt.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/sentipolc.py` & `pysentimiento-0.7.0rc1/pysentimiento/sentipolc.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/targeted_sa.py` & `pysentimiento-0.7.0rc1/pysentimiento/targeted_sa.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/tass.py` & `pysentimiento-0.7.0rc1/pysentimiento/tass.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/training.py` & `pysentimiento-0.7.0rc1/pysentimiento/training.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/tuning.py` & `pysentimiento-0.7.0rc1/pysentimiento/tuning.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/pysentimiento/utils.py` & `pysentimiento-0.7.0rc1/pysentimiento/utils.py`

 * *Files identical despite different names*

### Comparing `pysentimiento-0.7.0/setup.py` & `pysentimiento-0.7.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'emoji>=1.6.1,<2.0.0',
  'spacy>=3.5.0,<4.0.0',
  'torch==2.0.0',
  'transformers>=4.13.0']
 
 setup_kwargs = {
     'name': 'pysentimiento',
-    'version': '0.7.0',
+    'version': '0.7.0rc1',
     'description': 'A Transformer-based library for SocialNLP tasks',
-    'long_description': '# pysentimiento: A Python toolkit for Sentiment Analysis and Social NLP tasks\n\n![Tests](https://github.com/finiteautomata/pysentimiento/workflows/run_tests/badge.svg) [![Test it in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)\n<a href="https://console.tiyaro.ai/explore?q=pysentimiento/robertuito-&pub=pysentimiento"> <img src="https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/try_on_tiyaro_badge.svg"></a>\n\n\n\n\n\nA Transformer-based library for SocialNLP tasks.\n\nCurrently supports:\n\n\n| Task                                 | Languages                             |\n|:---------------------                |:---------------------------------------|\n| Sentiment Analysis                   | es, en, it, pt                        |\n| Hate Speech Detection                | es, en, it, pt                        |\n| Irony Detection                      | es, en, it, pt                        |\n| Emotion Analysis                     | es, en, it                            |\n| NER & POS tagging                    | es, en                                |\n| Contextualized Hate Speech Detection | es                                    |\n| Targeted Sentiment Analysis          | es                                    |\n\n\nJust do `pip install pysentimiento` and start using it:\n\n## Getting Started\n\n```python\nfrom pysentimiento import create_analyzer\nanalyzer = create_analyzer(task="sentiment", lang="es")\n\nanalyzer.predict("Qué gran jugador es Messi")\n# returns AnalyzerOutput(output=POS, probas={POS: 0.998, NEG: 0.002, NEU: 0.000})\nanalyzer.predict("Esto es pésimo")\n# returns AnalyzerOutput(output=NEG, probas={NEG: 0.999, POS: 0.001, NEU: 0.000})\nanalyzer.predict("Qué es esto?")\n# returns AnalyzerOutput(output=NEU, probas={NEU: 0.993, NEG: 0.005, POS: 0.002})\n\nanalyzer.predict("jejeje no te creo mucho")\n# AnalyzerOutput(output=NEG, probas={NEG: 0.587, NEU: 0.408, POS: 0.005})\n"""\nEmotion Analysis in English\n"""\n\nemotion_analyzer = create_analyzer(task="emotion", lang="en")\n\nemotion_analyzer.predict("yayyy")\n# returns AnalyzerOutput(output=joy, probas={joy: 0.723, others: 0.198, surprise: 0.038, disgust: 0.011, sadness: 0.011, fear: 0.010, anger: 0.009})\nemotion_analyzer.predict("fuck off")\n# returns AnalyzerOutput(output=anger, probas={anger: 0.798, surprise: 0.055, fear: 0.040, disgust: 0.036, joy: 0.028, others: 0.023, sadness: 0.019})\n\n"""\nHate Speech (misogyny & racism)\n"""\nhate_speech_analyzer = create_analyzer(task="hate_speech", lang="es")\n\nhate_speech_analyzer.predict("Esto es una mierda pero no es odio")\n# returns AnalyzerOutput(output=[], probas={hateful: 0.022, targeted: 0.009, aggressive: 0.018})\nhate_speech_analyzer.predict("Esto es odio porque los inmigrantes deben ser aniquilados")\n# returns AnalyzerOutput(output=[\'hateful\'], probas={hateful: 0.835, targeted: 0.008, aggressive: 0.476})\n\nhate_speech_analyzer.predict("Vaya guarra barata y de poca monta es XXXX!")\n# returns AnalyzerOutput(output=[\'hateful\', \'targeted\', \'aggressive\'], probas={hateful: 0.987, targeted: 0.978, aggressive: 0.969})\n```\n\nSee [TASKS](docs/TASKS.md) for more details on the supported tasks and languages, and also for reported performance for each benchmarked model.\n\nAlso, check these notebooks with examples of how to use `pysentimiento` for each language:\n\n- [Spanish + English](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)\n- [Italian](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/sentiment_analysis_in_italian.ipynb)\n- [Portuguese](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/sentiment_analysis_in_portuguese.ipynb)\n- [Contextualized Hate Speech - Spanish](https://colab.research.google.com/drive/1nktGLswbVeEas2_xCU0S_BhmH8tPBJ02#scrollTo=Z5DeW-UrcI_E)\n\n## Preprocessing\n\n`pysentimiento` features a tweet preprocessor specially suited for tweet classification with transformer-based models.\n\n```python\nfrom pysentimiento.preprocessing import preprocess_tweet\n\n# Replaces user handles and URLs by special tokens\npreprocess_tweet("@perezjotaeme debería cambiar esto http://bit.ly/sarasa") # "@usuario debería cambiar esto url"\n\n# Shortens repeated characters\npreprocess_tweet("no entiendo naaaaaaaadaaaaaaaa", shorten=2) # "no entiendo naadaa"\n\n# Normalizes laughters\npreprocess_tweet("jajajajaajjajaajajaja no lo puedo creer ajajaj") # "jaja no lo puedo creer jaja"\n\n# Handles hashtags\npreprocess_tweet("esto es #UnaGenialidad")\n# "esto es una genialidad"\n\n# Handles emojis\npreprocess_tweet("🎉🎉", lang="en")\n# \'emoji party popper emoji emoji party popper emoji\'\n```\n\n\n## Instructions for developers\n\n0. Clone and install\n\n```\ngit clone https://github.com/pysentimiento/pysentimiento\npip install poetry\npoetry shell\npoetry install\n```\n\n1. Run script to train models\n\nCheck [TRAIN.md](docs/TRAIN.md) for further information on how to train your models\n\nNote: you need access to the datasets, which are not public for the time being. Send us an email to get access to them.\n\n2. Upload models to Huggingface\'s Model Hub\n\nCheck ["Model sharing and upload"](https://huggingface.co/transformers/model_sharing.html) instructions in `huggingface` docs.\n\n## License\n\n`pysentimiento` is an open-source library. However, please be aware that models are trained with third-party datasets and are subject to their respective licenses, many of which are for non-commercial use\n\n1. [TASS Dataset license](http://tass.sepln.org/tass_data/download.php) (License for Sentiment Analysis in Spanish, Emotion Analysis in Spanish & English)\n2. [SEMEval 2017 Dataset license](https://www.dropbox.com/s/byzr8yoda6bua1b/2017_English_final.zip?file_subpath=%2F2017_English_final%2FDOWNLOAD%2FREADME.txt) (Sentiment Analysis in English)\n\n3. [LinCE Datasets](https://ritual.uh.edu/lince/datasets) (License for NER & POS tagging)\n\n## Suggestions and bugfixes\n\nPlease use the repository [issue tracker](https://github.com/pysentimiento/pysentimiento/issues) to point out bugs and make suggestions (new models, use another datasets, some other languages, etc)\n\n\n## Citation\n\nIf you use `pysentimiento` in your work, please cite [this paper](https://arxiv.org/abs/2106.09462)\n\n```\n@misc{perez2021pysentimiento,\n      title={pysentimiento: A Python Toolkit for Sentiment Analysis and SocialNLP tasks},\n      author={Juan Manuel Pérez and Juan Carlos Giudici and Franco Luque},\n      year={2021},\n      eprint={2106.09462},\n      archivePrefix={arXiv},\n      primaryClass={cs.CL}\n}\n```\n\nAlso, pleace cite related pre-trained models and datasets for the specific models you use. Check [REFERENCES](docs/REFERENCES.md) for details.\n\n',
+    'long_description': '# pysentimiento: A Python toolkit for Sentiment Analysis and Social NLP tasks\n\n![Tests](https://github.com/finiteautomata/pysentimiento/workflows/run_tests/badge.svg)\n\n[![Test it in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)\n\n<p>\n<a href="https://console.tiyaro.ai/explore?q=pysentimiento/robertuito-&pub=pysentimiento"> <img src="https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/try_on_tiyaro_badge.svg"></a>\n</p>\n\n\n\n\nA Transformer-based library for SocialNLP tasks.\n\nCurrently supports:\n\n\n| Task                                 | Languages                             |\n|:---------------------                |:---------------------------------------|\n| Sentiment Analysis                   | es, en, it, pt                        |\n| Hate Speech Detection                | es, en, it, pt                        |\n| Irony Detection                      | es, en, it, pt                        |\n| Emotion Analysis                     | es, en, it                            |\n| NER & POS tagging                    | es, en                                |\n| Contextualized Hate Speech Detection | es                                    |\n| Targeted Sentiment Analysis          | es                                    |\n\n\nJust do `pip install pysentimiento` and start using it:\n\n## Getting Started\n\n```python\nfrom pysentimiento import create_analyzer\nanalyzer = create_analyzer(task="sentiment", lang="es")\n\nanalyzer.predict("Qué gran jugador es Messi")\n# returns AnalyzerOutput(output=POS, probas={POS: 0.998, NEG: 0.002, NEU: 0.000})\nanalyzer.predict("Esto es pésimo")\n# returns AnalyzerOutput(output=NEG, probas={NEG: 0.999, POS: 0.001, NEU: 0.000})\nanalyzer.predict("Qué es esto?")\n# returns AnalyzerOutput(output=NEU, probas={NEU: 0.993, NEG: 0.005, POS: 0.002})\n\nanalyzer.predict("jejeje no te creo mucho")\n# AnalyzerOutput(output=NEG, probas={NEG: 0.587, NEU: 0.408, POS: 0.005})\n"""\nEmotion Analysis in English\n"""\n\nemotion_analyzer = create_analyzer(task="emotion", lang="en")\n\nemotion_analyzer.predict("yayyy")\n# returns AnalyzerOutput(output=joy, probas={joy: 0.723, others: 0.198, surprise: 0.038, disgust: 0.011, sadness: 0.011, fear: 0.010, anger: 0.009})\nemotion_analyzer.predict("fuck off")\n# returns AnalyzerOutput(output=anger, probas={anger: 0.798, surprise: 0.055, fear: 0.040, disgust: 0.036, joy: 0.028, others: 0.023, sadness: 0.019})\n\n"""\nHate Speech (misogyny & racism)\n"""\nhate_speech_analyzer = create_analyzer(task="hate_speech", lang="es")\n\nhate_speech_analyzer.predict("Esto es una mierda pero no es odio")\n# returns AnalyzerOutput(output=[], probas={hateful: 0.022, targeted: 0.009, aggressive: 0.018})\nhate_speech_analyzer.predict("Esto es odio porque los inmigrantes deben ser aniquilados")\n# returns AnalyzerOutput(output=[\'hateful\'], probas={hateful: 0.835, targeted: 0.008, aggressive: 0.476})\n\nhate_speech_analyzer.predict("Vaya guarra barata y de poca monta es XXXX!")\n# returns AnalyzerOutput(output=[\'hateful\', \'targeted\', \'aggressive\'], probas={hateful: 0.987, targeted: 0.978, aggressive: 0.969})\n```\n\nSee [TASKS](docs/TASKS.md) for more details on the supported tasks and languages, and also for reported performance for each benchmarked model.\n\nAlso, check these notebooks with examples of how to use `pysentimiento` for each language:\n\n- [Spanish + English](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)\n- [Italian](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/sentiment_analysis_in_italian.ipynb)\n- [Portuguese](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/sentiment_analysis_in_portuguese.ipynb)\n\n## Preprocessing\n\n`pysentimiento` features a tweet preprocessor specially suited for tweet classification with transformer-based models.\n\n```python\nfrom pysentimiento.preprocessing import preprocess_tweet\n\n# Replaces user handles and URLs by special tokens\npreprocess_tweet("@perezjotaeme debería cambiar esto http://bit.ly/sarasa") # "@usuario debería cambiar esto url"\n\n# Shortens repeated characters\npreprocess_tweet("no entiendo naaaaaaaadaaaaaaaa", shorten=2) # "no entiendo naadaa"\n\n# Normalizes laughters\npreprocess_tweet("jajajajaajjajaajajaja no lo puedo creer ajajaj") # "jaja no lo puedo creer jaja"\n\n# Handles hashtags\npreprocess_tweet("esto es #UnaGenialidad")\n# "esto es una genialidad"\n\n# Handles emojis\npreprocess_tweet("🎉🎉", lang="en")\n# \'emoji party popper emoji emoji party popper emoji\'\n```\n\n\n## Instructions for developers\n\n0. Clone and install\n\n```\ngit clone https://github.com/pysentimiento/pysentimiento\npip install poetry\npoetry shell\npoetry install\n```\n\n1. Run script to train models\n\nCheck [TRAIN.md](docs/TRAIN.md) for further information on how to train your models\n\nNote: you need access to the datasets, which are not public for the time being. Send us an email to get access to them.\n\n2. Upload models to Huggingface\'s Model Hub\n\nCheck ["Model sharing and upload"](https://huggingface.co/transformers/model_sharing.html) instructions in `huggingface` docs.\n\n## License\n\n`pysentimiento` is an open-source library. However, please be aware that models are trained with third-party datasets and are subject to their respective licenses, many of which are for non-commercial use\n\n1. [TASS Dataset license](http://tass.sepln.org/tass_data/download.php) (License for Sentiment Analysis in Spanish, Emotion Analysis in Spanish & English)\n2. [SEMEval 2017 Dataset license](https://www.dropbox.com/s/byzr8yoda6bua1b/2017_English_final.zip?file_subpath=%2F2017_English_final%2FDOWNLOAD%2FREADME.txt) (Sentiment Analysis in English)\n\n3. [LinCE Datasets](https://ritual.uh.edu/lince/datasets) (License for NER & POS tagging)\n\n## Suggestions and bugfixes\n\nPlease use the repository [issue tracker](https://github.com/pysentimiento/pysentimiento/issues) to point out bugs and make suggestions (new models, use another datasets, some other languages, etc)\n\n\n## Citation\n\nIf you use `pysentimiento` in your work, please cite [this paper](https://arxiv.org/abs/2106.09462)\n\n```\n@misc{perez2021pysentimiento,\n      title={pysentimiento: A Python Toolkit for Sentiment Analysis and SocialNLP tasks},\n      author={Juan Manuel Pérez and Juan Carlos Giudici and Franco Luque},\n      year={2021},\n      eprint={2106.09462},\n      archivePrefix={arXiv},\n      primaryClass={cs.CL}\n}\n```\n\nAlso, pleace cite related pre-trained models and datasets for the specific models you use. Check [REFERENCES](docs/REFERENCES.md) for details.\n\n',
     'author': 'Juan Manuel Pérez',
     'author_email': 'jmperez@dc.uba.ar',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pysentimiento/pysentimiento/',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,91 +1,90 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['pysentimiento', 'pysentimiento.baselines', 'pysentimiento.lince']
 package_data = \ {'': ['*']} install_requires = \ ['datasets>=1.13.3',
 'emoji>=1.6.1,<2.0.0', 'spacy>=3.5.0,<4.0.0', 'torch==2.0.0',
 'transformers>=4.13.0'] setup_kwargs = { 'name': 'pysentimiento', 'version':
-'0.7.0', 'description': 'A Transformer-based library for SocialNLP tasks',
+'0.7.0rc1', 'description': 'A Transformer-based library for SocialNLP tasks',
 'long_description': '# pysentimiento: A Python toolkit for Sentiment Analysis
 and Social NLP tasks\n\n![Tests](https://github.com/finiteautomata/
-pysentimiento/workflows/run_tests/badge.svg) [![Test it in Colab](https://
+pysentimiento/workflows/run_tests/badge.svg)\n\n[![Test it in Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/
-notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)\n[https:/
-/tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/
-try_on_tiyaro_badge.svg]\n\n\n\n\n\nA Transformer-based library for SocialNLP
-tasks.\n\nCurrently supports:\n\n\n| Task | Languages |\n|:--------------------
-- |:---------------------------------------|\n| Sentiment Analysis | es, en,
-it, pt |\n| Hate Speech Detection | es, en, it, pt |\n| Irony Detection | es,
-en, it, pt |\n| Emotion Analysis | es, en, it |\n| NER & POS tagging | es, en
-|\n| Contextualized Hate Speech Detection | es |\n| Targeted Sentiment Analysis
-| es |\n\n\nJust do `pip install pysentimiento` and start using it:\n\n##
-Getting Started\n\n```python\nfrom pysentimiento import
-create_analyzer\nanalyzer = create_analyzer(task="sentiment",
-lang="es")\n\nanalyzer.predict("QuÃ© gran jugador es Messi")\n# returns
-AnalyzerOutput(output=POS, probas={POS: 0.998, NEG: 0.002, NEU:
-0.000})\nanalyzer.predict("Esto es pÃ©simo")\n# returns AnalyzerOutput
-(output=NEG, probas={NEG: 0.999, POS: 0.001, NEU: 0.000})\nanalyzer.predict
-("QuÃ© es esto?")\n# returns AnalyzerOutput(output=NEU, probas={NEU: 0.993,
-NEG: 0.005, POS: 0.002})\n\nanalyzer.predict("jejeje no te creo mucho")\n#
-AnalyzerOutput(output=NEG, probas={NEG: 0.587, NEU: 0.408, POS:
-0.005})\n"""\nEmotion Analysis in English\n"""\n\nemotion_analyzer =
-create_analyzer(task="emotion", lang="en")\n\nemotion_analyzer.predict
-("yayyy")\n# returns AnalyzerOutput(output=joy, probas={joy: 0.723, others:
-0.198, surprise: 0.038, disgust: 0.011, sadness: 0.011, fear: 0.010, anger:
-0.009})\nemotion_analyzer.predict("fuck off")\n# returns AnalyzerOutput
-(output=anger, probas={anger: 0.798, surprise: 0.055, fear: 0.040, disgust:
-0.036, joy: 0.028, others: 0.023, sadness: 0.019})\n\n"""\nHate Speech
-(misogyny & racism)\n"""\nhate_speech_analyzer = create_analyzer
-(task="hate_speech", lang="es")\n\nhate_speech_analyzer.predict("Esto es una
-mierda pero no es odio")\n# returns AnalyzerOutput(output=[], probas={hateful:
-0.022, targeted: 0.009, aggressive: 0.018})\nhate_speech_analyzer.predict("Esto
-es odio porque los inmigrantes deben ser aniquilados")\n# returns
-AnalyzerOutput(output=[\'hateful\'], probas={hateful: 0.835, targeted: 0.008,
-aggressive: 0.476})\n\nhate_speech_analyzer.predict("Vaya guarra barata y de
-poca monta es XXXX!")\n# returns AnalyzerOutput(output=[\'hateful\',
-\'targeted\', \'aggressive\'], probas={hateful: 0.987, targeted: 0.978,
-aggressive: 0.969})\n```\n\nSee [TASKS](docs/TASKS.md) for more details on the
-supported tasks and languages, and also for reported performance for each
-benchmarked model.\n\nAlso, check these notebooks with examples of how to use
+notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)\n\n
+\n[https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/
+try_on_tiyaro_badge.svg]\n
+\n\n\n\n\nA Transformer-based library for SocialNLP tasks.\n\nCurrently
+supports:\n\n\n| Task | Languages |\n|:--------------------- |:----------------
+-----------------------|\n| Sentiment Analysis | es, en, it, pt |\n| Hate
+Speech Detection | es, en, it, pt |\n| Irony Detection | es, en, it, pt |\n|
+Emotion Analysis | es, en, it |\n| NER & POS tagging | es, en |\n|
+Contextualized Hate Speech Detection | es |\n| Targeted Sentiment Analysis | es
+|\n\n\nJust do `pip install pysentimiento` and start using it:\n\n## Getting
+Started\n\n```python\nfrom pysentimiento import create_analyzer\nanalyzer =
+create_analyzer(task="sentiment", lang="es")\n\nanalyzer.predict("QuÃ© gran
+jugador es Messi")\n# returns AnalyzerOutput(output=POS, probas={POS: 0.998,
+NEG: 0.002, NEU: 0.000})\nanalyzer.predict("Esto es pÃ©simo")\n# returns
+AnalyzerOutput(output=NEG, probas={NEG: 0.999, POS: 0.001, NEU:
+0.000})\nanalyzer.predict("QuÃ© es esto?")\n# returns AnalyzerOutput
+(output=NEU, probas={NEU: 0.993, NEG: 0.005, POS: 0.002})\n\nanalyzer.predict
+("jejeje no te creo mucho")\n# AnalyzerOutput(output=NEG, probas={NEG: 0.587,
+NEU: 0.408, POS: 0.005})\n"""\nEmotion Analysis in
+English\n"""\n\nemotion_analyzer = create_analyzer(task="emotion",
+lang="en")\n\nemotion_analyzer.predict("yayyy")\n# returns AnalyzerOutput
+(output=joy, probas={joy: 0.723, others: 0.198, surprise: 0.038, disgust:
+0.011, sadness: 0.011, fear: 0.010, anger: 0.009})\nemotion_analyzer.predict
+("fuck off")\n# returns AnalyzerOutput(output=anger, probas={anger: 0.798,
+surprise: 0.055, fear: 0.040, disgust: 0.036, joy: 0.028, others: 0.023,
+sadness: 0.019})\n\n"""\nHate Speech (misogyny &
+racism)\n"""\nhate_speech_analyzer = create_analyzer(task="hate_speech",
+lang="es")\n\nhate_speech_analyzer.predict("Esto es una mierda pero no es
+odio")\n# returns AnalyzerOutput(output=[], probas={hateful: 0.022, targeted:
+0.009, aggressive: 0.018})\nhate_speech_analyzer.predict("Esto es odio porque
+los inmigrantes deben ser aniquilados")\n# returns AnalyzerOutput(output=
+[\'hateful\'], probas={hateful: 0.835, targeted: 0.008, aggressive:
+0.476})\n\nhate_speech_analyzer.predict("Vaya guarra barata y de poca monta es
+XXXX!")\n# returns AnalyzerOutput(output=[\'hateful\', \'targeted\',
+\'aggressive\'], probas={hateful: 0.987, targeted: 0.978, aggressive:
+0.969})\n```\n\nSee [TASKS](docs/TASKS.md) for more details on the supported
+tasks and languages, and also for reported performance for each benchmarked
+model.\n\nAlso, check these notebooks with examples of how to use
 `pysentimiento` for each language:\n\n- [Spanish + English](https://
 colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/
 notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)\n-
 [Italian](https://colab.research.google.com/github/pysentimiento/pysentimiento/
 blob/master/notebooks/examples/sentiment_analysis_in_italian.ipynb)\n-
 [Portuguese](https://colab.research.google.com/github/pysentimiento/
 pysentimiento/blob/master/notebooks/examples/
-sentiment_analysis_in_portuguese.ipynb)\n- [Contextualized Hate Speech -
-Spanish](https://colab.research.google.com/drive/
-1nktGLswbVeEas2_xCU0S_BhmH8tPBJ02#scrollTo=Z5DeW-UrcI_E)\n\n##
-Preprocessing\n\n`pysentimiento` features a tweet preprocessor specially suited
-for tweet classification with transformer-based models.\n\n```python\nfrom
-pysentimiento.preprocessing import preprocess_tweet\n\n# Replaces user handles
-and URLs by special tokens\npreprocess_tweet("@perezjotaeme deberÃ­a cambiar
-esto http://bit.ly/sarasa") # "@usuario deberÃ­a cambiar esto url"\n\n#
-Shortens repeated characters\npreprocess_tweet("no entiendo
-naaaaaaaadaaaaaaaa", shorten=2) # "no entiendo naadaa"\n\n# Normalizes
-laughters\npreprocess_tweet("jajajajaajjajaajajaja no lo puedo creer ajajaj") #
-"jaja no lo puedo creer jaja"\n\n# Handles hashtags\npreprocess_tweet("esto es
-#UnaGenialidad")\n# "esto es una genialidad"\n\n# Handles
-emojis\npreprocess_tweet("ðð", lang="en")\n# \'emoji party popper emoji
-emoji party popper emoji\'\n```\n\n\n## Instructions for developers\n\n0. Clone
-and install\n\n```\ngit clone https://github.com/pysentimiento/
-pysentimiento\npip install poetry\npoetry shell\npoetry install\n```\n\n1. Run
-script to train models\n\nCheck [TRAIN.md](docs/TRAIN.md) for further
-information on how to train your models\n\nNote: you need access to the
-datasets, which are not public for the time being. Send us an email to get
-access to them.\n\n2. Upload models to Huggingface\'s Model Hub\n\nCheck
-["Model sharing and upload"](https://huggingface.co/transformers/
-model_sharing.html) instructions in `huggingface` docs.\n\n##
-License\n\n`pysentimiento` is an open-source library. However, please be aware
-that models are trained with third-party datasets and are subject to their
-respective licenses, many of which are for non-commercial use\n\n1. [TASS
-Dataset license](http://tass.sepln.org/tass_data/download.php) (License for
-Sentiment Analysis in Spanish, Emotion Analysis in Spanish & English)\n2.
-[SEMEval 2017 Dataset license](https://www.dropbox.com/s/byzr8yoda6bua1b/
+sentiment_analysis_in_portuguese.ipynb)\n\n## Preprocessing\n\n`pysentimiento`
+features a tweet preprocessor specially suited for tweet classification with
+transformer-based models.\n\n```python\nfrom pysentimiento.preprocessing import
+preprocess_tweet\n\n# Replaces user handles and URLs by special
+tokens\npreprocess_tweet("@perezjotaeme deberÃ­a cambiar esto http://bit.ly/
+sarasa") # "@usuario deberÃ­a cambiar esto url"\n\n# Shortens repeated
+characters\npreprocess_tweet("no entiendo naaaaaaaadaaaaaaaa", shorten=2) # "no
+entiendo naadaa"\n\n# Normalizes laughters\npreprocess_tweet
+("jajajajaajjajaajajaja no lo puedo creer ajajaj") # "jaja no lo puedo creer
+jaja"\n\n# Handles hashtags\npreprocess_tweet("esto es #UnaGenialidad")\n#
+"esto es una genialidad"\n\n# Handles emojis\npreprocess_tweet("ðð",
+lang="en")\n# \'emoji party popper emoji emoji party popper
+emoji\'\n```\n\n\n## Instructions for developers\n\n0. Clone and
+install\n\n```\ngit clone https://github.com/pysentimiento/pysentimiento\npip
+install poetry\npoetry shell\npoetry install\n```\n\n1. Run script to train
+models\n\nCheck [TRAIN.md](docs/TRAIN.md) for further information on how to
+train your models\n\nNote: you need access to the datasets, which are not
+public for the time being. Send us an email to get access to them.\n\n2. Upload
+models to Huggingface\'s Model Hub\n\nCheck ["Model sharing and upload"](https:
+//huggingface.co/transformers/model_sharing.html) instructions in `huggingface`
+docs.\n\n## License\n\n`pysentimiento` is an open-source library. However,
+please be aware that models are trained with third-party datasets and are
+subject to their respective licenses, many of which are for non-commercial
+use\n\n1. [TASS Dataset license](http://tass.sepln.org/tass_data/download.php)
+(License for Sentiment Analysis in Spanish, Emotion Analysis in Spanish &
+English)\n2. [SEMEval 2017 Dataset license](https://www.dropbox.com/s/
+byzr8yoda6bua1b/
 2017_English_final.zip?file_subpath=%2F2017_English_final%2FDOWNLOAD%2FREADME.txt)
 (Sentiment Analysis in English)\n\n3. [LinCE Datasets](https://ritual.uh.edu/
 lince/datasets) (License for NER & POS tagging)\n\n## Suggestions and
 bugfixes\n\nPlease use the repository [issue tracker](https://github.com/
 pysentimiento/pysentimiento/issues) to point out bugs and make suggestions (new
 models, use another datasets, some other languages, etc)\n\n\n## Citation\n\nIf
 you use `pysentimiento` in your work, please cite [this paper](https://
```

### Comparing `pysentimiento-0.7.0/PKG-INFO` & `pysentimiento-0.7.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysentimiento
-Version: 0.7.0
+Version: 0.7.0rc1
 Summary: A Transformer-based library for SocialNLP tasks
 Home-page: https://github.com/pysentimiento/pysentimiento/
 Author: Juan Manuel Pérez
 Author-email: jmperez@dc.uba.ar
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -17,17 +17,21 @@
 Requires-Dist: torch (==2.0.0)
 Requires-Dist: transformers (>=4.13.0)
 Project-URL: Repository, https://github.com/pysentimiento/pysentimiento/
 Description-Content-Type: text/markdown
 
 # pysentimiento: A Python toolkit for Sentiment Analysis and Social NLP tasks
 
-![Tests](https://github.com/finiteautomata/pysentimiento/workflows/run_tests/badge.svg) [![Test it in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)
-<a href="https://console.tiyaro.ai/explore?q=pysentimiento/robertuito-&pub=pysentimiento"> <img src="https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/try_on_tiyaro_badge.svg"></a>
+![Tests](https://github.com/finiteautomata/pysentimiento/workflows/run_tests/badge.svg)
+
+[![Test it in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)
 
+<p>
+<a href="https://console.tiyaro.ai/explore?q=pysentimiento/robertuito-&pub=pysentimiento"> <img src="https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/try_on_tiyaro_badge.svg"></a>
+</p>
 
 
 
 
 A Transformer-based library for SocialNLP tasks.
 
 Currently supports:
@@ -89,15 +93,14 @@
 See [TASKS](docs/TASKS.md) for more details on the supported tasks and languages, and also for reported performance for each benchmarked model.
 
 Also, check these notebooks with examples of how to use `pysentimiento` for each language:
 
 - [Spanish + English](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb)
 - [Italian](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/sentiment_analysis_in_italian.ipynb)
 - [Portuguese](https://colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/notebooks/examples/sentiment_analysis_in_portuguese.ipynb)
-- [Contextualized Hate Speech - Spanish](https://colab.research.google.com/drive/1nktGLswbVeEas2_xCU0S_BhmH8tPBJ02#scrollTo=Z5DeW-UrcI_E)
 
 ## Preprocessing
 
 `pysentimiento` features a tweet preprocessor specially suited for tweet classification with transformer-based models.
 
 ```python
 from pysentimiento.preprocessing import preprocess_tweet
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pysentimiento Version: 0.7.0 Summary: A
+Metadata-Version: 2.1 Name: pysentimiento Version: 0.7.0rc1 Summary: A
 Transformer-based library for SocialNLP tasks Home-page: https://github.com/
 pysentimiento/pysentimiento/ Author: Juan Manuel PÃ©rez Author-email:
 jmperez@dc.uba.ar Requires-Python: >=3.8,<4.0 Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: datasets (>=1.13.3) Requires-Dist: emoji (>=1.6.1,<2.0.0) Requires-Dist:
@@ -10,58 +10,57 @@
 transformers (>=4.13.0) Project-URL: Repository, https://github.com/
 pysentimiento/pysentimiento/ Description-Content-Type: text/markdown #
 pysentimiento: A Python toolkit for Sentiment Analysis and Social NLP tasks !
 [Tests](https://github.com/finiteautomata/pysentimiento/workflows/run_tests/
 badge.svg) [![Test it in Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/pysentimiento/
 pysentimiento/blob/master/notebooks/examples/
-pysentimiento_sentiment_analysis_in_spanish.ipynb) [https://tiyaro-public-
-docs.s3.us-west-2.amazonaws.com/assets/try_on_tiyaro_badge.svg] A Transformer-
-based library for SocialNLP tasks. Currently supports: | Task | Languages | |:-
--------------------- |:---------------------------------------| | Sentiment
-Analysis | es, en, it, pt | | Hate Speech Detection | es, en, it, pt | | Irony
-Detection | es, en, it, pt | | Emotion Analysis | es, en, it | | NER & POS
-tagging | es, en | | Contextualized Hate Speech Detection | es | | Targeted
-Sentiment Analysis | es | Just do `pip install pysentimiento` and start using
-it: ## Getting Started ```python from pysentimiento import create_analyzer
-analyzer = create_analyzer(task="sentiment", lang="es") analyzer.predict("QuÃ©
-gran jugador es Messi") # returns AnalyzerOutput(output=POS, probas={POS:
-0.998, NEG: 0.002, NEU: 0.000}) analyzer.predict("Esto es pÃ©simo") # returns
-AnalyzerOutput(output=NEG, probas={NEG: 0.999, POS: 0.001, NEU: 0.000})
-analyzer.predict("QuÃ© es esto?") # returns AnalyzerOutput(output=NEU, probas=
-{NEU: 0.993, NEG: 0.005, POS: 0.002}) analyzer.predict("jejeje no te creo
-mucho") # AnalyzerOutput(output=NEG, probas={NEG: 0.587, NEU: 0.408, POS:
-0.005}) """ Emotion Analysis in English """ emotion_analyzer = create_analyzer
-(task="emotion", lang="en") emotion_analyzer.predict("yayyy") # returns
-AnalyzerOutput(output=joy, probas={joy: 0.723, others: 0.198, surprise: 0.038,
-disgust: 0.011, sadness: 0.011, fear: 0.010, anger: 0.009})
-emotion_analyzer.predict("fuck off") # returns AnalyzerOutput(output=anger,
-probas={anger: 0.798, surprise: 0.055, fear: 0.040, disgust: 0.036, joy: 0.028,
-others: 0.023, sadness: 0.019}) """ Hate Speech (misogyny & racism) """
-hate_speech_analyzer = create_analyzer(task="hate_speech", lang="es")
-hate_speech_analyzer.predict("Esto es una mierda pero no es odio") # returns
-AnalyzerOutput(output=[], probas={hateful: 0.022, targeted: 0.009, aggressive:
-0.018}) hate_speech_analyzer.predict("Esto es odio porque los inmigrantes deben
-ser aniquilados") # returns AnalyzerOutput(output=['hateful'], probas={hateful:
-0.835, targeted: 0.008, aggressive: 0.476}) hate_speech_analyzer.predict("Vaya
-guarra barata y de poca monta es XXXX!") # returns AnalyzerOutput(output=
-['hateful', 'targeted', 'aggressive'], probas={hateful: 0.987, targeted: 0.978,
-aggressive: 0.969}) ``` See [TASKS](docs/TASKS.md) for more details on the
-supported tasks and languages, and also for reported performance for each
-benchmarked model. Also, check these notebooks with examples of how to use
-`pysentimiento` for each language: - [Spanish + English](https://
-colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/
-notebooks/examples/pysentimiento_sentiment_analysis_in_spanish.ipynb) -
-[Italian](https://colab.research.google.com/github/pysentimiento/pysentimiento/
-blob/master/notebooks/examples/sentiment_analysis_in_italian.ipynb) -
-[Portuguese](https://colab.research.google.com/github/pysentimiento/
+pysentimiento_sentiment_analysis_in_spanish.ipynb)
+[https://tiyaro-public-docs.s3.us-west-2.amazonaws.com/assets/
+try_on_tiyaro_badge.svg]
+A Transformer-based library for SocialNLP tasks. Currently supports: | Task |
+Languages | |:--------------------- |:---------------------------------------
+| | Sentiment Analysis | es, en, it, pt | | Hate Speech Detection | es, en, it,
+pt | | Irony Detection | es, en, it, pt | | Emotion Analysis | es, en, it | |
+NER & POS tagging | es, en | | Contextualized Hate Speech Detection | es | |
+Targeted Sentiment Analysis | es | Just do `pip install pysentimiento` and
+start using it: ## Getting Started ```python from pysentimiento import
+create_analyzer analyzer = create_analyzer(task="sentiment", lang="es")
+analyzer.predict("QuÃ© gran jugador es Messi") # returns AnalyzerOutput
+(output=POS, probas={POS: 0.998, NEG: 0.002, NEU: 0.000}) analyzer.predict
+("Esto es pÃ©simo") # returns AnalyzerOutput(output=NEG, probas={NEG: 0.999,
+POS: 0.001, NEU: 0.000}) analyzer.predict("QuÃ© es esto?") # returns
+AnalyzerOutput(output=NEU, probas={NEU: 0.993, NEG: 0.005, POS: 0.002})
+analyzer.predict("jejeje no te creo mucho") # AnalyzerOutput(output=NEG,
+probas={NEG: 0.587, NEU: 0.408, POS: 0.005}) """ Emotion Analysis in English
+""" emotion_analyzer = create_analyzer(task="emotion", lang="en")
+emotion_analyzer.predict("yayyy") # returns AnalyzerOutput(output=joy, probas=
+{joy: 0.723, others: 0.198, surprise: 0.038, disgust: 0.011, sadness: 0.011,
+fear: 0.010, anger: 0.009}) emotion_analyzer.predict("fuck off") # returns
+AnalyzerOutput(output=anger, probas={anger: 0.798, surprise: 0.055, fear:
+0.040, disgust: 0.036, joy: 0.028, others: 0.023, sadness: 0.019}) """ Hate
+Speech (misogyny & racism) """ hate_speech_analyzer = create_analyzer
+(task="hate_speech", lang="es") hate_speech_analyzer.predict("Esto es una
+mierda pero no es odio") # returns AnalyzerOutput(output=[], probas={hateful:
+0.022, targeted: 0.009, aggressive: 0.018}) hate_speech_analyzer.predict("Esto
+es odio porque los inmigrantes deben ser aniquilados") # returns AnalyzerOutput
+(output=['hateful'], probas={hateful: 0.835, targeted: 0.008, aggressive:
+0.476}) hate_speech_analyzer.predict("Vaya guarra barata y de poca monta es
+XXXX!") # returns AnalyzerOutput(output=['hateful', 'targeted', 'aggressive'],
+probas={hateful: 0.987, targeted: 0.978, aggressive: 0.969}) ``` See [TASKS]
+(docs/TASKS.md) for more details on the supported tasks and languages, and also
+for reported performance for each benchmarked model. Also, check these
+notebooks with examples of how to use `pysentimiento` for each language: -
+[Spanish + English](https://colab.research.google.com/github/pysentimiento/
 pysentimiento/blob/master/notebooks/examples/
-sentiment_analysis_in_portuguese.ipynb) - [Contextualized Hate Speech -
-Spanish](https://colab.research.google.com/drive/
-1nktGLswbVeEas2_xCU0S_BhmH8tPBJ02#scrollTo=Z5DeW-UrcI_E) ## Preprocessing
+pysentimiento_sentiment_analysis_in_spanish.ipynb) - [Italian](https://
+colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/
+notebooks/examples/sentiment_analysis_in_italian.ipynb) - [Portuguese](https://
+colab.research.google.com/github/pysentimiento/pysentimiento/blob/master/
+notebooks/examples/sentiment_analysis_in_portuguese.ipynb) ## Preprocessing
 `pysentimiento` features a tweet preprocessor specially suited for tweet
 classification with transformer-based models. ```python from
 pysentimiento.preprocessing import preprocess_tweet # Replaces user handles and
 URLs by special tokens preprocess_tweet("@perezjotaeme deberÃ­a cambiar esto
 http://bit.ly/sarasa") # "@usuario deberÃ­a cambiar esto url" # Shortens
 repeated characters preprocess_tweet("no entiendo naaaaaaaadaaaaaaaa",
 shorten=2) # "no entiendo naadaa" # Normalizes laughters preprocess_tweet
```

