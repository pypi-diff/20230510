# Comparing `tmp/akkadian-1.0.8.tar.gz` & `tmp/akkadian-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\akkadian-1.0.8.tar", last modified: Sat Aug 22 21:22:52 2020, max compression
+gzip compressed data, was "dist\akkadian-1.0.9.tar", last modified: Sat Aug 22 23:08:48 2020, max compression
```

## Comparing `akkadian-1.0.8.tar` & `akkadian-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2020-08-22 21:22:52.000000 akkadian-1.0.8/
--rw-rw-rw-   0        0        0    15110 2020-08-22 21:22:52.000000 akkadian-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    12447 2020-08-15 12:54:39.000000 akkadian-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2020-08-22 21:22:52.000000 akkadian-1.0.8/akkadian/
--rw-rw-rw-   0        0        0     1970 2020-08-11 11:36:24.000000 akkadian-1.0.8/akkadian/__init__.py
--rw-rw-rw-   0        0        0     8868 2020-08-12 21:46:38.000000 akkadian-1.0.8/akkadian/bilstm.py
--rw-rw-rw-   0        0        0     7731 2020-08-12 21:46:38.000000 akkadian-1.0.8/akkadian/build_data.py
--rw-rw-rw-   0        0        0    12408 2020-07-24 11:18:04.000000 akkadian-1.0.8/akkadian/check_translation.py
--rw-rw-rw-   0        0        0    10831 2020-07-24 10:00:06.000000 akkadian-1.0.8/akkadian/combine_algorithms.py
--rw-rw-rw-   0        0        0     9705 2020-08-08 22:11:48.000000 akkadian-1.0.8/akkadian/data.py
--rw-rw-rw-   0        0        0    20843 2020-07-24 10:00:06.000000 akkadian-1.0.8/akkadian/full_translation_build_data.py
--rw-rw-rw-   0        0        0     1109 2020-05-16 15:18:18.000000 akkadian-1.0.8/akkadian/get_texts_details.py
--rw-rw-rw-   0        0        0    12164 2020-08-12 21:46:38.000000 akkadian-1.0.8/akkadian/hmm.py
--rw-rw-rw-   0        0        0    18764 2020-08-12 21:46:38.000000 akkadian-1.0.8/akkadian/memm.py
--rw-rw-rw-   0        0        0    10181 2020-05-28 14:24:48.000000 akkadian-1.0.8/akkadian/parse_json.py
--rw-rw-rw-   0        0        0    12282 2020-08-12 21:46:39.000000 akkadian-1.0.8/akkadian/parse_xml.py
--rw-rw-rw-   0        0        0     3997 2020-08-22 21:19:46.000000 akkadian-1.0.8/akkadian/train.py
--rw-rw-rw-   0        0        0     1611 2020-03-29 14:36:06.000000 akkadian-1.0.8/akkadian/translation_tokenize.py
--rw-rw-rw-   0        0        0     7116 2020-08-18 19:23:49.000000 akkadian-1.0.8/akkadian/transliterate.py
-drwxrwxrwx   0        0        0        0 2020-08-22 21:22:52.000000 akkadian-1.0.8/akkadian.egg-info/
--rw-rw-rw-   0        0        0    15110 2020-08-22 21:22:51.000000 akkadian-1.0.8/akkadian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      543 2020-08-22 21:22:51.000000 akkadian-1.0.8/akkadian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-08-22 21:22:51.000000 akkadian-1.0.8/akkadian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2020-08-22 21:22:51.000000 akkadian-1.0.8/akkadian.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2020-08-22 21:22:51.000000 akkadian-1.0.8/akkadian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-08-22 21:22:52.000000 akkadian-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1034 2020-08-22 21:21:56.000000 akkadian-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2020-08-22 23:08:48.000000 akkadian-1.0.9/
+-rw-rw-rw-   0        0        0    15110 2020-08-22 23:08:48.000000 akkadian-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12447 2020-08-15 12:54:39.000000 akkadian-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2020-08-22 23:08:48.000000 akkadian-1.0.9/akkadian/
+-rw-rw-rw-   0        0        0     1970 2020-08-11 11:36:24.000000 akkadian-1.0.9/akkadian/__init__.py
+-rw-rw-rw-   0        0        0     8868 2020-08-12 21:46:38.000000 akkadian-1.0.9/akkadian/bilstm.py
+-rw-rw-rw-   0        0        0     7731 2020-08-22 22:37:12.000000 akkadian-1.0.9/akkadian/build_data.py
+-rw-rw-rw-   0        0        0    12408 2020-07-24 11:18:04.000000 akkadian-1.0.9/akkadian/check_translation.py
+-rw-rw-rw-   0        0        0    10831 2020-07-24 10:00:06.000000 akkadian-1.0.9/akkadian/combine_algorithms.py
+-rw-rw-rw-   0        0        0     9705 2020-08-08 22:11:48.000000 akkadian-1.0.9/akkadian/data.py
+-rw-rw-rw-   0        0        0    20843 2020-07-24 10:00:06.000000 akkadian-1.0.9/akkadian/full_translation_build_data.py
+-rw-rw-rw-   0        0        0     1109 2020-05-16 15:18:18.000000 akkadian-1.0.9/akkadian/get_texts_details.py
+-rw-rw-rw-   0        0        0    12164 2020-08-12 21:46:38.000000 akkadian-1.0.9/akkadian/hmm.py
+-rw-rw-rw-   0        0        0    18764 2020-08-12 21:46:38.000000 akkadian-1.0.9/akkadian/memm.py
+-rw-rw-rw-   0        0        0    10181 2020-05-28 14:24:48.000000 akkadian-1.0.9/akkadian/parse_json.py
+-rw-rw-rw-   0        0        0    12282 2020-08-12 21:46:39.000000 akkadian-1.0.9/akkadian/parse_xml.py
+-rw-rw-rw-   0        0        0     3997 2020-08-22 23:06:15.000000 akkadian-1.0.9/akkadian/train.py
+-rw-rw-rw-   0        0        0     1611 2020-03-29 14:36:06.000000 akkadian-1.0.9/akkadian/translation_tokenize.py
+-rw-rw-rw-   0        0        0     7466 2020-08-22 23:06:34.000000 akkadian-1.0.9/akkadian/transliterate.py
+drwxrwxrwx   0        0        0        0 2020-08-22 23:08:48.000000 akkadian-1.0.9/akkadian.egg-info/
+-rw-rw-rw-   0        0        0    15110 2020-08-22 23:08:47.000000 akkadian-1.0.9/akkadian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2020-08-22 23:08:47.000000 akkadian-1.0.9/akkadian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-08-22 23:08:47.000000 akkadian-1.0.9/akkadian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2020-08-22 23:08:47.000000 akkadian-1.0.9/akkadian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2020-08-22 23:08:47.000000 akkadian-1.0.9/akkadian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-08-22 23:08:48.000000 akkadian-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1034 2020-08-22 23:08:35.000000 akkadian-1.0.9/setup.py
```

### Comparing `akkadian-1.0.8/PKG-INFO` & `akkadian-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akkadian
-Version: 1.0.8
+Version: 1.0.9
 Summary: Translating Akkadian signs to transliteration using NLP algorithms
 Home-page: https://github.com/gaigutherz/Translating-Akkadian-using-NLP
 Author: Ariel Elazary, Gai Gutherz
 Author-email: am.elazary@gmail.com, gaigutherz@gmail.com
 License: UNKNOWN
 Description: # Akkademia
         Akkademia is a tool for automatically transliterating Unicode cuneiform glyphs. It is written in python script and uses HMM, MEMM and BiLSTM neural networks to determine appropriate sign-readings and segmentation.
```

### Comparing `akkadian-1.0.8/README.md` & `akkadian-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/__init__.py` & `akkadian-1.0.9/akkadian/__init__.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/bilstm.py` & `akkadian-1.0.9/akkadian/bilstm.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/build_data.py` & `akkadian-1.0.9/akkadian/build_data.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/check_translation.py` & `akkadian-1.0.9/akkadian/check_translation.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/combine_algorithms.py` & `akkadian-1.0.9/akkadian/combine_algorithms.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/data.py` & `akkadian-1.0.9/akkadian/data.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/full_translation_build_data.py` & `akkadian-1.0.9/akkadian/full_translation_build_data.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/get_texts_details.py` & `akkadian-1.0.9/akkadian/get_texts_details.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/hmm.py` & `akkadian-1.0.9/akkadian/hmm.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/memm.py` & `akkadian-1.0.9/akkadian/memm.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/parse_json.py` & `akkadian-1.0.9/akkadian/parse_json.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/parse_xml.py` & `akkadian-1.0.9/akkadian/parse_xml.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/train.py` & `akkadian-1.0.9/akkadian/train.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -86,18 +86,18 @@
     """
     Trains biLSTM, MEMM and HMM models, stores all data and print the accuracies
     :return: nothing, stores everything in pickles
     """
 
     corpora = ['rinap/rinap1', 'rinap/rinap3', 'rinap/rinap4', 'rinap/rinap5']
 
-    #print('##### MEMM #####')
-    #memm_train_and_test(corpora)
-
     #print('##### HMM #####')
     #hmm_train_and_test(corpora)
 
+    #print('##### MEMM #####')
+    #memm_train_and_test(corpora)
+
     print('##### BiLSTM #####')
     biLSTM_train_and_test(corpora)
 
 if __name__ == '__main__':
     main()
```

### Comparing `akkadian-1.0.8/akkadian/translation_tokenize.py` & `akkadian-1.0.9/akkadian/translation_tokenize.py`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/akkadian/transliterate.py` & `akkadian-1.0.9/akkadian/transliterate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from akkadian.data import logits_to_trans, load_object_from_file
 from akkadian.combine_algorithms import overall_classifier, list_to_tran, sentence_to_allen_format, sentence_to_HMM_format
 from akkadian.hmm import hmm_viterbi
 from akkadian.memm import memm_greedy
 from akkadian.__init__ import hmm_path, memm_path, bilstm_path
 
 
+def sanitize(sentence):
+    out_sentence = ""
+    for sign in sentence:
+        if 0x12000 <= ord(sign) or ord(sign) == 'x':
+            out_sentence += sign
+
+    return out_sentence
+
+
 def transliterate(sentence):
     """
     Transliterate signs using best transliteration algorithm so far
     :param sentence: signs to be transliterated
     :return: transliteration of the sentence
     """
     return transliterate_bilstm(sentence)
@@ -16,54 +25,62 @@
 
 def transliterate_bilstm(sentence):
     """
     Transliterate signs using biLSTM
     :param sentence: signs to be transliterated
     :return: transliteration of the sentence
     """
+    sentence = sanitize(sentence)
+
     model, predictor, sign_to_id, id_to_tran, test_texts = load_object_from_file(bilstm_path)
 
     tag_logits = predictor.predict(sentence_to_allen_format(sentence, sign_to_id, True))['tag_logits']
     biLSTM_predicted_tags, _, _, _, _, _ = logits_to_trans(tag_logits, model, id_to_tran)
     return list_to_tran(biLSTM_predicted_tags)
 
 
 def transliterate_bilstm_top3(sentence):
     """
     Transliterate signs using biLSTM
     :param sentence: signs to be transliterated
     :return: 3 top transliterations of the sentence with their scores
     """
+    sentence = sanitize(sentence)
+
     model, predictor, sign_to_id, id_to_tran, test_texts = load_object_from_file(bilstm_path)
 
     tag_logits = predictor.predict(sentence_to_allen_format(sentence, sign_to_id, True))['tag_logits']
     prediction1, prediction2, prediction3, score1, score2, score3 = logits_to_trans(tag_logits, model, id_to_tran)
     return list_to_tran(prediction1), list_to_tran(prediction2), list_to_tran(prediction3)
 
 
 def transliterate_hmm(sentence):
     """
     Transliterate signs using HMM
     :param sentence: signs to be transliterated
     :return: transliteration of the sentence
     """
+    sentence = sanitize(sentence)
+
     most_common_tag, possible_tags, q, e, S, total_tokens, q_bi_counts, q_uni_counts, lambda1, lambda2, test_texts = \
         load_object_from_file(hmm_path)
 
     HMM_predicted_tags = hmm_viterbi(sentence_to_HMM_format(sentence), total_tokens, q_bi_counts, q_uni_counts, q, e,
                            S, most_common_tag, possible_tags, lambda1, lambda2)
     return list_to_tran(HMM_predicted_tags)
 
 
 def transliterate_memm(sentence):
     """
     Transliterate signs using MEMM
     :param sentence: signs to be transliterated
     :return: transliteration of the sentence
     """
+    sentence = sanitize(sentence)
+
     logreg, vec, idx_to_tag_dict, test_texts = load_object_from_file(memm_path)
 
     MEMM_predicted_tags = memm_greedy(sentence_to_HMM_format(sentence), logreg, vec, idx_to_tag_dict)
 
     return list_to_tran(MEMM_predicted_tags)
 
 
@@ -123,15 +140,15 @@
 
  	
 𒊮𒁉 𒌒𒇴𒈠 𒋞𒄭𒀀
 
  	
 𒂍𒊕𒅍 𒅇 𒂍𒍣𒁕
 
-10	
+10
 𒀸 𒆳𒄩𒀜𒁴 𒀸 𒋗𒈫𒐊 𒂖𒇷𒋾
 
  	
 𒄿𒈾 𒉌𒄑 𒊒𒍑𒋾 𒀠𒁉𒅔𒈠
 
  	
 𒀀𒈾 𒈾𒁲𒂊 𒍑𒋗 𒊭 𒂍𒊕𒅍
@@ -273,12 +290,13 @@
 
  	
 𒁕𒈪𒅅𒋾𒋙𒉡
 
  	
 𒇷𒅖𒃻𒆥 𒄿𒈾 𒉿𒄿𒅗
 """
-    #print(transliterate(example))
-    #print(transliterate_bilstm(example))
-    #print(transliterate_bilstm_top3(example))
+    print(transliterate(example))
+    print(transliterate_bilstm(example))
+    print(transliterate_bilstm_top3(example))
     print(transliterate_hmm(example))
-    #print(transliterate_memm(example))
+    print(transliterate_memm(example))
+    #main()
```

### Comparing `akkadian-1.0.8/akkadian.egg-info/PKG-INFO` & `akkadian-1.0.9/akkadian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akkadian
-Version: 1.0.8
+Version: 1.0.9
 Summary: Translating Akkadian signs to transliteration using NLP algorithms
 Home-page: https://github.com/gaigutherz/Translating-Akkadian-using-NLP
 Author: Ariel Elazary, Gai Gutherz
 Author-email: am.elazary@gmail.com, gaigutherz@gmail.com
 License: UNKNOWN
 Description: # Akkademia
         Akkademia is a tool for automatically transliterating Unicode cuneiform glyphs. It is written in python script and uses HMM, MEMM and BiLSTM neural networks to determine appropriate sign-readings and segmentation.
```

### Comparing `akkadian-1.0.8/akkadian.egg-info/SOURCES.txt` & `akkadian-1.0.9/akkadian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akkadian-1.0.8/setup.py` & `akkadian-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(file="README.md", mode="r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="akkadian",
-    version="1.0.8",
+    version="1.0.9",
     author="Ariel Elazary, Gai Gutherz",
     author_email="am.elazary@gmail.com, gaigutherz@gmail.com",
     description="Translating Akkadian signs to transliteration using NLP algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaigutherz/Translating-Akkadian-using-NLP",
     packages=setuptools.find_packages(),
```

