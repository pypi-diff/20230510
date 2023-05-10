# Comparing `tmp/open_gpt_torch-0.0.1rc6.tar.gz` & `tmp/open_gpt_torch-0.0.1rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gpt_torch-0.0.1rc6.tar", max compression
+gzip compressed data, was "open_gpt_torch-0.0.1rc7.tar", max compression
```

## Comparing `open_gpt_torch-0.0.1rc6.tar` & `open_gpt_torch-0.0.1rc7.tar`

### file list

```diff
@@ -1,43 +1,46 @@
--rw-r--r--   0        0        0    10825 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/LICENSE
--rw-r--r--   0        0        0     7531 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/README.md
--rw-r--r--   0        0        0      853 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/__init__.py
--rw-r--r--   0        0        0      107 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/__main__.py
--rw-r--r--   0        0        0      474 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/adapter.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/__init__.py
--rw-r--r--   0        0        0     1039 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/application.py
--rw-r--r--   0        0        0      508 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/command_loader.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/__init__.py
--rw-r--r--   0        0        0      567 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/about.py
--rw-r--r--   0        0        0     1232 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/serve.py
--rw-r--r--   0        0        0     1898 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/factory.py
--rw-r--r--   0        0        0     1767 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/helper.py
--rw-r--r--   0        0        0      349 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/hub.py
--rw-r--r--   0        0        0      498 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/logging.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/__init__.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0        0        0     5274 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0        0        0     5658 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/loading.py
--rw-r--r--   0        0        0     8561 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flan/__init__.py
--rw-r--r--   0        0        0     1074 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/flan/loading.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/llama/__init__.py
--rw-r--r--   0        0        0      846 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/llama/loading.py
--rw-r--r--   0        0        0     4469 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/loading.py
--rw-r--r--   0        0        0     2623 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/modeling.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/moss/__init__.py
--rw-r--r--   0        0        0     1860 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/moss/loading.py
--rw-r--r--   0        0        0      947 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/moss/modeling.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/pythia/__init__.py
--rw-r--r--   0        0        0     2157 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/pythia/loading.py
--rw-r--r--   0        0        0      669 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/pythia/modeling.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0        0        0      852 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/stablelm/loading.py
--rw-r--r--   0        0        0     1619 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/models/stablelm/modeling.py
--rw-r--r--   0        0        0     2862 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/profile.py
--rw-r--r--   0        0        0        0 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/__init__.py
--rw-r--r--   0        0        0       36 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/executors/__init__.py
--rw-r--r--   0        0        0     1742 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/executors/base.py
--rw-r--r--   0        0        0      437 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/flow.py
--rw-r--r--   0        0        0      931 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/open_gpt/serve/gateway.py
--rw-r--r--   0        0        0     2263 2023-05-08 08:16:29.735031 open_gpt_torch-0.0.1rc6/pyproject.toml
--rw-r--r--   0        0        0    19871 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc6/PKG-INFO
+-rw-r--r--   0        0        0    10825 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/LICENSE
+-rw-r--r--   0        0        0     7531 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/README.md
+-rw-r--r--   0        0        0      853 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/__main__.py
+-rw-r--r--   0        0        0      474 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/adapter.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/__init__.py
+-rw-r--r--   0        0        0     1039 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/application.py
+-rw-r--r--   0        0        0      508 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/command_loader.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0        0        0      567 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/about.py
+-rw-r--r--   0        0        0     1232 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/serve.py
+-rw-r--r--   0        0        0     2977 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/factory.py
+-rw-r--r--   0        0        0     2509 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/helper.py
+-rw-r--r--   0        0        0      349 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/hub.py
+-rw-r--r--   0        0        0      498 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/logging.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0        0        0     5774 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0        0        0     8574 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0        0        0     5309 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0        0        0     2403 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flan/__init__.py
+-rw-r--r--   0        0        0     1074 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/flan/loading.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/llama/__init__.py
+-rw-r--r--   0        0        0     1407 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/llama/modeling.py
+-rw-r--r--   0        0        0     4952 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/loading.py
+-rw-r--r--   0        0        0     2737 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/moss/__init__.py
+-rw-r--r--   0        0        0      234 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/moss/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0        0        0     2157 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/pythia/loading.py
+-rw-r--r--   0        0        0      239 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/pythia/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0        0        0      907 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/stablelm/modeling.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0        0        0     3372 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0        0        0      771 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0        0        0     2862 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/profile.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0        0        0     1742 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/executors/base.py
+-rw-r--r--   0        0        0        0 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0        0        0      608 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/flow.py
+-rw-r--r--   0        0        0      931 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/open_gpt/serve/gateway.py
+-rw-r--r--   0        0        0     2279 2023-05-10 02:11:18.588579 open_gpt_torch-0.0.1rc7/pyproject.toml
+-rw-r--r--   0        0        0    19904 1970-01-01 00:00:00.000000 open_gpt_torch-0.0.1rc7/PKG-INFO
```

### Comparing `open_gpt_torch-0.0.1rc6/LICENSE` & `open_gpt_torch-0.0.1rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/README.md` & `open_gpt_torch-0.0.1rc7/README.md`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/__init__.py` & `open_gpt_torch-0.0.1rc7/open_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/cli/application.py` & `open_gpt_torch-0.0.1rc7/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/about.py` & `open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/cli/commands/serve.py` & `open_gpt_torch-0.0.1rc7/open_gpt/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/factory.py` & `open_gpt_torch-0.0.1rc7/open_gpt/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,41 @@
 
     :param model_name: The name of the model to create.
     :param precision: The precision to use. Can be one of ``"float16"``, ``"float32"``, ``"float64"``, ``"bfloat16"``, ``"mixed"`` or ``None``.
     :param device: The device to use. Can be one of ``"cpu"``, ``"cuda"``, ``"cuda:X"`` or ``None``.
     :param device_map: The device map to use. Can be one of ``"balanced"``, ``"single"`` or a list of device IDs.
     :param kwargs: Additional keyword arguments to pass to the model.
     """
-    if model_name.startswith('EleutherAI/pythia'):
+
+    if model_name.startswith('facebook/llama') or model_name.startswith(
+        'decapoda-research/llama'
+    ):
+        from .models.llama.modeling import LlamaModel
+
+        return LlamaModel(
+            model_name,
+            device=device,
+            precision=precision,
+            device_map=device_map,
+            **kwargs,
+        )
+    elif model_name.startswith('lmsys/vicuna'):
+        assert not model_name.endswith(
+            'v0'
+        ), 'You are using an outdated model, please use the newer version ``v1.1+``'
+        from .models.vicuna.modeling import VicunaModel
+
+        return VicunaModel(
+            model_name,
+            device=device,
+            precision=precision,
+            device_map=device_map,
+            **kwargs,
+        )
+    elif model_name.startswith('EleutherAI/pythia'):
         from .models.pythia.modeling import PythiaModel
 
         return PythiaModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
@@ -45,14 +71,24 @@
         return MossModel(
             model_name,
             device=device,
             precision=precision,
             device_map=device_map,
             **kwargs,
         )
+    elif model_name.startswith('openflamingo/OpenFlamingo'):
+        from .models.flamingo.modeling import FlamingoModel
+
+        return FlamingoModel(
+            model_name,
+            device=device,
+            precision=precision,
+            device_map=device_map,
+            **kwargs,
+        )
     else:
         from .models.modeling import BaseModel
 
         return BaseModel(
             model_name,
             device=device,
             precision=precision,
```

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/flamingo_lm.py` & `open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,25 +12,34 @@
 class FlamingoLayer(nn.Module):
     def __init__(self, gated_cross_attn_layer, decoder_layer):
         super().__init__()
         self.gated_cross_attn_layer = gated_cross_attn_layer
         self.decoder_layer = decoder_layer
         self.vis_x = None
         self.media_locations = None
+        self.device = self.decoder_layer.parameters().__next__().device
+
+        # This is a hack to gaurantee that the gated_cross_attn_layer is on the same device as the decoder_layer
+        if self.gated_cross_attn_layer is not None:
+            self.gated_cross_attn_layer.to(self.device)
 
     def is_conditioned(self) -> bool:
         """Check whether the layer is conditioned."""
         return self.vis_x is not None
 
     # Used this great idea from this implementation of Flamingo (https://github.com/dhansmair/flamingo-mini/)
     def condition_vis_x(self, vis_x):
-        self.vis_x = vis_x
+        self.vis_x = vis_x.to(self.device) if vis_x is not None else vis_x
 
     def condition_media_locations(self, media_locations):
-        self.media_locations = media_locations
+        self.media_locations = (
+            media_locations.to(self.device)
+            if media_locations is not None
+            else media_locations
+        )
 
     def condition_attend_previous(self, attend_previous):
         self.attend_previous = attend_previous
 
     def forward(
         self,
         lang_x,
@@ -44,14 +53,15 @@
 
         if self.vis_x is None:
             raise ValueError("vis_x must be conditioned before forward pass")
 
         if self.media_locations is None:
             raise ValueError("media_locations must be conditioned before forward pass")
 
+        lang_x = lang_x.to(self.device)
         lang_x = self.gated_cross_attn_layer(
             lang_x,
             self.vis_x,
             media_locations=self.media_locations,
             attend_previous=self.attend_previous,
         )
         lang_x = self.decoder_layer(
@@ -110,15 +120,15 @@
         self.media_token_id = media_token_id
         self.use_media_placement_augmentation = use_media_placement_augmentation
         self.initialized_flamingo = True
 
         dtype, device = auto_dtype_and_device(dtype, device)
         if str(dtype) == 'torch.float16':
             self.gated_cross_attn_layers.half()
-        self.gated_cross_attn_layers.to(device)
+        # self.gated_cross_attn_layers.to(device)
 
     def forward(self, *input, **kwargs):
         """Condition the Flamingo layers on the media locations before forward()"""
 
         if not self.initialized_flamingo:
             raise ValueError(
                 "Flamingo layers are not initialized. Please call `init_flamingo` first."
```

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/loading.py` & `open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 import open_clip
 import torch
-from loguru import logger
 from open_flamingo.src.utils import extend_instance
 
+from open_gpt.logging import logger
+
 
 def load_model_and_transforms(
     model_name_or_path: str,
     vision_model_name_or_path: str,
     lang_model_name_or_path: str,
     tokenizer_name_or_path: Optional[str] = None,
     decoder_layers_attr_name: Optional[str] = None,
     device: 'torch.device' = torch.device('cuda'),
     dtype: 'torch.dtype' = torch.float16,
+    device_map: Optional[Union[str, List[int]]] = None,
+    no_split_module_classes: Optional[List[str]] = None,
     **kwargs,
 ):
     """Load a Flamingo model and its associated image and text processors.
 
     :param model_name_or_path: The name or path of the model to load.
     :param vision_model_name_or_path: The name or path of the vision model to use.
     :param lang_model_name_or_path: The name or path of the language model to use.
     :param tokenizer_name_or_path: The name or path of the tokenizer to use. If not specified, the tokenizer associated with the model will be used.
     :param decoder_layers_attr_name: The name of the attribute that specifies the decoder layers.
     :param device: The device to load the model on.
     :param dtype: The dtype to load the model with.
     """
 
     from ...helper import cast_precision
-    from ..llama.loading import (
-        load_model_and_tokenizer as load_llama_model_and_tokenizer,
-    )
+
+    # from ..llama.loading import (
+    #     load_model_and_tokenizer as load_llama_model_and_tokenizer,
+    # )
+    from ..loading import load_model_and_tokenizer as load_llama_model_and_tokenizer
     from .flamingo_lm import FlamingoLMMixin
-    from .modeling import FlamingoModel
+    from .flamingo_model import FlamingoLMModel
 
     # load the vision model
     precision = cast_precision(dtype)
     model_name, *pretrained = vision_model_name_or_path.split("::")
     pretrained = pretrained[0] if len(pretrained) == 1 else 'openai'
     clip_model, _, image_processor = open_clip.create_model_and_transforms(
         model_name, pretrained=pretrained, device=device, precision=precision
@@ -46,44 +51,28 @@
 
     # remove text encoder to save footprint and memory
     if hasattr(clip_model, 'text'):
         del clip_model.text
     elif hasattr(clip_model, 'transformer'):
         del clip_model.transformer
 
-    # execution_device = next(iter(clip_model.parameters())).device
-    # add_hook_to_module(clip_model, AlignDevicesHook(io_same_device=True), append=True)
-    #
-    # attach_align_device_hook_on_blocks(
-    #     clip_model,
-    #     execution_device=execution_device,
-    #     offload=None,
-    #     offload_buffers=False,
-    #     weights_map=None,
-    #     preload_module_classes=None,
-    # )
-
     # load the language model
     lang_model, tokenizer = load_llama_model_and_tokenizer(
         model_name_or_path=lang_model_name_or_path,
         tokenizer_name_or_path=tokenizer_name_or_path,
         device=device,
         dtype=dtype,
+        device_map=None,  # TODO: fix this to support multi-gpu
+        no_split_module_classes=no_split_module_classes,
     )
 
     # add Flamingo special tokens to the tokenizer
     tokenizer.add_special_tokens(
         {"additional_special_tokens": ["<|endofchunk|>", "<image>"]}
     )
-    if tokenizer.pad_token is None:
-        # Issue: GPT models don't have a pad token, which we use to
-        # modify labels for the loss.
-        tokenizer.add_special_tokens({"pad_token": "<PAD>"})
-    # For generation padding tokens should be on the left
-    tokenizer.padding_side = "left"
 
     extend_instance(lang_model, FlamingoLMMixin)
 
     if decoder_layers_attr_name is None:
         decoder_layers_attr_name = _infer_decoder_layers_attr_name(lang_model)
     lang_model.set_decoder_layers_attr_name(decoder_layers_attr_name)
     lang_model.resize_token_embeddings(len(tokenizer))
@@ -91,15 +80,15 @@
     flamingo_config = {
         "image_size": open_clip.get_model_config(model_name)["vision_cfg"]["width"],
         "cross_attn_every_n_layers": 4,
         "end_chunk_token_id": tokenizer.encode("<|endofchunk|>")[-1],
         "media_token_id": tokenizer.encode("<image>")[-1],
     }
 
-    model = FlamingoModel(
+    model = FlamingoLMModel(
         clip_model,
         lang_model,
         model_config=flamingo_config,
         device=device,
         dtype=dtype,
     )
```

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/models/flamingo/modeling.py` & `open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/flamingo_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Callable, Optional, Union
 
 import torch
 from einops import rearrange
-from loguru import logger
 from open_flamingo.src.helpers import PerceiverResampler
 from torch import nn
 
+from open_gpt.logging import logger
+
 from ...helper import auto_dtype_and_device
 
 
-class FlamingoModel(nn.Module):
+class FlamingoLMModel(nn.Module):
     def __init__(
         self,
         vision_encoder: 'nn.Module',
         language_model: 'nn.Module',
         device: Optional[Union[str, 'torch.device']] = None,
         dtype: Optional[Union[str, 'torch.dtype']] = None,
         model_config: dict = {},
```

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/models/flan/loading.py` & `open_gpt_torch-0.0.1rc7/open_gpt/models/flan/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/models/loading.py` & `open_gpt_torch-0.0.1rc7/open_gpt/models/loading.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,23 @@
 
     dtype, device = auto_dtype_and_device(dtype, device)
 
     tokenizer = AutoTokenizer.from_pretrained(
         tokenizer_name_or_path or model_name_or_path, trust_remote_code=True
     )
 
+    if tokenizer.pad_token is None:
+        # Issue: GPT models don't have a pad token
+        # tokenizer.add_special_tokens({"pad_token": "<PAD>"})
+        tokenizer.pad_token = tokenizer.eos_token
+        tokenizer.pad_token_id = tokenizer.eos_token_id
+
+    # For generation padding tokens should be on the left
+    tokenizer.padding_side = "left"
+
     if device_map:
         import huggingface_hub
         from accelerate import init_empty_weights, load_checkpoint_and_dispatch
 
         if not os.path.exists(model_name_or_path):
             model_path = huggingface_hub.snapshot_download(model_name_or_path)
         else:
@@ -55,78 +64,78 @@
             model_name_or_path, torch_dtype=dtype, trust_remote_code=True
         )
         model.to(device)
 
     return model, tokenizer
 
 
-def create_model_and_transforms(
-    model_name: str,
-    device: Optional[Union[str, torch.device]] = None,
-    precision: Optional[str] = None,
-    **kwargs,
-):
-    """Create a model of the given name.
-
-    :param model_name: The name of the model to create.
-    :param device: The device to create the model on.
-    :param precision: The precision to use for the model.
-    :param kwargs: Additional arguments to pass to the model.
-    :return: The model.
-    """
-
-    dtype, device = auto_dtype_and_device(precision, device)
-
-    # TODO: Add support for loading config based on model name
-    model_config = {}
-
-    logger.info(
-        f'Loading "{model_name}" with precision: `{dtype}` on device: `{device}`'
-    )
-
-    if model_name.startswith('openflamingo/OpenFlamingo'):
-        from .flamingo.loading import load_model_and_transforms
-
-        model_config = {
-            'vision_model_name_or_path': 'ViT-L-14::openai',
-            'lang_model_name_or_path': 'llama_7B',
-            'tokenizer_name_or_path': 'llama_7B',
-        }
-        return load_model_and_transforms(
-            model_name, device=device, dtype=dtype, **model_config
-        )
-    elif model_name.startswith('facebook/llama'):
-        from .llama.loading import load_model_and_tokenizer
-
-        model_config = {
-            'model_name_or_path': 'llama_7B',
-            'tokenizer_name_or_path': 'llama_7B',
-        }
-        return load_model_and_tokenizer(
-            model_name, device=device, dtype=dtype, **model_config
-        )
-    elif model_name.startswith('google/flan'):
-        from .flan.loading import load_model_and_tokenizer
-
-        return load_model_and_tokenizer(
-            model_name, device=device, dtype=dtype, **model_config
-        )
-    elif model_name.startswith('EleutherAI/pythia'):
-        from .pythia.loading import load_model_and_tokenizer
-
-        return load_model_and_tokenizer(
-            model_name, device=device, dtype=dtype, **model_config
-        )
-    elif model_name.startswith('stabilityai/stablelm'):
-        from .stablelm.loading import load_model_and_tokenizer
-
-        return load_model_and_tokenizer(
-            model_name, device=device, dtype=dtype, **model_config
-        )
-    elif model_name.startswith('fnlp/moss-moon'):
-        from .moss.loading import load_model_and_tokenizer
-
-        return load_model_and_tokenizer(
-            model_name, device=device, dtype=dtype, **model_config, **kwargs
-        )
-    else:
-        raise ValueError(f'Unknown model name: {model_name}')
+# def create_model_and_transforms(
+#     model_name: str,
+#     device: Optional[Union[str, torch.device]] = None,
+#     precision: Optional[str] = None,
+#     **kwargs,
+# ):
+#     """Create a model of the given name.
+#
+#     :param model_name: The name of the model to create.
+#     :param device: The device to create the model on.
+#     :param precision: The precision to use for the model.
+#     :param kwargs: Additional arguments to pass to the model.
+#     :return: The model.
+#     """
+#
+#     dtype, device = auto_dtype_and_device(precision, device)
+#
+#     # TODO: Add support for loading config based on model name
+#     model_config = {}
+#
+#     logger.info(
+#         f'Loading "{model_name}" with precision: `{dtype}` on device: `{device}`'
+#     )
+#
+#     if model_name.startswith('openflamingo/OpenFlamingo'):
+#         from .flamingo.loading import load_model_and_transforms
+#
+#         model_config = {
+#             'vision_model_name_or_path': 'ViT-L-14::openai',
+#             'lang_model_name_or_path': 'llama_7B',
+#             'tokenizer_name_or_path': 'llama_7B',
+#         }
+#         return load_model_and_transforms(
+#             model_name, device=device, dtype=dtype, **model_config
+#         )
+#     elif model_name.startswith('facebook/llama'):
+#         from .llama.loading import load_model_and_tokenizer
+#
+#         model_config = {
+#             'model_name_or_path': 'llama_7B',
+#             'tokenizer_name_or_path': 'llama_7B',
+#         }
+#         return load_model_and_tokenizer(
+#             model_name, device=device, dtype=dtype, **model_config
+#         )
+#     elif model_name.startswith('google/flan'):
+#         from .flan.loading import load_model_and_tokenizer
+#
+#         return load_model_and_tokenizer(
+#             model_name, device=device, dtype=dtype, **model_config
+#         )
+#     elif model_name.startswith('EleutherAI/pythia'):
+#         from .pythia.loading import load_model_and_tokenizer
+#
+#         return load_model_and_tokenizer(
+#             model_name, device=device, dtype=dtype, **model_config
+#         )
+#     elif model_name.startswith('stabilityai/stablelm'):
+#         from .stablelm.loading import load_model_and_tokenizer
+#
+#         return load_model_and_tokenizer(
+#             model_name, device=device, dtype=dtype, **model_config
+#         )
+#     elif model_name.startswith('fnlp/moss-moon'):
+#         from .moss.loading import load_model_and_tokenizer
+#
+#         return load_model_and_tokenizer(
+#             model_name, device=device, dtype=dtype, **model_config, **kwargs
+#         )
+#     else:
+#         raise ValueError(f'Unknown model name: {model_name}')
```

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/models/modeling.py` & `open_gpt_torch-0.0.1rc7/open_gpt/models/modeling.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 from typing import TYPE_CHECKING, List, Optional, Union
 
 import torch
 from torch import nn
 
 from ..helper import auto_dtype_and_device
-from .loading import create_model_and_transforms
 
 if TYPE_CHECKING:
     from transformers import AutoModelForCausalLM, AutoTokenizer
 
 
 class BaseModel(nn.Module):
 
     model: 'AutoModelForCausalLM'
     tokenizer: 'AutoTokenizer'
+    no_split_module_classes: List[str] = None
 
     def __init__(
         self,
         model_name_or_path: str,
         tokenizer_name_or_path: Optional[str] = None,
         dtype: Optional[Union[str, torch.dtype]] = None,
         device: Optional[torch.device] = None,
-        device_map: Optional[Union[str, List[int]]] = 'auto',
-        **kwargs
+        device_map: Optional[Union[str, List[int]]] = None,
+        **kwargs,
     ):
         """Create a model of the given name."""
 
         super().__init__()
 
         self._dtype, self._device = auto_dtype_and_device(dtype, device)
 
-        self._device_map = device_map or 'auto'
+        self._device_map = device_map or 'balanced'
 
         self.load_model_and_transforms(
             model_name_or_path, tokenizer_name_or_path=tokenizer_name_or_path
         )
 
     def load_model_and_transforms(
         self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
     ):
-        self.model, self.tokenizer, *_ = create_model_and_transforms(
+        from .loading import load_model_and_tokenizer
+
+        self.model, self.tokenizer = load_model_and_tokenizer(
             model_name_or_path,
             tokenizer_name_or_path=tokenizer_name_or_path,
             dtype=self._dtype,
             device=self._device,
             device_map=self._device_map,
+            no_split_module_classes=self.no_split_module_classes,
         )
 
         self.model.eval()
 
     def generate(self, prompts: Union[str, List[str]], **kwargs):
         """Generate text from the given prompt."""
```

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/models/pythia/loading.py` & `open_gpt_torch-0.0.1rc7/open_gpt/models/pythia/loading.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/models/stablelm/modeling.py` & `open_gpt_torch-0.0.1rc7/open_gpt/models/flamingo/modeling.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,74 @@
 from typing import List, Optional, Union
 
 import torch
-from transformers import StoppingCriteria, StoppingCriteriaList
+from PIL import Image
 
 from open_gpt.models.modeling import BaseModel
 
 
-class StopOnTokens(StoppingCriteria):
-    def __call__(
-        self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs
-    ) -> bool:
-        stop_ids = [50278, 50279, 50277, 1, 0]
-        for stop_id in stop_ids:
-            if input_ids[0][-1] == stop_id:
-                return True
-        return False
+class FlamingoModel(BaseModel):
+    no_split_module_classes = ["LlamaDecoderLayer"]
+    image_processor = None
 
-
-class StableLMModel(BaseModel):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def load_model_and_transforms(
         self, model_name_or_path: str, tokenizer_name_or_path: Optional[str] = None
     ):
-        from ..loading import load_model_and_tokenizer
+        from .loading import load_model_and_transforms
 
-        self.model, self.tokenizer = load_model_and_tokenizer(
+        self.model, self.tokenizer, self.image_processor = load_model_and_transforms(
             model_name_or_path,
+            vision_model_name_or_path='ViT-L-14::openai',
+            lang_model_name_or_path='facebook/llama_7b',
             tokenizer_name_or_path=tokenizer_name_or_path,
             dtype=self._dtype,
             device=self._device,
             device_map=self._device_map,
-            no_split_module_classes=["GPTNeoXLayer"],
+            no_split_module_classes=self.no_split_module_classes,
         )
 
         self.model.eval()
 
-        if self.tokenizer.pad_token_id is None:
-            self.tokenizer.pad_token = self.tokenizer.eos_token
-            self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
-        self.tokenizer.padding_side = "left"
-
-    def generate(self, prompts: Union[str, List[str]], **kwargs):
+    def generate(self, prompt: str, interleave_images: List[bytes] = [], **kwargs):
         """Generate text from the given prompt."""
-        return super().generate(
-            prompts, stopping_criteria=StoppingCriteriaList([StopOnTokens()]), **kwargs
-        )
+
+        assert isinstance(prompt, str), "Prompt must be a string."
+        prompt_len = len(prompt)
+
+        with torch.inference_mode():
+            vision_x = []
+
+            for image in interleave_images:
+                vision_x.append(self.image_processor(Image.open(image)).unsqueeze(0))
+            vision_x = torch.cat(vision_x, dim=0)
+            vision_x = vision_x.unsqueeze(1).unsqueeze(0)
+
+            lang_x = self.tokenizer(
+                [prompt],
+                padding=True,
+                return_tensors="pt",
+            )
+
+            generated_tokens = self.model.generate(
+                vision_inputs=vision_x,
+                text_inputs=lang_x["input_ids"],
+                attention_mask=lang_x["attention_mask"],
+                max_new_tokens=20,
+                num_beams=6,
+                top_p=0.9,
+                no_repeat_ngram_size=2,
+                temperature=0.7,
+                length_penalty=1.5,
+            )[0].tolist()
+
+            text = self.tokenizer.decode(
+                generated_tokens,
+                clean_up_tokenization_spaces=True,
+                skip_special_tokens=True,
+            )
+
+            text = text[prompt_len:] if text[:prompt_len] == prompt else text
+
+            return text
```

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/profile.py` & `open_gpt_torch-0.0.1rc7/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/serve/executors/base.py` & `open_gpt_torch-0.0.1rc7/open_gpt/serve/executors/base.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/open_gpt/serve/gateway.py` & `open_gpt_torch-0.0.1rc7/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open_gpt_torch-0.0.1rc6/pyproject.toml` & `open_gpt_torch-0.0.1rc7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "open_gpt_torch"
-version = "0.0.1rc6"
+version = "0.0.1rc7"
 description = "An open-source implementation of large-scale language model (LLM)."
 
 license = "Apache-2.0"
 
 authors = [
     "Felix Wang <felix.wang@jina.ai>"
 ]
@@ -41,24 +41,26 @@
 docarray = "^0.21.0"
 loguru = "^0.5"
 cleo = "^2.0.0"
 click = "^8.1.3"
 numpy = "^1.21.2"
 einops = "^0.6.0"
 transformers = "^4.28.0"
-open_clip_torch = "~2.16.0"
+open_clip_torch = "^2.16"
 accelerate = "^0.18.0"
+tqdm = "^4.62.3"
 
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
 open-flamingo = { version = "^0.0", optional = true }
 
 [tool.poetry.extras]
 flamingo = ["open-flamingo"]
 
+
 # Dependency groups are supported for organizing your dependencies
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.0.262"
 mypy = "^1.2.0"
 pre-commit = ">=2.15.0"
 pytest = "^7.1.2"
 pytest-cov = "^3.0"
```

### Comparing `open_gpt_torch-0.0.1rc6/PKG-INFO` & `open_gpt_torch-0.0.1rc7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.1rc6
+Version: 0.0.1rc7
 Summary: An open-source implementation of large-scale language model (LLM).
 Home-page: https://open-gpt.jina.ai
 License: Apache-2.0
 Keywords: Pytorch,LLM,GPT
 Author: Felix Wang
 Author-email: felix.wang@jina.ai
 Requires-Python: >=3.8,<4.0
@@ -26,15 +26,16 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: docarray (>=0.21.0,<0.22.0)
 Requires-Dist: einops (>=0.6.0,<0.7.0)
 Requires-Dist: jina (>=3.15.0,<4.0.0)
 Requires-Dist: loguru (>=0.5,<0.6)
 Requires-Dist: numpy (>=1.21.2,<2.0.0)
 Requires-Dist: open-flamingo (>=0.0,<0.1) ; extra == "flamingo"
-Requires-Dist: open_clip_torch (>=2.16.0,<2.17.0)
+Requires-Dist: open_clip_torch (>=2.16,<3.0)
+Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: transformers (>=4.28.0,<5.0.0)
 Project-URL: Repository, https://github.com/jina-ai/open_gpt
 Description-Content-Type: text/markdown
 
 # OpenGPT
 
 `OpenGPT` is an open-source _cloud-native_ large **multi-modal models** (LMMs) serving solution.
```

