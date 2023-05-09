# Comparing `tmp/lion-pytorch-0.0.7.tar.gz` & `tmp/lion-pytorch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lion-pytorch-0.0.7.tar", last modified: Wed Feb 22 20:57:08 2023, max compression
+gzip compressed data, was "lion-pytorch-0.0.8.tar", last modified: Tue May  9 21:03:43 2023, max compression
```

## Comparing `lion-pytorch-0.0.7.tar` & `lion-pytorch-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:57:08.403190 lion-pytorch-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-22 20:56:57.000000 lion-pytorch-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-22 20:57:08.403190 lion-pytorch-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-02-22 20:56:57.000000 lion-pytorch-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:57:08.403190 lion-pytorch-0.0.7/lion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-22 20:56:57.000000 lion-pytorch-0.0.7/lion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-02-22 20:56:57.000000 lion-pytorch-0.0.7/lion_pytorch/lion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-02-22 20:56:57.000000 lion-pytorch-0.0.7/lion_pytorch/triton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 20:57:08.403190 lion-pytorch-0.0.7/lion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-22 20:57:08.000000 lion-pytorch-0.0.7/lion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-22 20:57:08.000000 lion-pytorch-0.0.7/lion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 20:57:08.000000 lion-pytorch-0.0.7/lion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-22 20:57:08.000000 lion-pytorch-0.0.7/lion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-22 20:57:08.000000 lion-pytorch-0.0.7/lion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 20:57:08.403190 lion-pytorch-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-22 20:56:57.000000 lion-pytorch-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:43.288182 lion-pytorch-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 21:03:43.288182 lion-pytorch-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:43.280182 lion-pytorch-0.0.8/lion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/lion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/lion_pytorch/lion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/lion_pytorch/triton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:43.288182 lion-pytorch-0.0.8/lion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:03:43.288182 lion-pytorch-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/setup.py
```

### Comparing `lion-pytorch-0.0.7/LICENSE` & `lion-pytorch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lion-pytorch-0.0.7/PKG-INFO` & `lion-pytorch-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lion-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Lion Optimizer - Pytorch
 Home-page: https://github.com/lucidrains/lion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lion-pytorch-0.0.7/lion_pytorch/lion_pytorch.py` & `lion-pytorch-0.0.8/lion_pytorch/lion_pytorch.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,16 @@
             betas = betas,
             weight_decay = weight_decay
         )
 
         super().__init__(params, defaults)
 
         self.update_fn = update_fn
+        self.use_triton = use_triton
+        self.took_first_step = False
 
         if use_triton:
             from lion_pytorch.triton import update_fn as triton_update_fn
             self.update_fn = triton_update_fn
 
     @torch.no_grad()
     def step(
@@ -59,14 +61,21 @@
     ):
 
         loss = None
         if exists(closure):
             with torch.enable_grad():
                 loss = closure()
 
+        # address an issue with autotune and in-place updates with triton
+        # on the first .step call, simply do not update parameters in-place, if using triton
+
+        update_kwargs = dict(inplace = False) if self.use_triton and not self.took_first_step else dict()
+
+        # update all parameters
+
         for group in self.param_groups:
             for p in filter(lambda p: exists(p.grad), group['params']):
 
                 grad, lr, wd, beta1, beta2, state = p.grad, group['lr'], group['weight_decay'], *group['betas'], self.state[p]
 
                 # init state - exponential moving average of gradient values
 
@@ -78,11 +87,15 @@
                 self.update_fn(
                     p,
                     grad,
                     exp_avg,
                     lr,
                     wd,
                     beta1,
-                    beta2
+                    beta2,
+                    **update_kwargs
                 )
 
+        if not self.took_first_step:
+            self.took_first_step = True
+
         return loss
```

### Comparing `lion-pytorch-0.0.7/lion_pytorch/triton.py` & `lion-pytorch-0.0.8/lion_pytorch/triton.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import torch
+from torch import Tensor
 
 try:
     import triton
     import triton.language as tl
 except ImportError as e:
     print('triton is not installed, please install by running `pip install triton -U --pre`')
     exit()
 
+# triton cuda kernel
 
 @triton.autotune(configs = [
     triton.Config({'BLOCK_SIZE': 128}, num_warps = 4),
     triton.Config({'BLOCK_SIZE': 1024}, num_warps = 8),
 ], key = ['n_elements'])
 @triton.jit
 def update_fn_kernel(
@@ -68,30 +70,48 @@
 
     # store new params and momentum running average coefficient
 
     tl.store(offset_p_ptr, p, mask = mask)
     tl.store(offset_exp_avg_ptr, exp_avg, mask = mask)
 
 def update_fn(
-    p: torch.Tensor,
-    grad: torch.Tensor,
-    exp_avg: torch.Tensor,
+    p: Tensor,
+    grad: Tensor,
+    exp_avg: Tensor,
     lr: float,
     wd: float,
     beta1: float,
-    beta2: float
+    beta2: float,
+    inplace: bool = True
 ):
     assert all([t.is_cuda for t in (p, grad, exp_avg)])
     n_elements = p.numel()
 
     grid = lambda meta: (triton.cdiv(n_elements, meta['BLOCK_SIZE']),)    
 
+    # address autotune and in-place update issue
+
+    if not inplace:
+        orig_p = p
+        orig_exp_avg = exp_avg
+
+        p = p.clone()
+        exp_avg = exp_avg.clone()
+
+    # call triton cuda kernel
+
     update_fn_kernel[grid](
         p,
         grad,
         exp_avg,
         lr,
         wd,
         beta1,
         beta2,
         n_elements
     )
+
+    # update if not in-place call
+
+    if not inplace:
+        orig_p.copy_(p)
+        orig_exp_avg.copy_(exp_avg)
```

### Comparing `lion-pytorch-0.0.7/lion_pytorch.egg-info/PKG-INFO` & `lion-pytorch-0.0.8/lion_pytorch.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lion-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Lion Optimizer - Pytorch
 Home-page: https://github.com/lucidrains/lion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lion-pytorch-0.0.7/setup.py` & `lion-pytorch-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'lion-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Lion Optimizer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/lion-pytorch',
   keywords = [
```

