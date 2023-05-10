# Comparing `tmp/CoLT5-attention-0.6.2.tar.gz` & `tmp/CoLT5-attention-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.6.2.tar", last modified: Fri May  5 16:53:20 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.7.0.tar", last modified: Wed May 10 20:49:10 2023, max compression
```

## Comparing `CoLT5-attention-0.6.2.tar` & `CoLT5-attention-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 16:53:20.000000 CoLT5-attention-0.6.2/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    29733 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:53:20.663538 CoLT5-attention-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 16:53:02.000000 CoLT5-attention-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 20:49:10.000000 CoLT5-attention-0.7.0/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35401 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:49:10.328197 CoLT5-attention-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 20:48:59.000000 CoLT5-attention-0.7.0/setup.py
```

### Comparing `CoLT5-attention-0.6.2/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.7.0/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.6.2
+Version: 0.7.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.6.2/LICENSE` & `CoLT5-attention-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.6.2/PKG-INFO` & `CoLT5-attention-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.6.2
+Version: 0.7.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.6.2/README.md` & `CoLT5-attention-0.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     mask = tokens_mask,
     context_mask = memories_mask
 )
 
 cross_attn_out.shape # (1, 1024, 512) - same as tokens
 ```
 
-Finally, this repository also has an improvised version for autoregressive attention. The way this was achieved was by viewing the sequence in windows. Each window can only attend to windows of key / values into the past. The local attention of the light branch covers the intra-window attention.
+This repository also has an improvised version for autoregressive attention. The way this was achieved was by viewing the sequence in windows. Each window can only attend to windows of key / values into the past. The local attention of the light branch covers the intra-window attention.
 
 The coordinate descent is made viable through a CUDA kernel written in <a href="https://github.com/openai/triton">Triton</a>. Finally, to get autoregressive generation to work well, I had to make sure for the unrouted tokens (for queries), outputs a learned output embedding rather than just zeros.
 
 Currently I am seeing occasional differences between the gradients (as high as 1e-1 for a very small fraction of elements) once the number of iterations exceed 20. However, enwik8 seems to train well and I can see the effects of the routing. Training is surprisingly stable too
 
 ex.
 
@@ -156,36 +156,59 @@
     use_triton = True,            # will need to use Triton for this to be viable, otherwise it is too slow and memory efficient with the number of iterations
     use_flash_attn = True         # use flash attention in heavy branch
 ).cuda()
 
 attn_out = attn(tokens) + tokens # (2, 8192, 512) - output of attention with residual (prenorm is included)
 ```
 
+Finally, this repository contains a version for image feature maps. Typically a lot of research papers cannot do attention on image feature maps with dimensions greater than 32 by 32. This routed attention will use a local window patch for the light branch, and routed attention for the heavy
+
+ex.
+
+```python
+import torch
+from colt5_attention import ConditionalRoutedImageAttention
+
+attn = ConditionalRoutedImageAttention(
+    dim = 32,
+    light_dim_head = 64,       # attention head dimension of light branch
+    light_heads = 8,           # number of attention heads for light branch
+    light_window_size = 32,    # height and width of local window attention on the image feature map
+    heavy_dim_head = 64,       # attention head dimension of heavy branch
+    heavy_heads = 8,           # number of attention heads for heavy branch
+    num_heavy_tokens_q = 1024, # heavy branch receives only 1024 routed tokens of 65536
+    num_heavy_tokens_kv = 1024 # heavy branch receives only 1024 routed tokens of 65536
+).cuda()
+
+fmap = torch.randn(1, 32, 256, 256).cuda() # image feature map is too large for attention, given 256 ^ 2  == 65536 tokens
+
+out = attn(fmap)
+```
+
 ## Todo
 
 - [x] add the coordinate descent method as another router
 - [x] allow for multi-headed routing (multiple routing tokens), only for key-values
 - [x] add an autoregressive version of the conditionally routed attention
 - [x] test out the autoregressive version and verify that more routed key / value tokens lead to better results - it works
 - [x] make flash attention compatible
+- [x] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 - [x] fused coordinate descent kernel using triton
     - [x] forwards        
     - [x] backwards
     - [x] benchmark triton vs plain pytorch coor_descent - 50 iterations with 4 segments - 18.5x faster for forward (7.23 vs 0.39), 7.2x faster for backwards (5.77 vs 0.80)
     - [x] fall back on plain coordinate descent for cpu
     - [x] handle edge case for when a row is completely masked out for triton, or simply enforce it never to be so
     - [x] fix masking in coordinate descent
     - [x] simplified some logic within the triton kernel and the problem went away. probably some tiny quirk with the compiler
     - [x] maximum block size in triton allowed is 131k, make sure at least quarter of million sequence length can be reached. to get around this initially, one can fold a million token sequence into ~9 131k and uniformly route. offer uniform routing scheme within router itself
     - [x] remove sinkhorn and cumulative softmax approaches and cleanup; neither can work as well as coordinate descent
     - [x] allow for saving intermediates every number of iterations - trading memory for recompute efficiency during backwards
     - [x] in-place write to checkpointed a and b tensor for potentially savings on forward when recompute segments is high
 
-- [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
-
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
     year    = {2023}
```

#### html2text {}

```diff
@@ -45,20 +45,20 @@
 dim_head = 64, heads = 8, num_tokens_q = 512, # only 512 routed from 1024
 num_tokens_kv = 1024, # only 1024 routed from 1 million kv_routing_tokens = 2,
 # say you want 2 routing tokens to route different sets of key / values to the
 queries. 4 attention heads will be allocated to each routed set in this example
 (8 / 2) use_triton = True, # use cuda kernel route_block_size = 131072 # route
 in blocks of 131072 ).cuda() cross_attn_out = cross_attn( tokens, context =
 memories, mask = tokens_mask, context_mask = memories_mask )
-cross_attn_out.shape # (1, 1024, 512) - same as tokens ``` Finally, this
-repository also has an improvised version for autoregressive attention. The way
-this was achieved was by viewing the sequence in windows. Each window can only
-attend to windows of key / values into the past. The local attention of the
-light branch covers the intra-window attention. The coordinate descent is made
-viable through a CUDA kernel written in Triton. Finally, to get autoregressive
+cross_attn_out.shape # (1, 1024, 512) - same as tokens ``` This repository also
+has an improvised version for autoregressive attention. The way this was
+achieved was by viewing the sequence in windows. Each window can only attend to
+windows of key / values into the past. The local attention of the light branch
+covers the intra-window attention. The coordinate descent is made viable
+through a CUDA kernel written in Triton. Finally, to get autoregressive
 generation to work well, I had to make sure for the unrouted tokens (for
 queries), outputs a learned output embedding rather than just zeros. Currently
 I am seeing occasional differences between the gradients (as high as 1e-1 for a
 very small fraction of elements) once the number of iterations exceed 20.
 However, enwik8 seems to train well and I can see the effects of the routing.
 Training is surprisingly stable too ex. ```python import torch from
 colt5_attention import ConditionalRoutedAutoregressiveAttention # mock input,
@@ -76,43 +76,58 @@
 1024, # heavy branch receives only 1024 routed tokens for key-values
 num_routed_kv = 2, # one can split the attention heads so that groups of heads
 attend to different sets of key - values (2 routing tokens in this case)
 use_triton = True, # will need to use Triton for this to be viable, otherwise
 it is too slow and memory efficient with the number of iterations
 use_flash_attn = True # use flash attention in heavy branch ).cuda() attn_out =
 attn(tokens) + tokens # (2, 8192, 512) - output of attention with residual
-(prenorm is included) ``` ## Todo - [x] add the coordinate descent method as
-another router - [x] allow for multi-headed routing (multiple routing tokens),
-only for key-values - [x] add an autoregressive version of the conditionally
-routed attention - [x] test out the autoregressive version and verify that more
-routed key / value tokens lead to better results - it works - [x] make flash
-attention compatible - [x] fused coordinate descent kernel using triton - [x]
+(prenorm is included) ``` Finally, this repository contains a version for image
+feature maps. Typically a lot of research papers cannot do attention on image
+feature maps with dimensions greater than 32 by 32. This routed attention will
+use a local window patch for the light branch, and routed attention for the
+heavy ex. ```python import torch from colt5_attention import
+ConditionalRoutedImageAttention attn = ConditionalRoutedImageAttention( dim =
+32, light_dim_head = 64, # attention head dimension of light branch light_heads
+= 8, # number of attention heads for light branch light_window_size = 32, #
+height and width of local window attention on the image feature map
+heavy_dim_head = 64, # attention head dimension of heavy branch heavy_heads =
+8, # number of attention heads for heavy branch num_heavy_tokens_q = 1024, #
+heavy branch receives only 1024 routed tokens of 65536 num_heavy_tokens_kv =
+1024 # heavy branch receives only 1024 routed tokens of 65536 ).cuda() fmap =
+torch.randn(1, 32, 256, 256).cuda() # image feature map is too large for
+attention, given 256 ^ 2 == 65536 tokens out = attn(fmap) ``` ## Todo - [x] add
+the coordinate descent method as another router - [x] allow for multi-headed
+routing (multiple routing tokens), only for key-values - [x] add an
+autoregressive version of the conditionally routed attention - [x] test out the
+autoregressive version and verify that more routed key / value tokens lead to
+better results - it works - [x] make flash attention compatible - [x] create a
+variant of CoLT5 for high resolution feature maps (image attention) - then try
+out for diffusion - [x] fused coordinate descent kernel using triton - [x]
 forwards - [x] backwards - [x] benchmark triton vs plain pytorch coor_descent -
 50 iterations with 4 segments - 18.5x faster for forward (7.23 vs 0.39), 7.2x
 faster for backwards (5.77 vs 0.80) - [x] fall back on plain coordinate descent
 for cpu - [x] handle edge case for when a row is completely masked out for
 triton, or simply enforce it never to be so - [x] fix masking in coordinate
 descent - [x] simplified some logic within the triton kernel and the problem
 went away. probably some tiny quirk with the compiler - [x] maximum block size
 in triton allowed is 131k, make sure at least quarter of million sequence
 length can be reached. to get around this initially, one can fold a million
 token sequence into ~9 131k and uniformly route. offer uniform routing scheme
 within router itself - [x] remove sinkhorn and cumulative softmax approaches
 and cleanup; neither can work as well as coordinate descent - [x] allow for
 saving intermediates every number of iterations - trading memory for recompute
 efficiency during backwards - [x] in-place write to checkpointed a and b tensor
-for potentially savings on forward when recompute segments is high - [ ] create
-a variant of CoLT5 for high resolution feature maps (image attention) - then
-try out for diffusion ## Citations ```bibtex @inproceedings{Ainslie2023CoLT5FL,
-title = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
-author = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on
-and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and
-James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai}, year = {2023}
-} ``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
-language and compiler for tiled neural network computations}, author =
-{Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
-SIGPLAN International Workshop on Machine Learning and Programming Languages},
-year = {2019} } ``` ```bibtex @inproceedings{dao2022flashattention, title =
-{Flash{A}ttention: Fast and Memory-Efficient Exact Attention with {IO}-
-Awareness}, author = {Dao, Tri and Fu, Daniel Y. and Ermon, Stefano and Rudra,
-Atri and R{\'e}, Christopher}, booktitle = {Advances in Neural Information
-Processing Systems}, year = {2022} } ```
+for potentially savings on forward when recompute segments is high ## Citations
+```bibtex @inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
+Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
+Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
+Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
+Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ``` ```bibtex @article
+{Tillet2019TritonAI, title = {Triton: an intermediate language and compiler for
+tiled neural network computations}, author = {Philippe Tillet and H. Kung and
+D. Cox}, journal = {Proceedings of the 3rd ACM SIGPLAN International Workshop
+on Machine Learning and Programming Languages}, year = {2019} } ``` ```bibtex
+@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
+Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
+Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
+} ```
```

### Comparing `CoLT5-attention-0.6.2/colt5_attention/attend.py` & `CoLT5-attention-0.7.0/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.6.2/colt5_attention/coor_descent.py` & `CoLT5-attention-0.7.0/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.6.2/colt5_attention/transformer_block.py` & `CoLT5-attention-0.7.0/colt5_attention/transformer_block.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,14 +69,54 @@
     return nn.Sequential(
         RMSNorm(dim),
         nn.Linear(dim, dim_hidden),
         nn.GELU(),
         nn.Linear(dim_hidden, dim)
     )
 
+class SelfAttention(nn.Module):
+    def __init__(
+        self,
+        dim,
+        dim_head = 64,
+        heads = 8,
+        use_flash = False,
+        prenorm = False
+    ):
+        super().__init__()
+        self.heads = heads
+        self.scale = dim_head ** -0.5
+        dim_hidden = dim_head * heads
+
+        self.norm = RMSNorm(dim) if prenorm else nn.Identity()
+
+        self.attend = Attend(use_flash = use_flash)
+
+        self.to_qkv = nn.Linear(dim, dim_hidden * 3, bias = False)
+        self.to_out = nn.Linear(dim_hidden, dim, bias = False)
+
+    def forward(self, x):
+        h = self.heads
+
+        x = self.norm(x)
+
+        # get queries, keys, values
+
+        q, k, v = self.to_qkv(x).chunk(3, dim = -1)
+        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
+
+        # attention
+
+        out = self.attend(q, k, v)
+
+        # merge heads
+
+        out = rearrange(out, 'b h n d -> b n (h d)')
+        return self.to_out(out)
+
 class Attention(nn.Module):
     def __init__(
         self,
         dim,
         dim_head = 64,
         heads = 8,
         multiply_keys_by_score = False,
@@ -517,14 +557,150 @@
 
         heavy_out = self.q_router.route_back(heavy_out, routed_tokens_out, indices_q)
 
         # sum light and heavy branches
 
         return light_out + heavy_out
 
+# conditionally routed image feature map attention
+
+class ConditionalRoutedImageAttention(nn.Module):
+    def __init__(
+        self,
+        dim,
+        *,
+        num_heavy_tokens_q,
+        num_heavy_tokens_kv,
+        num_routed_kv = 1,
+        light_dim_head = 64,
+        light_heads = 8,
+        light_window_size = 128,        # each token would see ~ 64 tokens either way to left or right
+        heavy_dim_head = 64,
+        heavy_heads = 8,
+        router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
+        router_kwargs: dict = {},
+        multiply_keys_by_score = False,
+        multiply_queries_by_score = False,
+        use_triton = False,
+        use_null_q_tokens = True,
+        use_flash_attn = False
+    ):
+        super().__init__()
+
+        if use_triton:
+            router_kwargs = {**router_kwargs, 'use_triton': True}
+
+        self.num_heavy_tokens_q = num_heavy_tokens_q
+        self.num_heavy_tokens_kv = num_heavy_tokens_kv
+
+        self.multiply_queries_by_score = multiply_queries_by_score
+
+        self.light_window_size = light_window_size
+
+        self.light_attn = SelfAttention(
+            dim = dim,
+            dim_head = light_dim_head,
+            heads = light_heads,
+            prenorm = True
+        )
+
+        self.null_q_token = None
+        if use_null_q_tokens:
+            self.null_q_token = nn.Parameter(torch.randn(dim)) # for the query tokens not selected by the router, give it a learned output embed
+
+        self.q_router = CoordinateDescentRouter(
+            dim = dim,
+            straight_through = router_straight_through,
+            **router_kwargs
+        )
+
+        self.kv_router = CoordinateDescentRouter(
+            dim = dim,
+            num_routing_tokens = num_routed_kv,
+            straight_through = router_straight_through,
+            **router_kwargs
+        )
+
+        self.heavy_attn = Attention(
+            dim = dim,
+            dim_head = heavy_dim_head,
+            heads = heavy_heads,
+            multiply_keys_by_score = multiply_keys_by_score,
+            use_flash = use_flash_attn
+        )
+
+    def forward(
+        self,
+        x,
+        *,
+        num_heavy_tokens_q = None,
+        num_heavy_tokens_kv = None,
+        mask = None
+    ):
+        batch, device, w = x.shape[0], x.device, self.light_window_size
+
+        num_heavy_tokens_q = default(num_heavy_tokens_q, self.num_heavy_tokens_q)
+        num_heavy_tokens_kv = default(num_heavy_tokens_kv, self.num_heavy_tokens_kv)
+
+        # light local attention sees all tokens in a limited context
+
+        light_input = rearrange(x, 'b d (h p1) (w p2) -> b h w (p1 p2) d', p1 = w, p2 = w)
+        x, ps = pack_one(light_input, '* n d')
+
+        light_out = self.light_attn(x)
+        light_out = unpack_one(light_out, ps, '* n d')
+        light_out = rearrange(light_out, 'b h w (p1 p2) d -> b d (h p1) (w p2)', p1 = w, p2 = w)
+
+        # route tokens appropriately for heavy branch
+
+        normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_heavy_tokens_q, mask = mask)
+        normalized_scores_kv, indices_kv = self.kv_router(x, num_tokens = num_heavy_tokens_kv, mask = mask)
+
+        # select the tokens to be routed to full attention
+
+        routed_tokens_q = batched_gather(x, indices_q)
+
+        kv_batch_range = create_batch_range(x, right_pad_dims = indices_kv.ndim - 1)
+        routed_tokens_kv = batched_gather(x, indices_kv)
+
+        # calculate key padding mask
+
+        routed_tokens_kv_mask = None
+        if exists(mask):
+            routed_tokens_kv_mask = mask[kv_batch_range, indices_kv]
+
+        # do the heavier branch with only routed tokens
+
+        routed_tokens_out = self.heavy_attn(
+            routed_tokens_q,
+            mask = routed_tokens_kv_mask,
+            context = routed_tokens_kv,
+            normalized_scores_kv = normalized_scores_kv,
+            normalized_scores_q = normalized_scores_q if self.multiply_queries_by_score else None
+        )
+
+        routed_tokens_out = routed_tokens_out * rearrange(normalized_scores_q, '... -> ... 1')
+
+        # scatter back the output of the heavy branch
+
+        if exists(self.null_q_token):
+            heavy_out = rearrange(self.null_q_token, 'd -> 1 1 d')
+            heavy_out = heavy_out.expand_as(x).clone()
+        else:
+            heavy_out = torch.zeros_like(x)
+
+        heavy_out = self.q_router.route_back(heavy_out, routed_tokens_out, indices_q)
+
+        heavy_out = unpack_one(heavy_out, ps, '* n d')
+        heavy_out = rearrange(heavy_out, 'b h w (p1 p2) d -> b d (h p1) (w p2)', p1 = w, p2 = w)
+
+        # sum light and heavy branches
+
+        return light_out + heavy_out
+
 # improvised conditionally routed autoregressive attention
 
 class ConditionalRoutedAutoregressiveAttention(nn.Module):
     def __init__(
         self,
         dim,
         *,
```

### Comparing `CoLT5-attention-0.6.2/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.7.0/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.6.2/setup.py` & `CoLT5-attention-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.6.2',
+  version = '0.7.0',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

