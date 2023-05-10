# Comparing `tmp/langkit-0.0.1.dev0.tar.gz` & `tmp/langkit-0.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.1.dev0.tar", max compression
+gzip compressed data, was "langkit-0.0.1.dev1.tar", max compression
```

## Comparing `langkit-0.0.1.dev0.tar` & `langkit-0.0.1.dev1.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1.dev0/LICENSE
--rw-r--r--   0        0        0       65 2023-05-08 19:26:42.352898 langkit-0.0.1.dev0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 19:51:56.468542 langkit-0.0.1.dev0/langkit/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 16:31:57.882898 langkit-0.0.1.dev0/langkit/exclusions.py
--rw-r--r--   0        0        0     1203 2023-05-08 19:29:19.602898 langkit-0.0.1.dev0/langkit/input_output.py
--rw-r--r--   0        0        0      428 2023-04-28 02:33:55.065900 langkit-0.0.1.dev0/langkit/sentiment.py
--rw-r--r--   0        0        0     2394 2023-05-08 18:55:12.642898 langkit-0.0.1.dev0/langkit/textstat.py
--rw-r--r--   0        0        0      473 2023-05-08 19:04:44.352898 langkit-0.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 langkit-0.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.1.dev1/LICENSE
+-rw-r--r--   0        0        0     2001 2023-05-10 18:06:28.152898 langkit-0.0.1.dev1/README.md
+-rw-r--r--   0        0        0      244 2023-05-09 22:21:18.502898 langkit-0.0.1.dev1/langkit/__init__.py
+-rw-r--r--   0        0        0   267008 2023-05-10 18:29:55.652898 langkit-0.0.1.dev1/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0     1680 2023-05-10 18:06:28.152898 langkit-0.0.1.dev1/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0        0 2023-05-08 16:31:57.882898 langkit-0.0.1.dev1/langkit/exclusions.py
+-rw-r--r--   0        0        0     1097 2023-05-09 23:30:20.252898 langkit-0.0.1.dev1/langkit/input_output.py
+-rw-r--r--   0        0        0     1051 2023-05-10 18:06:37.882898 langkit-0.0.1.dev1/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2403 2023-05-10 18:06:37.882898 langkit-0.0.1.dev1/langkit/regexes.py
+-rw-r--r--   0        0        0      488 2023-05-09 23:30:20.252898 langkit-0.0.1.dev1/langkit/sentiment.py
+-rw-r--r--   0        0        0     2072 2023-05-10 18:06:37.882898 langkit-0.0.1.dev1/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     2404 2023-05-09 23:30:20.252898 langkit-0.0.1.dev1/langkit/textstat.py
+-rw-r--r--   0        0        0      605 2023-05-10 18:19:07.442898 langkit-0.0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 langkit-0.0.1.dev1/PKG-INFO
```

### Comparing `langkit-0.0.1.dev0/LICENSE` & `langkit-0.0.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.1.dev0/langkit/input_output.py` & `langkit-0.0.1.dev1/langkit/input_output.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Tuple
+from typing import Optional, Tuple
 from sentence_transformers import SentenceTransformer, util
 from torch import Tensor
-from whylogs.core.datatypes import String
 from whylogs.experimental.core.metrics.udf_metric import (
     register_metric_udf,
 )
-from typing import Callable
-from whylogs.core.datatypes import DataType
-from whylogs.experimental.core.metrics.udf_metric import (
-    _col_type_submetrics
-)
 
-_example_model = SentenceTransformer('sentence-transformers/all-MiniLM-L6-v2')
+_transformer_model = None
+
+
+def init(transformer_name: Optional[str]):
+    global _transformer_model
+    if transformer_name is None:
+        transformer_name = 'sentence-transformers/all-MiniLM-L6-v2'
+    _transformer_model = SentenceTransformer(transformer_name)
 
 
-def register_udf(name: str, func: Callable, col_type: DataType):
-    _col_type_submetrics[col_type].append((name, func))
+init()
 
 
 def get_subject_similarity(text: str, comparison_embedding: Tensor) -> float:
-    embedding = _example_model.encode(text, convert_to_tensor=True)
+    embedding = _transformer_model.encode(text, convert_to_tensor=True)
     similarity = util.pytorch_cos_sim(embedding, comparison_embedding)
     return similarity.item()
 
 
 @register_metric_udf(col_name="combined")
 def similarity_MiniLM_L6_v2(combined: Tuple[str, str]) -> float:
     x, y = combined
-    embedding_1 = _example_model.encode(x, convert_to_tensor=True)
-    embedding_2 = _example_model.encode(y, convert_to_tensor=True)
+    embedding_1 = _transformer_model.encode(x, convert_to_tensor=True)
+    embedding_2 = _transformer_model.encode(y, convert_to_tensor=True)
     similarity = util.pytorch_cos_sim(embedding_1, embedding_2)
     return similarity.item()
```

### Comparing `langkit-0.0.1.dev0/langkit/textstat.py` & `langkit-0.0.1.dev1/langkit/textstat.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     return textstat.textstat.linsear_write_formula(text)
 
 @register_metric_udf(col_type=String)
 def gunning_fog(text: str) -> float:
     return textstat.textstat.gunning_fog(text)
 
 @register_metric_udf(col_type=String)
-def text_standard(text: str) -> float:
+def aggregate_reading_level(text: str) -> float:
     return textstat.textstat.text_standard(text)
 
 @register_metric_udf(col_type=String)
 def fernandez_huerta(text: str) -> float:
     return textstat.textstat.fernandez_huerta(text)
 
 @register_metric_udf(col_type=String)
```

