# Comparing `tmp/vz-recommender-0.4.4.tar.gz` & `tmp/vz-recommender-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vz-recommender-0.4.4.tar", last modified: Mon Apr  3 22:39:12 2023, max compression
+gzip compressed data, was "vz-recommender-0.4.5.tar", last modified: Wed May 10 01:58:12 2023, max compression
```

## Comparing `vz-recommender-0.4.4.tar` & `vz-recommender-0.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-04-03 22:39:12.569515 vz-recommender-0.4.4/
--rw-r--r--   0 tangca     (502) staff       (20)      567 2022-11-30 18:56:25.000000 vz-recommender-0.4.4/LICENSE
--rw-r--r--   0 tangca     (502) staff       (20)     2535 2023-04-03 22:39:12.569711 vz-recommender-0.4.4/PKG-INFO
--rw-r--r--   0 tangca     (502) staff       (20)     2151 2023-01-24 15:48:11.000000 vz-recommender-0.4.4/README.md
--rw-r--r--   0 tangca     (502) staff       (20)      103 2022-11-30 18:56:26.000000 vz-recommender-0.4.4/pyproject.toml
--rw-r--r--   0 tangca     (502) staff       (20)      508 2023-04-03 22:39:12.570692 vz-recommender-0.4.4/setup.cfg
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-04-03 22:39:12.538372 vz-recommender-0.4.4/src/
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-04-03 22:39:12.545950 vz-recommender-0.4.4/src/vz_recommender/
--rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.4/src/vz_recommender/__init__.py
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-04-03 22:39:12.563725 vz-recommender-0.4.4/src/vz_recommender/models/
--rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.4/src/vz_recommender/models/__init__.py
--rw-r--r--   0 tangca     (502) staff       (20)     4744 2022-11-30 18:56:26.000000 vz-recommender-0.4.4/src/vz_recommender/models/ae.py
--rw-r--r--   0 tangca     (502) staff       (20)    43599 2023-04-03 14:38:11.000000 vz-recommender-0.4.4/src/vz_recommender/models/bst.py
--rw-r--r--   0 tangca     (502) staff       (20)    11865 2023-01-17 15:09:38.000000 vz-recommender-0.4.4/src/vz_recommender/models/context.py
--rw-r--r--   0 tangca     (502) staff       (20)     4418 2023-01-24 17:20:36.000000 vz-recommender-0.4.4/src/vz_recommender/models/mmoe.py
--rw-r--r--   0 tangca     (502) staff       (20)    42611 2023-04-03 14:38:07.000000 vz-recommender-0.4.4/src/vz_recommender/models/moe.py
--rw-r--r--   0 tangca     (502) staff       (20)    13003 2023-01-10 16:37:33.000000 vz-recommender-0.4.4/src/vz_recommender/models/multitask.py
--rw-r--r--   0 tangca     (502) staff       (20)    18072 2023-04-03 14:38:02.000000 vz-recommender-0.4.4/src/vz_recommender/models/pars.py
--rw-r--r--   0 tangca     (502) staff       (20)    18893 2023-03-24 14:13:49.000000 vz-recommender-0.4.4/src/vz_recommender/models/transformer.py
--rw-r--r--   0 tangca     (502) staff       (20)     3988 2023-01-17 15:09:38.000000 vz-recommender-0.4.4/src/vz_recommender/models/txt.py
--rw-r--r--   0 tangca     (502) staff       (20)    10192 2023-03-24 14:13:49.000000 vz-recommender-0.4.4/src/vz_recommender/models/utils.py
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-04-03 22:39:12.568643 vz-recommender-0.4.4/src/vz_recommender/utils/
--rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.4/src/vz_recommender/utils/__init__.py
--rw-r--r--   0 tangca     (502) staff       (20)    10835 2023-03-24 14:13:49.000000 vz-recommender-0.4.4/src/vz_recommender/utils/callbacks_base.py
--rw-r--r--   0 tangca     (502) staff       (20)     4517 2022-11-30 18:56:26.000000 vz-recommender-0.4.4/src/vz_recommender/utils/loggers_base.py
--rw-r--r--   0 tangca     (502) staff       (20)     5763 2023-03-24 14:13:49.000000 vz-recommender-0.4.4/src/vz_recommender/utils/utils.py
-drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-04-03 22:39:12.548684 vz-recommender-0.4.4/src/vz_recommender.egg-info/
--rw-r--r--   0 tangca     (502) staff       (20)     2535 2023-04-03 22:39:12.000000 vz-recommender-0.4.4/src/vz_recommender.egg-info/PKG-INFO
--rw-r--r--   0 tangca     (502) staff       (20)      785 2023-04-03 22:39:12.000000 vz-recommender-0.4.4/src/vz_recommender.egg-info/SOURCES.txt
--rw-r--r--   0 tangca     (502) staff       (20)        1 2023-04-03 22:39:12.000000 vz-recommender-0.4.4/src/vz_recommender.egg-info/dependency_links.txt
--rw-r--r--   0 tangca     (502) staff       (20)       15 2023-04-03 22:39:12.000000 vz-recommender-0.4.4/src/vz_recommender.egg-info/top_level.txt
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.095938 vz-recommender-0.4.5/
+-rw-r--r--   0 tangca     (502) staff       (20)      567 2022-11-30 18:56:25.000000 vz-recommender-0.4.5/LICENSE
+-rw-r--r--   0 tangca     (502) staff       (20)     2535 2023-05-10 01:58:12.096211 vz-recommender-0.4.5/PKG-INFO
+-rw-r--r--   0 tangca     (502) staff       (20)     2151 2023-01-24 15:48:11.000000 vz-recommender-0.4.5/README.md
+-rw-r--r--   0 tangca     (502) staff       (20)      103 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/pyproject.toml
+-rw-r--r--   0 tangca     (502) staff       (20)      508 2023-05-10 01:58:12.097148 vz-recommender-0.4.5/setup.cfg
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.053831 vz-recommender-0.4.5/src/
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.075709 vz-recommender-0.4.5/src/vz_recommender/
+-rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/__init__.py
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.091503 vz-recommender-0.4.5/src/vz_recommender/models/
+-rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/models/__init__.py
+-rw-r--r--   0 tangca     (502) staff       (20)     4744 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/models/ae.py
+-rw-r--r--   0 tangca     (502) staff       (20)    48448 2023-05-09 17:30:48.000000 vz-recommender-0.4.5/src/vz_recommender/models/bst.py
+-rw-r--r--   0 tangca     (502) staff       (20)    11865 2023-01-17 15:09:38.000000 vz-recommender-0.4.5/src/vz_recommender/models/context.py
+-rw-r--r--   0 tangca     (502) staff       (20)     4418 2023-01-24 17:20:36.000000 vz-recommender-0.4.5/src/vz_recommender/models/mmoe.py
+-rw-r--r--   0 tangca     (502) staff       (20)    42778 2023-05-04 20:55:32.000000 vz-recommender-0.4.5/src/vz_recommender/models/moe.py
+-rw-r--r--   0 tangca     (502) staff       (20)    13003 2023-01-10 16:37:33.000000 vz-recommender-0.4.5/src/vz_recommender/models/multitask.py
+-rw-r--r--   0 tangca     (502) staff       (20)    34073 2023-05-09 17:30:35.000000 vz-recommender-0.4.5/src/vz_recommender/models/pars.py
+-rw-r--r--   0 tangca     (502) staff       (20)    39847 2023-05-09 17:30:35.000000 vz-recommender-0.4.5/src/vz_recommender/models/transformer.py
+-rw-r--r--   0 tangca     (502) staff       (20)     3988 2023-01-17 15:09:38.000000 vz-recommender-0.4.5/src/vz_recommender/models/txt.py
+-rw-r--r--   0 tangca     (502) staff       (20)    10192 2023-03-24 14:13:49.000000 vz-recommender-0.4.5/src/vz_recommender/models/utils.py
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.095262 vz-recommender-0.4.5/src/vz_recommender/utils/
+-rw-r--r--   0 tangca     (502) staff       (20)        0 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/utils/__init__.py
+-rw-r--r--   0 tangca     (502) staff       (20)    10835 2023-03-24 14:13:49.000000 vz-recommender-0.4.5/src/vz_recommender/utils/callbacks_base.py
+-rw-r--r--   0 tangca     (502) staff       (20)     4517 2022-11-30 18:56:26.000000 vz-recommender-0.4.5/src/vz_recommender/utils/loggers_base.py
+-rw-r--r--   0 tangca     (502) staff       (20)     5763 2023-03-24 14:13:49.000000 vz-recommender-0.4.5/src/vz_recommender/utils/utils.py
+drwxr-xr-x   0 tangca     (502) staff       (20)        0 2023-05-10 01:58:12.078982 vz-recommender-0.4.5/src/vz_recommender.egg-info/
+-rw-r--r--   0 tangca     (502) staff       (20)     2535 2023-05-10 01:58:12.000000 vz-recommender-0.4.5/src/vz_recommender.egg-info/PKG-INFO
+-rw-r--r--   0 tangca     (502) staff       (20)      785 2023-05-10 01:58:12.000000 vz-recommender-0.4.5/src/vz_recommender.egg-info/SOURCES.txt
+-rw-r--r--   0 tangca     (502) staff       (20)        1 2023-05-10 01:58:12.000000 vz-recommender-0.4.5/src/vz_recommender.egg-info/dependency_links.txt
+-rw-r--r--   0 tangca     (502) staff       (20)       15 2023-05-10 01:58:12.000000 vz-recommender-0.4.5/src/vz_recommender.egg-info/top_level.txt
```

### Comparing `vz-recommender-0.4.4/LICENSE` & `vz-recommender-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/PKG-INFO` & `vz-recommender-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vz-recommender
-Version: 0.4.4
+Version: 0.4.5
 Summary: vz recommender package
 Author: lu
 Author-email: luyang.wang@verizon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `vz-recommender-0.4.4/README.md` & `vz-recommender-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/models/ae.py` & `vz-recommender-0.4.5/src/vz_recommender/models/ae.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/models/bst.py` & `vz-recommender-0.4.5/src/vz_recommender/models/bst.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,20 +68,146 @@
         self.dense2 = torch.nn.Linear((seq_embed_dim+2*wad_embed_dim)//2, seq_embed_dim)
 
     @abc.abstractmethod
     def forward(self, **kwargs):
         pass
 
 
+class BSTAudienceTaWTTwoNLP(nn.Module):
+    def __init__(self, user_deep_dims, user_deep_embed_dims, user_num_wide, user_wad_embed_dim,
+                 offer_deep_dims, offer_deep_embed_dims, offer_num_wide, offer_wad_embed_dim,
+                 svc_dim, svc_embed_dim, new_svc_dim, new_svc_embed_dim,
+                 svc_desc_dly_dim, svc_desc_dly_embed_dim,
+                 page_dim, item_dim, seq_embed_dim,
+                 nlp_encoder_path, nlp_dim, sequence_transformer_kwargs=None):
+        super().__init__()
+        # user layers
+        self.user_context_head = ContextTransformerAndWide(
+            deep_dims=user_deep_dims,
+            num_wide=user_num_wide,
+            deep_embed_dims=user_deep_embed_dims,
+            wad_embed_dim=user_wad_embed_dim,
+        )
+
+        self.svc_embedding = nn.Embedding(svc_dim, svc_embed_dim)
+        self.new_svc_embedding = nn.Embedding(new_svc_dim, new_svc_embed_dim)
+        self.svc_desc_dly_embedding = nn.Embedding(svc_desc_dly_dim, svc_desc_dly_embed_dim)
+        self.mm_pooling = MeanMaxPooling()
+
+        self.page_embedding = nn.Embedding(page_dim, seq_embed_dim)
+        self.item_embedding = nn.Embedding(item_dim, seq_embed_dim)
+        self.sequence_transformer = ParallelTransformerAEP(
+            page_embedding=self.page_embedding,
+            item_embedding=self.item_embedding,
+            dim=seq_embed_dim,
+            dim_head=seq_embed_dim,
+            heads=sequence_transformer_kwargs.get("seq_num_heads"),
+            num_layers=sequence_transformer_kwargs.get("seq_num_layers"),
+        )
+
+        if user_num_wide:
+            user_ctx_out_dims = user_wad_embed_dim
+        else:
+            user_ctx_out_dims = user_wad_embed_dim // 2
+        self.user_att_pooling = ParallelTransformerBlock(
+            dim=seq_embed_dim, dim_head=seq_embed_dim, heads=1
+        )
+        self.user_dense_0 = torch.nn.Linear(
+            # nlp_out + aep_seq_out + user_ctx_out + svc_out + new_svc_out + svc_desc_dly_out
+            in_features=seq_embed_dim + user_ctx_out_dims +
+                        svc_embed_dim * 2 + new_svc_embed_dim * 2 + svc_desc_dly_embed_dim * 2,
+            out_features=seq_embed_dim * 4
+        )
+        self.user_dense_1 = torch.nn.Linear(
+            in_features=seq_embed_dim * 4,
+            out_features=seq_embed_dim
+        )
+        self.user_act = nn.LeakyReLU(0.2)
+        self.user_dropout = nn.Dropout(p=0.1)
+
+        # offer layers
+        self.offer_context_head = ContextTransformerAndWide(
+            deep_dims=offer_deep_dims,
+            num_wide=offer_num_wide,
+            deep_embed_dims=offer_deep_embed_dims,
+            wad_embed_dim=offer_wad_embed_dim,
+        )
+
+        if offer_num_wide:
+            offer_ctx_out_dims = offer_wad_embed_dim
+        else:
+            offer_ctx_out_dims = offer_wad_embed_dim // 2
+        self.offer_dense_0 = torch.nn.Linear(
+            in_features=offer_ctx_out_dims,
+            out_features=offer_ctx_out_dims + offer_ctx_out_dims // 2
+        )
+        self.offer_dense_1 = torch.nn.Linear(
+            in_features=offer_ctx_out_dims + offer_ctx_out_dims // 2,
+            out_features=seq_embed_dim
+        )
+        self.offer_act = nn.LeakyReLU(0.2)
+        self.offer_dropout = nn.Dropout(p=0.1)
+
+        self.out_act = nn.Sigmoid()
+
+    def forward(self, user_deep_in, offer_deep_in, svc_in, new_svc_in, svc_desc_dly_in,
+                page_in, item_in, vl_in, user_wide_in, offer_wide_in):
+        """
+        Args:
+            deep_in: list, a list of Tensor of shape [batch_size, deep_dims].
+            seq_in: Tensor, shape [batch_size, seq_len].
+            vl_in: Tensor, shape [batch_size].
+            wide_in: list, a list of Tensor of shape [batch_size, num_wide].
+            shared_in: list, a list of Tensor of shape [batch_size, num_shared] (default=None).
+            nlp_in: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
+            att_mask: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
+        Return:
+            out: Tensor, shape [batch_size, seq_dim].
+            user_out: Tensor, shape [batch_size, seq_embed_dim].
+        """
+        svc_out = self.svc_embedding(svc_in.long())
+        svc_out = self.mm_pooling(svc_out)
+        new_svc_out = self.new_svc_embedding(new_svc_in.long())
+        new_svc_out = self.mm_pooling(new_svc_out)
+        svc_desc_dly_out = self.svc_desc_dly_embedding(svc_desc_dly_in.long())
+        svc_desc_dly_out = self.mm_pooling(svc_desc_dly_out)
+
+        aep_seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, vl_in=vl_in)
+
+        user_ctx_out = self.user_context_head(deep_in=user_deep_in, wide_in=user_wide_in)
+        user_out = torch.stack([aep_seq_out, user_ctx_out, svc_out, new_svc_out, svc_desc_dly_out], dim=1)
+        user_out = self.user_att_pooling(user_out)
+        user_out = torch.concat(user_out.unbind(1), dim=1)
+        user_out = self.user_dense_0(user_out)
+        user_out = self.user_act(user_out)
+        user_out = self.user_dropout(user_out)
+        user_out = self.user_dense_1(user_out)
+        user_out = self.user_act(user_out)
+
+        offer_ctx_out = self.offer_context_head(deep_in=offer_deep_in, wide_in=offer_wide_in)
+        offer_out = offer_ctx_out
+        offer_out = self.offer_dense_0(offer_out)
+        offer_out = self.offer_act(offer_out)
+        offer_out = self.offer_dropout(offer_out)
+        offer_out = self.offer_dense_1(offer_out)
+        offer_out = self.offer_act(offer_out)
+
+        out = torch.mul(user_out, offer_out)
+        out = torch.sum(out, dim=1)
+        out = self.out_act(out)
+
+        return out, user_out, offer_out
+
+
 class BSTAudienceTaWTT(nn.Module):
     def __init__(self, user_deep_dims, user_deep_embed_dims, user_num_wide, user_wad_embed_dim,
                  offer_deep_dims, offer_deep_embed_dims, offer_num_wide, offer_wad_embed_dim,
                  svc_dim, svc_embed_dim, new_svc_dim, new_svc_embed_dim,
                  svc_desc_dly_dim, svc_desc_dly_embed_dim,
-                 page_dim, page_embed_dim, item_dim, item_embed_dim, seq_embed_dim, seq_hidden_size,
+                 page_dim, item_dim, seq_embed_dim,
                  nlp_encoder_path, nlp_dim, sequence_transformer_kwargs=None):
         super().__init__()
         # user layers
         self.user_context_head = ContextTransformerAndWide(
             deep_dims=user_deep_dims,
             num_wide=user_num_wide,
             deep_embed_dims=user_deep_embed_dims,
@@ -89,55 +215,42 @@
         )
 
         self.svc_embedding = nn.Embedding(svc_dim, svc_embed_dim)
         self.new_svc_embedding = nn.Embedding(new_svc_dim, new_svc_embed_dim)
         self.svc_desc_dly_embedding = nn.Embedding(svc_desc_dly_dim, svc_desc_dly_embed_dim)
         self.mm_pooling = MeanMaxPooling()
 
-        self.page_embedding = nn.Embedding(page_dim, page_embed_dim)
-        self.item_embedding = nn.Embedding(item_dim, item_embed_dim)
-        self.sequence_transformer = TransformerAEPCat(
+        self.page_embedding = nn.Embedding(page_dim, seq_embed_dim)
+        self.item_embedding = nn.Embedding(item_dim, seq_embed_dim)
+        self.sequence_transformer = ParallelTransformerAEP(
             page_embedding=self.page_embedding,
             item_embedding=self.item_embedding,
-            seq_embed_dim=seq_embed_dim,
-            seq_hidden_size=seq_hidden_size,
-            **sequence_transformer_kwargs,
+            dim=seq_embed_dim,
+            dim_head=seq_embed_dim,
+            heads=sequence_transformer_kwargs.get("seq_num_heads"),
+            num_layers=sequence_transformer_kwargs.get("seq_num_layers"),
         )
 
         self.nlp_encoder = DistilBertModel.from_pretrained(nlp_encoder_path)
-        self.search_nlp_dense_0 = torch.nn.Linear(
+        self.nlp_dense_0 = torch.nn.Linear(
             in_features=nlp_dim,
-            out_features=seq_embed_dim * 2
-        )
-        self.search_nlp_dense_1 = torch.nn.Linear(
-            in_features=seq_embed_dim * 2,
             out_features=seq_embed_dim
         )
         self.nlp_act = nn.LeakyReLU(0.2)
 
-#         self.ihq_dense_0 = torch.nn.Linear(
-#             in_features=1024,
-#             out_features=seq_embed_dim * 2
-#         )
-#         self.ihq_dense_1 = torch.nn.Linear(
-#             in_features=seq_embed_dim * 2,
-#             out_features=seq_embed_dim
-#         )
-#         self.ihq_act = nn.LeakyReLU(0.2)
-
         if user_num_wide:
             user_ctx_out_dims = user_wad_embed_dim
         else:
             user_ctx_out_dims = user_wad_embed_dim // 2
         self.user_att_pooling = ParallelTransformerBlock(
             dim=seq_embed_dim, dim_head=seq_embed_dim, heads=1
         )
         self.user_dense_0 = torch.nn.Linear(
-            # nlp_out + aep_seq_out + user_ctx_out + ihq_dim + svc_out + new_svc_out + svc_desc_dly_out
-            in_features=seq_embed_dim + user_ctx_out_dims + seq_embed_dim +
+            # nlp_out + aep_seq_out + user_ctx_out + svc_out + new_svc_out + svc_desc_dly_out
+            in_features=seq_embed_dim + seq_embed_dim + user_ctx_out_dims +
                         svc_embed_dim * 2 + new_svc_embed_dim * 2 + svc_desc_dly_embed_dim * 2,
             out_features=seq_embed_dim * 4
         )
         self.user_dense_1 = torch.nn.Linear(
             in_features=seq_embed_dim * 4,
             out_features=seq_embed_dim
         )
@@ -166,52 +279,43 @@
         )
         self.offer_act = nn.LeakyReLU(0.2)
         self.offer_dropout = nn.Dropout(p=0.1)
 
         self.out_act = nn.Sigmoid()
 
     def forward(self, user_deep_in, offer_deep_in, svc_in, new_svc_in, svc_desc_dly_in,
-                page_in, item_in, vl_in, user_wide_in, offer_wide_in, search_in):
+                page_in, item_in, vl_in, user_wide_in, offer_wide_in, nlp_in):
         """
         Args:
             deep_in: list, a list of Tensor of shape [batch_size, deep_dims].
             seq_in: Tensor, shape [batch_size, seq_len].
             vl_in: Tensor, shape [batch_size].
             wide_in: list, a list of Tensor of shape [batch_size, num_wide].
             shared_in: list, a list of Tensor of shape [batch_size, num_shared] (default=None).
-            search_ids: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
+            nlp_in: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
             att_mask: tensor, Tensor of shape [batch_size, sentence_length] (default=None).
         Return:
             out: Tensor, shape [batch_size, seq_dim].
             user_out: Tensor, shape [batch_size, seq_embed_dim].
         """
         svc_out = self.svc_embedding(svc_in.long())
         svc_out = self.mm_pooling(svc_out)
         new_svc_out = self.new_svc_embedding(new_svc_in.long())
         new_svc_out = self.mm_pooling(new_svc_out)
         svc_desc_dly_out = self.svc_desc_dly_embedding(svc_desc_dly_in.long())
         svc_desc_dly_out = self.mm_pooling(svc_desc_dly_out)
 
         aep_seq_out = self.sequence_transformer(page_in=page_in, item_in=item_in, vl_in=vl_in)
 
-        search_out = self.nlp_encoder(**search_in).last_hidden_state[:, 0, :].to(dtype=torch.float32)
-        search_out = self.search_nlp_dense_0(search_out)
-        search_out = self.nlp_act(search_out)
-        search_out = self.search_nlp_dense_1(search_out)
-        search_out = self.nlp_act(search_out)
-
-#         ihq_out = self.ihq_dense_0(ihq_in)
-#         ihq_out = self.ihq_act(ihq_out)
-#         ihq_out = self.ihq_dense_1(ihq_out)
-#         ihq_out = self.ihq_act(ihq_out)
+        nlp_out = self.nlp_encoder(**nlp_in).last_hidden_state[:, 0, :].to(dtype=torch.float32)
+        nlp_out = self.nlp_dense_0(nlp_out)
+        nlp_out = self.nlp_act(nlp_out)
 
         user_ctx_out = self.user_context_head(deep_in=user_deep_in, wide_in=user_wide_in)
-        user_out = torch.stack([search_out, aep_seq_out, user_ctx_out, 
-#                                 ihq_out,
-                              svc_out, new_svc_out, svc_desc_dly_out], dim=1)
+        user_out = torch.stack([nlp_out, aep_seq_out, user_ctx_out, svc_out, new_svc_out, svc_desc_dly_out], dim=1)
         user_out = self.user_att_pooling(user_out)
         user_out = torch.concat(user_out.unbind(1), dim=1)
         user_out = self.user_dense_0(user_out)
         user_out = self.user_act(user_out)
         user_out = self.user_dropout(user_out)
         user_out = self.user_dense_1(user_out)
         user_out = self.user_act(user_out)
```

### Comparing `vz-recommender-0.4.4/src/vz_recommender/models/context.py` & `vz-recommender-0.4.5/src/vz_recommender/models/context.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/models/mmoe.py` & `vz-recommender-0.4.5/src/vz_recommender/models/mmoe.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/models/moe.py` & `vz-recommender-0.4.5/src/vz_recommender/models/moe.py`

 * *Files 1% similar despite different names*

```diff
@@ -568,16 +568,15 @@
 
         # Mask tokens outside expert capacity. Sum over each sequence
         token_priority = torch.cumsum(expert_index, dim=-2)
 
         # mask if the token routed to to the expert will overflow
         expert_capacity_mask = token_priority <= self.expert_capacity * self.num_K
         expert_index = expert_index * expert_capacity_mask
-        router_probs_top_k = router_probs_top_k.unsqueeze(-1)
-        return expert_index, router_probs_top_k, router_logits
+        return expert_index_list, expert_index, expert_capacity_mask, router_probs_top_k, router_logits
 
 
 class Top1Router(nn.Module):
     """
     Router using tokens choose top-1 experts assignment.
     This router uses the same mechanism as in Switch Transformer (https://arxiv.org/abs/2101.03961) and V-MoE
     (https://arxiv.org/abs/2106.05974): tokens choose their top experts. Items are sorted by router_probs and then
@@ -726,41 +725,43 @@
                  router_ignore_padding_tokens=False, router_dtype="float32", num_K=1):
         super().__init__()
         # Step 1: Get the correct router according to its class
         self.num_K = num_K
         self.router = TopKRouter(num_experts, expert_capacity, hidden_size, router_bias, router_jitter_noise,
                                  router_ignore_padding_tokens, router_dtype, num_K)
         # Step 2: Get the top K experts
-        self.experts = nn.ModuleDict()
-        for idx in range(num_experts):
-            self.experts[f"expert_{idx}"] = expert_class(dim, hidden_size)
+        self.experts = nn.ModuleList([
+            expert_class(dim, hidden_size) for _ in range(4)
+        ])
 
     def forward(self, hidden_states, task_state=None):
         r"""
         Hold on, this will be slightly tricky to understand In the correct order, a MoE layer does the following:
         1- Gets the `router_mask` from the router. The shape of the mask is `(batch_size, sequence_length, num_expert)`. 
         The probabilities are needed in the computation of the hidden states : they are broadcasted to the hidden states 
         values (can be interpreted as a scaling factor). 2- Dispatch the tokens to its associated experts. 
         We do a classic for loop over the experts and assign for each expert the corresponding hidden states.
         """
         # Step 1: Get the k router_masks from the router as wel as the probabilities
         router_state = hidden_states if task_state is None else task_state
-        router_mask, router_probs_top_k, router_logits = self.router(router_state)
-        _, expert_index = torch.topk(router_mask, dim=-1, k=self.num_K)
+        expert_index_list, expert_index, expert_capacity_mask, router_probs_top_k, router_logits = self.router(router_state)
+        _, expert_index = torch.topk(expert_index, dim=-1, k=self.num_K)
 
         # The routers introduced might not always map all the tokens, to a router, which means that some hidden states
         # can be unchanged from one layer to another. That is why the hidden states are cloned before updating only the seleced ones.
 
         next_states = [hidden_states.clone() for _ in range(self.num_K)]
 
         for k in range(self.num_K):
-            for idx, expert in enumerate(self.experts.values()):
-                token_indices = router_mask[:, :, idx].bool()
-                next_states[k][token_indices] = expert(hidden_states[token_indices])
-            next_states[k] *= router_probs_top_k[:, :, k]
+            token_indices_k = torch.nn.functional.one_hot(expert_index_list[:, :, k], num_classes=4).bool()
+            token_indices_k = token_indices_k * expert_capacity_mask
+            for idx, expert in enumerate(self.experts):
+                token_indices = token_indices_k[:, :, idx]
+                p = router_probs_top_k[:, :, k][token_indices].unsqueeze(1)
+                next_states[k][token_indices] = expert(hidden_states[token_indices]) * p
 
         hidden_states = torch.stack(next_states, dim=0).sum(dim=0)
 
         return hidden_states, (router_logits, expert_index)
 
 
 class SparseMoELayer(nn.Module):
```

### Comparing `vz-recommender-0.4.4/src/vz_recommender/models/multitask.py` & `vz-recommender-0.4.5/src/vz_recommender/models/multitask.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/models/txt.py` & `vz-recommender-0.4.5/src/vz_recommender/models/txt.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/models/utils.py` & `vz-recommender-0.4.5/src/vz_recommender/models/utils.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/utils/callbacks_base.py` & `vz-recommender-0.4.5/src/vz_recommender/utils/callbacks_base.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/utils/loggers_base.py` & `vz-recommender-0.4.5/src/vz_recommender/utils/loggers_base.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender/utils/utils.py` & `vz-recommender-0.4.5/src/vz_recommender/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vz-recommender-0.4.4/src/vz_recommender.egg-info/PKG-INFO` & `vz-recommender-0.4.5/src/vz_recommender.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vz-recommender
-Version: 0.4.4
+Version: 0.4.5
 Summary: vz recommender package
 Author: lu
 Author-email: luyang.wang@verizon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `vz-recommender-0.4.4/src/vz_recommender.egg-info/SOURCES.txt` & `vz-recommender-0.4.5/src/vz_recommender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

