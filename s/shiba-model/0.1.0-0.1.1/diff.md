# Comparing `tmp/shiba-model-0.1.0.tar.gz` & `tmp/shiba-model-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiba-model-0.1.0.tar", last modified: Fri Jun 25 00:30:38 2021, max compression
+gzip compressed data, was "shiba-model-0.1.1.tar", last modified: Wed May 10 07:47:44 2023, max compression
```

## Comparing `shiba-model-0.1.0.tar` & `shiba-model-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2021-06-25 00:30:38.608582 shiba-model-0.1.0/
--rw-rw-r--   0 josh      (1000) josh      (1000)    10480 2021-06-24 11:00:47.000000 shiba-model-0.1.0/LICENSE.md
--rw-rw-r--   0 josh      (1000) josh      (1000)     9163 2021-06-25 00:30:38.608582 shiba-model-0.1.0/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)     8575 2021-06-24 11:25:48.000000 shiba-model-0.1.0/README.md
--rw-rw-r--   0 josh      (1000) josh      (1000)      103 2021-06-24 11:00:47.000000 shiba-model-0.1.0/pyproject.toml
--rw-rw-r--   0 josh      (1000) josh      (1000)       38 2021-06-25 00:30:38.608582 shiba-model-0.1.0/setup.cfg
--rw-rw-r--   0 josh      (1000) josh      (1000)      912 2021-06-24 11:00:47.000000 shiba-model-0.1.0/setup.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2021-06-25 00:30:38.608582 shiba-model-0.1.0/shiba/
--rw-rw-r--   0 josh      (1000) josh      (1000)      210 2021-06-24 11:00:47.000000 shiba-model-0.1.0/shiba/__init__.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2008 2021-06-24 11:00:47.000000 shiba-model-0.1.0/shiba/codepoint_tokenizer.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     3486 2021-06-24 11:00:47.000000 shiba-model-0.1.0/shiba/local_self_attention.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     2768 2021-06-24 11:00:47.000000 shiba-model-0.1.0/shiba/local_transformer_encoder_layer.py
--rw-rw-r--   0 josh      (1000) josh      (1000)    22263 2021-06-24 11:00:47.000000 shiba-model-0.1.0/shiba/model.py
--rw-rw-r--   0 josh      (1000) josh      (1000)     1446 2021-06-24 11:00:47.000000 shiba-model-0.1.0/shiba/multi_hashing_embedder.py
--rw-rw-r--   0 josh      (1000) josh      (1000)      628 2021-06-24 11:00:47.000000 shiba-model-0.1.0/shiba/position_embedder.py
-drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2021-06-25 00:30:38.608582 shiba-model-0.1.0/shiba_model.egg-info/
--rw-rw-r--   0 josh      (1000) josh      (1000)     9163 2021-06-25 00:30:38.000000 shiba-model-0.1.0/shiba_model.egg-info/PKG-INFO
--rw-rw-r--   0 josh      (1000) josh      (1000)      410 2021-06-25 00:30:38.000000 shiba-model-0.1.0/shiba_model.egg-info/SOURCES.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        1 2021-06-25 00:30:38.000000 shiba-model-0.1.0/shiba_model.egg-info/dependency_links.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)       29 2021-06-25 00:30:38.000000 shiba-model-0.1.0/shiba_model.egg-info/requires.txt
--rw-rw-r--   0 josh      (1000) josh      (1000)        6 2021-06-25 00:30:38.000000 shiba-model-0.1.0/shiba_model.egg-info/top_level.txt
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-10 07:47:44.647017 shiba-model-0.1.1/
+-rw-r--r--   0 josh       (501) staff       (20)    10480 2023-03-18 22:41:21.000000 shiba-model-0.1.1/LICENSE.md
+-rw-r--r--   0 josh       (501) staff       (20)     9079 2023-05-10 07:47:44.646671 shiba-model-0.1.1/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     8528 2023-05-10 07:41:56.000000 shiba-model-0.1.1/README.md
+-rw-r--r--   0 josh       (501) staff       (20)      103 2023-03-18 22:41:21.000000 shiba-model-0.1.1/pyproject.toml
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-05-10 07:47:44.647083 shiba-model-0.1.1/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      912 2023-05-10 07:46:20.000000 shiba-model-0.1.1/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-10 07:47:44.644246 shiba-model-0.1.1/shiba/
+-rw-r--r--   0 josh       (501) staff       (20)      208 2023-05-10 07:29:25.000000 shiba-model-0.1.1/shiba/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     2008 2023-03-18 22:41:21.000000 shiba-model-0.1.1/shiba/codepoint_tokenizer.py
+-rw-r--r--   0 josh       (501) staff       (20)     3486 2023-03-18 22:41:21.000000 shiba-model-0.1.1/shiba/local_self_attention.py
+-rw-r--r--   0 josh       (501) staff       (20)     2768 2023-03-18 22:41:21.000000 shiba-model-0.1.1/shiba/local_transformer_encoder_layer.py
+-rw-r--r--   0 josh       (501) staff       (20)    23461 2023-05-10 07:39:17.000000 shiba-model-0.1.1/shiba/model.py
+-rw-r--r--   0 josh       (501) staff       (20)     1446 2023-03-18 22:41:21.000000 shiba-model-0.1.1/shiba/multi_hashing_embedder.py
+-rw-r--r--   0 josh       (501) staff       (20)      628 2023-03-18 22:41:21.000000 shiba-model-0.1.1/shiba/position_embedder.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-10 07:47:44.646080 shiba-model-0.1.1/shiba_model.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     9079 2023-05-10 07:47:44.000000 shiba-model-0.1.1/shiba_model.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      410 2023-05-10 07:47:44.000000 shiba-model-0.1.1/shiba_model.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-05-10 07:47:44.000000 shiba-model-0.1.1/shiba_model.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)       29 2023-05-10 07:47:44.000000 shiba-model-0.1.1/shiba_model.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)        6 2023-05-10 07:47:44.000000 shiba-model-0.1.1/shiba_model.egg-info/top_level.txt
```

### Comparing `shiba-model-0.1.0/LICENSE.md` & `shiba-model-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shiba-model-0.1.0/PKG-INFO` & `shiba-model-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: shiba-model
-Version: 0.1.0
+Version: 0.1.1
 Summary: An efficient character-level transformer encoder, pretrained for Japanese
 Home-page: https://github.com/octanove/shiba
 Author: Octanove Labs
 Author-email: mindful.jt@gmail.com
-License: UNKNOWN
 Keywords: natural language processing,deep learning,transformer
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -51,20 +49,21 @@
 
 ## How do I use it?
 
 If you just want to use the SHIBA model, you can install it like this:
 > pip install shiba-model
 
 
-For an example of how to load and use the pretrained model, see below. `get_pretrained_state_dict()` will automatically download the pretrained model for you, but if you'd like to do it yourself the model can be downloaded from [here](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt).
+For an example of how to load and use the pretrained model, see below. `get_pretrained_from_hub()` will automatically download the pretrained model for you, but if you'd like to do it yourself the model can be downloaded from [here](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt).
 
 ```python
-from shiba import Shiba, CodepointTokenizer, get_pretrained_state_dict
+from shiba import Shiba, CodepointTokenizer, get_pretrained_from_hub
 shiba_model = Shiba()
-shiba_model.load_state_dict(get_pretrained_state_dict())
+shiba_model.load_state_dict(get_pretrained_from_hub())
+shiba_model.eval() # disable dropout
 tokenizer = CodepointTokenizer()
 
 inputs = tokenizer.encode_batch(['自然言語処理', '柴ドリル'])
 outputs = shiba_model(**inputs)
 ```
 
 SHIBA can then be fine-tuned for classification or character-level tasks just like any other transformer encoder. Adding task-specific layers should be relatively easy, but premade models for classification and sequence labeling are also included. These are `ShibaForClassification` and `ShibaForSequenceLabeling`, respectively. 
@@ -112,22 +111,22 @@
 
 ## Training Code
 
 This repository also includes the code used for actually training the SHIBA model (which is not in the `shiba-model` package). This code has significantly more dependencies than just the model and is not as polished, but if you are considering training a SHIBA/CANINE model it may be of interest to you. In particular, there are implementations of BPE masking and random span masking in the [masking.py](training/masking.py) file. 
 
 ## Checkpoints
 
-The default model is the encoder model that performs best on downstream tasks, but we provide a few other checkpoints. 
+The default model is the encoder model that performs best on downstream tasks, but we provide a few other checkpoints.
 
-| Type              | Step | Note            |
-|-------------------|------|-----------------|
-| [Encoder Only](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt)      | 45k  | (default model) |
-| [Encoder Only](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check60k.pt)     | 60k  |                 |
-| [LM Head + Encoder](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/lm_check45k.pt) | 45k  |                 |
-| [LM Head + Encoder](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/lm_check60k.pt) | 60k  |                 |
+| Type                                                              | Step | Note            |
+|-------------------------------------------------------------------|------|-----------------|
+| [Encoder Only](https://huggingface.co/octanove/shiba-enc-45k)     | 45k  | (default model) |
+| [Encoder Only](https://huggingface.co/octanove/shiba-enc-60k)     | 60k  |                 |
+| [LM Head + Encoder](https://huggingface.co/octanove/shiba-lm-45k) | 45k  |                 |
+| [LM Head + Encoder](https://huggingface.co/octanove/shiba-lm-60k) | 60k  |                 |
 
 # Licensing
 
 The code and contents of this repository are provided under the Apache License 2.0. The pretrained model weights are provided under the CC BY-SA 4.0 license. 
 
 # How to cite this work
 
@@ -164,9 +163,7 @@
 <a id="3">[3]</a>
 Peter Izsak and Moshe Berchansky and Omer Levy (2021). [How to Train BERT with an Academic Budget](https://arxiv.org/abs/2104.07705). CoRR, abs/2104.07705.
 
 
 
 
 
-
-
```

### Comparing `shiba-model-0.1.0/README.md` & `shiba-model-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,20 +34,21 @@
 
 ## How do I use it?
 
 If you just want to use the SHIBA model, you can install it like this:
 > pip install shiba-model
 
 
-For an example of how to load and use the pretrained model, see below. `get_pretrained_state_dict()` will automatically download the pretrained model for you, but if you'd like to do it yourself the model can be downloaded from [here](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt).
+For an example of how to load and use the pretrained model, see below. `get_pretrained_from_hub()` will automatically download the pretrained model for you, but if you'd like to do it yourself the model can be downloaded from [here](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt).
 
 ```python
-from shiba import Shiba, CodepointTokenizer, get_pretrained_state_dict
+from shiba import Shiba, CodepointTokenizer, get_pretrained_from_hub
 shiba_model = Shiba()
-shiba_model.load_state_dict(get_pretrained_state_dict())
+shiba_model.load_state_dict(get_pretrained_from_hub())
+shiba_model.eval() # disable dropout
 tokenizer = CodepointTokenizer()
 
 inputs = tokenizer.encode_batch(['自然言語処理', '柴ドリル'])
 outputs = shiba_model(**inputs)
 ```
 
 SHIBA can then be fine-tuned for classification or character-level tasks just like any other transformer encoder. Adding task-specific layers should be relatively easy, but premade models for classification and sequence labeling are also included. These are `ShibaForClassification` and `ShibaForSequenceLabeling`, respectively. 
@@ -95,22 +96,22 @@
 
 ## Training Code
 
 This repository also includes the code used for actually training the SHIBA model (which is not in the `shiba-model` package). This code has significantly more dependencies than just the model and is not as polished, but if you are considering training a SHIBA/CANINE model it may be of interest to you. In particular, there are implementations of BPE masking and random span masking in the [masking.py](training/masking.py) file. 
 
 ## Checkpoints
 
-The default model is the encoder model that performs best on downstream tasks, but we provide a few other checkpoints. 
+The default model is the encoder model that performs best on downstream tasks, but we provide a few other checkpoints.
 
-| Type              | Step | Note            |
-|-------------------|------|-----------------|
-| [Encoder Only](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt)      | 45k  | (default model) |
-| [Encoder Only](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check60k.pt)     | 60k  |                 |
-| [LM Head + Encoder](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/lm_check45k.pt) | 45k  |                 |
-| [LM Head + Encoder](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/lm_check60k.pt) | 60k  |                 |
+| Type                                                              | Step | Note            |
+|-------------------------------------------------------------------|------|-----------------|
+| [Encoder Only](https://huggingface.co/octanove/shiba-enc-45k)     | 45k  | (default model) |
+| [Encoder Only](https://huggingface.co/octanove/shiba-enc-60k)     | 60k  |                 |
+| [LM Head + Encoder](https://huggingface.co/octanove/shiba-lm-45k) | 45k  |                 |
+| [LM Head + Encoder](https://huggingface.co/octanove/shiba-lm-60k) | 60k  |                 |
 
 # Licensing
 
 The code and contents of this repository are provided under the Apache License 2.0. The pretrained model weights are provided under the CC BY-SA 4.0 license. 
 
 # How to cite this work
```

### Comparing `shiba-model-0.1.0/setup.py` & `shiba-model-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="shiba-model",
-    version="0.1.0",
+    version="0.1.1",
     author="Octanove Labs",
     author_email="mindful.jt@gmail.com",
     description="An efficient character-level transformer encoder, pretrained for Japanese",
     keywords=['natural language processing', 'deep learning', 'transformer'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/octanove/shiba",
```

### Comparing `shiba-model-0.1.0/shiba/codepoint_tokenizer.py` & `shiba-model-0.1.1/shiba/codepoint_tokenizer.py`

 * *Files identical despite different names*

### Comparing `shiba-model-0.1.0/shiba/local_self_attention.py` & `shiba-model-0.1.1/shiba/local_self_attention.py`

 * *Files identical despite different names*

### Comparing `shiba-model-0.1.0/shiba/local_transformer_encoder_layer.py` & `shiba-model-0.1.1/shiba/local_transformer_encoder_layer.py`

 * *Files identical despite different names*

### Comparing `shiba-model-0.1.0/shiba/model.py` & `shiba-model-0.1.1/shiba/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import urllib
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Dict, Optional, Tuple
 
 import torch
+from huggingface_hub import hf_hub_url
 
 from shiba.codepoint_tokenizer import CodepointTokenizer
 from shiba.local_transformer_encoder_layer import LocalTransformerEncoderLayer
 from shiba.multi_hashing_embedder import MultiHashingEmbedder
 
 from shiba.position_embedder import PositionEmbedder
 
@@ -247,14 +248,16 @@
         lhs_padding = math.floor(total_padding / 2)
         rhs_padding = math.ceil(total_padding / 2)
 
         return torch.nn.functional.pad(hidden_state, (0, 0, lhs_padding, rhs_padding))
 
 
 def get_pretrained_state_dict():
+    """DEPRECATED: This gets the state dict from Google's cloud storage, and we may eventually delete those files.
+    Safer to get models from the hub."""
     download_url = 'https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt'
     save_location = Path.home() / '.shiba' / 'pretrained_shiba.pt'
 
     if not save_location.parent.exists():
         os.makedirs(save_location.parent, exist_ok=True)
 
     if not save_location.exists():
@@ -264,22 +267,47 @@
             data = response.read()
             state_dict_file.write(data)
         print('Done')
 
     return torch.load(save_location, map_location=torch.device('cpu'))
 
 
+def get_pretrained_from_hub(repo: Optional[str] = None):
+    if repo is None:
+        repo = 'octanove/shiba-enc-45k'
+
+    if not repo.startswith('octanove') or 'shiba' not in repo:
+        raise ValueError('Repo name should look like octanove/shiba-*')
+
+    download_url = hf_hub_url(repo_id=repo, filename='model.pt')
+    local_model_name = repo.split('/')[1] + '.pt'
+    save_location = Path.home() / '.shiba' / local_model_name
+
+    if not save_location.parent.exists():
+        os.makedirs(save_location.parent, exist_ok=True)
+
+    if not save_location.exists():
+        print(f'Downloading {repo}: {download_url} -> {save_location}')
+        with open(save_location, 'wb') as state_dict_file:
+            response = urllib.request.urlopen(download_url)
+            data = response.read()
+            state_dict_file.write(data)
+        print('Done')
+
+    return torch.load(save_location, map_location=torch.device('cpu'))
+
+
 class ShibaForTask(torch.nn.Module):
     def __init__(self, **kwargs):
         super(ShibaForTask, self).__init__()
         self.shiba_model = Shiba(**kwargs)
 
     def load_encoder_checkpoint(self, checkpoint_location: Optional[str] = None):
-        if checkpoint_location is None:
-            state_dict = get_pretrained_state_dict()
+        if checkpoint_location is None or checkpoint_location.startswith('octanove/shiba-enc'):
+            state_dict = get_pretrained_from_hub(checkpoint_location)
         else:
             state_dict = torch.load(checkpoint_location, map_location=torch.device('cpu'))
 
         self.shiba_model.load_state_dict(state_dict)
 
 
 class ShibaForSequenceLabeling(ShibaForTask):
```

### Comparing `shiba-model-0.1.0/shiba/multi_hashing_embedder.py` & `shiba-model-0.1.1/shiba/multi_hashing_embedder.py`

 * *Files identical despite different names*

### Comparing `shiba-model-0.1.0/shiba/position_embedder.py` & `shiba-model-0.1.1/shiba/position_embedder.py`

 * *Files identical despite different names*

### Comparing `shiba-model-0.1.0/shiba_model.egg-info/PKG-INFO` & `shiba-model-0.1.1/shiba_model.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: shiba-model
-Version: 0.1.0
+Version: 0.1.1
 Summary: An efficient character-level transformer encoder, pretrained for Japanese
 Home-page: https://github.com/octanove/shiba
 Author: Octanove Labs
 Author-email: mindful.jt@gmail.com
-License: UNKNOWN
 Keywords: natural language processing,deep learning,transformer
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -51,20 +49,21 @@
 
 ## How do I use it?
 
 If you just want to use the SHIBA model, you can install it like this:
 > pip install shiba-model
 
 
-For an example of how to load and use the pretrained model, see below. `get_pretrained_state_dict()` will automatically download the pretrained model for you, but if you'd like to do it yourself the model can be downloaded from [here](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt).
+For an example of how to load and use the pretrained model, see below. `get_pretrained_from_hub()` will automatically download the pretrained model for you, but if you'd like to do it yourself the model can be downloaded from [here](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt).
 
 ```python
-from shiba import Shiba, CodepointTokenizer, get_pretrained_state_dict
+from shiba import Shiba, CodepointTokenizer, get_pretrained_from_hub
 shiba_model = Shiba()
-shiba_model.load_state_dict(get_pretrained_state_dict())
+shiba_model.load_state_dict(get_pretrained_from_hub())
+shiba_model.eval() # disable dropout
 tokenizer = CodepointTokenizer()
 
 inputs = tokenizer.encode_batch(['自然言語処理', '柴ドリル'])
 outputs = shiba_model(**inputs)
 ```
 
 SHIBA can then be fine-tuned for classification or character-level tasks just like any other transformer encoder. Adding task-specific layers should be relatively easy, but premade models for classification and sequence labeling are also included. These are `ShibaForClassification` and `ShibaForSequenceLabeling`, respectively. 
@@ -112,22 +111,22 @@
 
 ## Training Code
 
 This repository also includes the code used for actually training the SHIBA model (which is not in the `shiba-model` package). This code has significantly more dependencies than just the model and is not as polished, but if you are considering training a SHIBA/CANINE model it may be of interest to you. In particular, there are implementations of BPE masking and random span masking in the [masking.py](training/masking.py) file. 
 
 ## Checkpoints
 
-The default model is the encoder model that performs best on downstream tasks, but we provide a few other checkpoints. 
+The default model is the encoder model that performs best on downstream tasks, but we provide a few other checkpoints.
 
-| Type              | Step | Note            |
-|-------------------|------|-----------------|
-| [Encoder Only](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check45k.pt)      | 45k  | (default model) |
-| [Encoder Only](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/shiba_check60k.pt)     | 60k  |                 |
-| [LM Head + Encoder](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/lm_check45k.pt) | 45k  |                 |
-| [LM Head + Encoder](https://storage.googleapis.com/shiba.octanove.com/published_checkpoints/lm_check60k.pt) | 60k  |                 |
+| Type                                                              | Step | Note            |
+|-------------------------------------------------------------------|------|-----------------|
+| [Encoder Only](https://huggingface.co/octanove/shiba-enc-45k)     | 45k  | (default model) |
+| [Encoder Only](https://huggingface.co/octanove/shiba-enc-60k)     | 60k  |                 |
+| [LM Head + Encoder](https://huggingface.co/octanove/shiba-lm-45k) | 45k  |                 |
+| [LM Head + Encoder](https://huggingface.co/octanove/shiba-lm-60k) | 60k  |                 |
 
 # Licensing
 
 The code and contents of this repository are provided under the Apache License 2.0. The pretrained model weights are provided under the CC BY-SA 4.0 license. 
 
 # How to cite this work
 
@@ -164,9 +163,7 @@
 <a id="3">[3]</a>
 Peter Izsak and Moshe Berchansky and Omer Levy (2021). [How to Train BERT with an Academic Budget](https://arxiv.org/abs/2104.07705). CoRR, abs/2104.07705.
 
 
 
 
 
-
-
```

