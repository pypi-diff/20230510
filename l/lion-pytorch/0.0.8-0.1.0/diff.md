# Comparing `tmp/lion-pytorch-0.0.8.tar.gz` & `tmp/lion-pytorch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lion-pytorch-0.0.8.tar", last modified: Tue May  9 21:03:43 2023, max compression
+gzip compressed data, was "lion-pytorch-0.1.0.tar", last modified: Tue May  9 22:03:20 2023, max compression
```

## Comparing `lion-pytorch-0.0.8.tar` & `lion-pytorch-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:43.288182 lion-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 21:03:43.288182 lion-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:43.280182 lion-pytorch-0.0.8/lion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/lion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/lion_pytorch/lion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/lion_pytorch/triton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:03:43.288182 lion-pytorch-0.0.8/lion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 21:03:43.000000 lion-pytorch-0.0.8/lion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:03:43.288182 lion-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-09 21:03:24.000000 lion-pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:03:20.085794 lion-pytorch-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-09 22:03:03.000000 lion-pytorch-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 22:03:20.085794 lion-pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-09 22:03:03.000000 lion-pytorch-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:03:20.085794 lion-pytorch-0.1.0/lion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 22:03:03.000000 lion-pytorch-0.1.0/lion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-09 22:03:03.000000 lion-pytorch-0.1.0/lion_pytorch/lion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-09 22:03:03.000000 lion-pytorch-0.1.0/lion_pytorch/triton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 22:03:20.085794 lion-pytorch-0.1.0/lion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-09 22:03:20.000000 lion-pytorch-0.1.0/lion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-09 22:03:20.000000 lion-pytorch-0.1.0/lion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 22:03:20.000000 lion-pytorch-0.1.0/lion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-09 22:03:20.000000 lion-pytorch-0.1.0/lion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 22:03:20.000000 lion-pytorch-0.1.0/lion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 22:03:20.085794 lion-pytorch-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-09 22:03:03.000000 lion-pytorch-0.1.0/setup.py
```

### Comparing `lion-pytorch-0.0.8/LICENSE` & `lion-pytorch-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lion-pytorch-0.0.8/PKG-INFO` & `lion-pytorch-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lion-pytorch
-Version: 0.0.8
+Version: 0.1.0
 Summary: Lion Optimizer - Pytorch
 Home-page: https://github.com/lucidrains/lion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lion-pytorch-0.0.8/README.md` & `lion-pytorch-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lion-pytorch-0.0.8/lion_pytorch/lion_pytorch.py` & `lion-pytorch-0.1.0/lion_pytorch/lion_pytorch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import partial
 from typing import Tuple, Optional, Callable
 
 import torch
 from torch.optim.optimizer import Optimizer
 
 # functions
 
@@ -29,15 +30,16 @@
 class Lion(Optimizer):
     def __init__(
         self,
         params,
         lr: float = 1e-4,
         betas: Tuple[float, float] = (0.9, 0.99),
         weight_decay: float = 0.0,
-        use_triton: bool = False
+        use_triton: bool = False,
+        triton_block_size: int = 1024
     ):
         assert lr > 0.
         assert all([0. <= beta <= 1. for beta in betas])
 
         defaults = dict(
             lr = lr,
             betas = betas,
@@ -48,32 +50,27 @@
 
         self.update_fn = update_fn
         self.use_triton = use_triton
         self.took_first_step = False
 
         if use_triton:
             from lion_pytorch.triton import update_fn as triton_update_fn
-            self.update_fn = triton_update_fn
+            self.update_fn = partial(triton_update_fn, BLOCK_SIZE = triton_block_size)
 
     @torch.no_grad()
     def step(
         self,
         closure: Optional[Callable] = None
     ):
 
         loss = None
         if exists(closure):
             with torch.enable_grad():
                 loss = closure()
 
-        # address an issue with autotune and in-place updates with triton
-        # on the first .step call, simply do not update parameters in-place, if using triton
-
-        update_kwargs = dict(inplace = False) if self.use_triton and not self.took_first_step else dict()
-
         # update all parameters
 
         for group in self.param_groups:
             for p in filter(lambda p: exists(p.grad), group['params']):
 
                 grad, lr, wd, beta1, beta2, state = p.grad, group['lr'], group['weight_decay'], *group['betas'], self.state[p]
 
@@ -87,15 +84,11 @@
                 self.update_fn(
                     p,
                     grad,
                     exp_avg,
                     lr,
                     wd,
                     beta1,
-                    beta2,
-                    **update_kwargs
+                    beta2
                 )
 
-        if not self.took_first_step:
-            self.took_first_step = True
-
         return loss
```

### Comparing `lion-pytorch-0.0.8/lion_pytorch/triton.py` & `lion-pytorch-0.1.0/lion_pytorch/triton.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,26 @@
 try:
     import triton
     import triton.language as tl
 except ImportError as e:
     print('triton is not installed, please install by running `pip install triton -U --pre`')
     exit()
 
+# helper functions
+
+def calc_num_warps(block_size):
+    num_warps = 4
+    if block_size >= 2048:
+        num_warps = 8
+    if block_size >= 4096:
+        num_warps = 16
+    return num_warps
+
 # triton cuda kernel
 
-@triton.autotune(configs = [
-    triton.Config({'BLOCK_SIZE': 128}, num_warps = 4),
-    triton.Config({'BLOCK_SIZE': 1024}, num_warps = 8),
-], key = ['n_elements'])
 @triton.jit
 def update_fn_kernel(
     p_ptr,
     grad_ptr,
     exp_avg_ptr,
     lr,
     wd,
@@ -77,41 +83,32 @@
     p: Tensor,
     grad: Tensor,
     exp_avg: Tensor,
     lr: float,
     wd: float,
     beta1: float,
     beta2: float,
-    inplace: bool = True
+    inplace: bool = True,
+    BLOCK_SIZE: int = 1024
 ):
     assert all([t.is_cuda for t in (p, grad, exp_avg)])
-    n_elements = p.numel()
-
-    grid = lambda meta: (triton.cdiv(n_elements, meta['BLOCK_SIZE']),)    
 
-    # address autotune and in-place update issue
-
-    if not inplace:
-        orig_p = p
-        orig_exp_avg = exp_avg
+    n_elements = p.numel()
 
-        p = p.clone()
-        exp_avg = exp_avg.clone()
+    block_size = triton.next_power_of_2(BLOCK_SIZE)
+    num_warps = calc_num_warps(block_size)
+    n_rows = triton.cdiv(n_elements, block_size)
 
     # call triton cuda kernel
 
-    update_fn_kernel[grid](
+    update_fn_kernel[(n_rows,)](
         p,
         grad,
         exp_avg,
         lr,
         wd,
         beta1,
         beta2,
-        n_elements
+        n_elements,
+        num_warps = num_warps,
+        BLOCK_SIZE = BLOCK_SIZE
     )
-
-    # update if not in-place call
-
-    if not inplace:
-        orig_p.copy_(p)
-        orig_exp_avg.copy_(exp_avg)
```

### Comparing `lion-pytorch-0.0.8/lion_pytorch.egg-info/PKG-INFO` & `lion-pytorch-0.1.0/lion_pytorch.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lion-pytorch
-Version: 0.0.8
+Version: 0.1.0
 Summary: Lion Optimizer - Pytorch
 Home-page: https://github.com/lucidrains/lion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lion-pytorch-0.0.8/setup.py` & `lion-pytorch-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'lion-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.1.0',
   license='MIT',
   description = 'Lion Optimizer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/lion-pytorch',
   keywords = [
```

