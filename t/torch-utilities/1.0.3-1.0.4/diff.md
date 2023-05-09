# Comparing `tmp/torch_utilities-1.0.3.tar.gz` & `tmp/torch_utilities-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_utilities-1.0.3.tar", last modified: Sat Apr 15 13:53:30 2023, max compression
+gzip compressed data, was "torch_utilities-1.0.4.tar", last modified: Tue May  9 23:05:44 2023, max compression
```

## Comparing `torch_utilities-1.0.3.tar` & `torch_utilities-1.0.4.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/
--rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2023-04-12 21:50:16.000000 torch_utilities-1.0.3/LICENSE
--rw-rw-r--   0 deema     (1000) deema     (1000)     4980 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     4643 2023-04-15 12:37:07.000000 torch_utilities-1.0.3/README.md
--rw-rw-r--   0 deema     (1000) deema     (1000)       80 2023-04-12 21:50:16.000000 torch_utilities-1.0.3/pyproject.toml
--rw-rw-r--   0 deema     (1000) deema     (1000)      837 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/setup.cfg
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/tests/
--rw-rw-r--   0 deema     (1000) deema     (1000)      196 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3514 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/generate_test_data.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    10294 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     2179 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     5321 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     5870 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     1228 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     9425 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_model_trainer.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    37202 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3675 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/tests/test_pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/torch_utilities/
--rw-rw-r--   0 deema     (1000) deema     (1000)      373 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    19083 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6376 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6300 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    13302 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4664 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3777 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    29223 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/model_trainer.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    44684 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    11611 2023-04-12 21:50:15.000000 torch_utilities-1.0.3/torch_utilities/pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-04-15 13:53:30.153149 torch_utilities-1.0.3/torch_utilities.egg-info/
--rw-rw-r--   0 deema     (1000) deema     (1000)     4980 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     1057 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)        1 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      147 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/entry_points.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      154 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/requires.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)       22 2023-04-15 13:53:30.000000 torch_utilities-1.0.3/torch_utilities.egg-info/top_level.txt
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-09 23:05:44.705839 torch_utilities-1.0.4/
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/LICENSE
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5072 2023-05-09 23:05:44.705839 torch_utilities-1.0.4/PKG-INFO
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4735 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/README.md
+-rw-rw-r--   0 deema     (1000) deema     (1000)       80 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/pyproject.toml
+-rw-rw-r--   0 deema     (1000) deema     (1000)      837 2023-05-09 23:05:44.709839 torch_utilities-1.0.4/setup.cfg
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-09 23:05:44.701839 torch_utilities-1.0.4/tests/
+-rw-rw-r--   0 deema     (1000) deema     (1000)      196 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/__init__.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3514 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/generate_test_data.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    11107 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_audio.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     2179 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_augmentation.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     6096 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_common.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5870 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_data_loading.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     2045 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_features.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_io.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1228 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_metrics.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     9425 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_model_trainer.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    37668 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_modules.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3980 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_pytorch.py
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-09 23:05:44.705839 torch_utilities-1.0.4/torch_utilities/
+-rw-rw-r--   0 deema     (1000) deema     (1000)      410 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/__init__.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    17154 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/audio.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     6376 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/augmentation.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     9044 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/common.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    13587 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/data_loading.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4079 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/features.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     7047 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/io.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1867 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/losses.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3695 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/metrics.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    29213 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/model_trainer.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    45377 2023-05-09 22:59:52.000000 torch_utilities-1.0.4/torch_utilities/modules.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    10451 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/pytorch.py
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-09 23:05:44.705839 torch_utilities-1.0.4/torch_utilities.egg-info/
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5072 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1163 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)        1 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)      147 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/entry_points.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)      154 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/requires.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)       22 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/top_level.txt
```

### Comparing `torch_utilities-1.0.3/LICENSE` & `torch_utilities-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.3/PKG-INFO` & `torch_utilities-1.0.4/torch_utilities.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch_utilities
-Version: 1.0.3
+Name: torch-utilities
+Version: 1.0.4
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,16 +26,17 @@
 ```bash
 python torch_utilities/scripts/run_tests.py
 ```
 This will run a suite of tests to ensure that the module is functioning as expected. If any tests fail, it may indicate that there is a bug in the code or that some aspect of the API has changed. In such cases, we encourage you to open an issue on the repository so that we can help resolve the problem.
 
 
 ## Module Documentation
-To read the API documentation of the module run the following line.
+To read the API documentation of the module you need to clone the repository locally and run pdoc.
 ```bash
+git clone git@github.com:FedericoDiMarzo/torch_utilities.git
 pdoc --docformat numpy torch_utilities/torch_utilities
 ```
 The documentation will then be accessible at the address http://localhost:8080 .
 
 ## Audio Tools
 **Torch Utilities**  includes a comprehensive set of tools for handling audio signals, making it easy for you to preprocess, augment, and manipulate audio data. With simplified *IO utilities*, you can quickly and easily load audio data from disk and save the processed results, without worrying about low level details such as handling PyTorch devices. The module also includes functions for processing and extracting features from audio signals, allowing you to quickly transform raw audio into a format suitable for use with deep learning models.
 These tools support both numpy ndarrays and PyTorch tensors, making it effortless to switch between the two and use the best tool for the job.
```

### Comparing `torch_utilities-1.0.3/README.md` & `torch_utilities-1.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 ```bash
 python torch_utilities/scripts/run_tests.py
 ```
 This will run a suite of tests to ensure that the module is functioning as expected. If any tests fail, it may indicate that there is a bug in the code or that some aspect of the API has changed. In such cases, we encourage you to open an issue on the repository so that we can help resolve the problem.
 
 
 ## Module Documentation
-To read the API documentation of the module run the following line.
+To read the API documentation of the module you need to clone the repository locally and run pdoc.
 ```bash
+git clone git@github.com:FedericoDiMarzo/torch_utilities.git
 pdoc --docformat numpy torch_utilities/torch_utilities
 ```
 The documentation will then be accessible at the address http://localhost:8080 .
 
 ## Audio Tools
 **Torch Utilities**  includes a comprehensive set of tools for handling audio signals, making it easy for you to preprocess, augment, and manipulate audio data. With simplified *IO utilities*, you can quickly and easily load audio data from disk and save the processed results, without worrying about low level details such as handling PyTorch devices. The module also includes functions for processing and extracting features from audio signals, allowing you to quickly transform raw audio into a format suitable for use with deep learning models.
 These tools support both numpy ndarrays and PyTorch tensors, making it effortless to switch between the two and use the best tool for the job.
```

### Comparing `torch_utilities-1.0.3/setup.cfg` & `torch_utilities-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch_utilities
-version = 1.0.3
+version = 1.0.4
 author = Federico Di Marzo
 author_email = federicodimarzo@protonmail.com
 description = Simplifying audio and deep learning with PyTorch.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FedericoDiMarzo/torch_utilities
```

### Comparing `torch_utilities-1.0.3/tests/generate_test_data.py` & `torch_utilities-1.0.4/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.3/tests/test_audio.py` & `torch_utilities-1.0.4/tests/test_audio.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,56 +21,81 @@
 
 class TestSTFT(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         _setup()
 
     def setUp(self):
-        module = (np, torch)  # 0
-        channels = (1, 4)  # 1
-        sample_rate = (8000, 16000, 24000, 48000)  # 2
-        hopsize_ms = (8, 10)  # 3
-        win_oversamp = (1, 2)  # 5
+        module = (np, torch)
+        channels = (1, 4)
+        sample_rate = (8000, 16000, 48000)
+        hopsize_ms = (4, 8)
+        ola_ratio = (2, 3, 4)
+        win_oversamp = (1, 2)
         self.params = product(
             module,
             channels,
             sample_rate,
             hopsize_ms,
+            ola_ratio,
             win_oversamp,
         )
-        self.params = [(*p[:4], 2 * p[3], p[4]) for p in self.params]
 
     def test_stft(self):
         for p in self.params:
-            mod = p[0]
+            (
+                mod,
+                channels,
+                sample_rate,
+                hopsize_ms,
+                ola_ratio,
+                win_oversamp,
+            ) = p
             with self.subTest(p=p):
-                x = mod.ones((p[1], p[2] * 1))
-                y = tu.stft(x, p[2], p[3], "hann", p[4], p[5])
-                bins = int(p[2] * p[4] * p[5] / 2000 + 1)
+                x = mod.ones((channels, sample_rate * 1))
+                win_len_ms = hopsize_ms * ola_ratio
+                y = tu.stft(x, sample_rate, hopsize_ms, "hamming", win_len_ms, win_oversamp)
+                bins = int(sample_rate * win_len_ms * win_oversamp / 2000 + 1)
                 self.assertEqual(y.shape[-1], bins)
 
     def test_istft(self):
         for p in self.params:
-            mod = p[0]
+            (
+                mod,
+                channels,
+                sample_rate,
+                hopsize_ms,
+                ola_ratio,
+                win_oversamp,
+            ) = p
             with self.subTest(p=p):
-                bins = int(p[2] * p[4] * p[5] / 2000 + 1)
-                x = mod.ones((p[1], int(p[2] * 0.05), bins)) + 0j
-                y = tu.istft(x, p[2], p[3], "hann", p[4], p[5])
+                win_len_ms = hopsize_ms * ola_ratio
+                bins = int(sample_rate * win_len_ms * win_oversamp / 2000 + 1)
+                x = mod.ones((channels, int(sample_rate * 0.05), bins)) + 0j
+                y = tu.istft(x, sample_rate, hopsize_ms, "hann", win_len_ms, win_oversamp)
 
     def test_inversion(self):
         for p in self.params:
-            mod = p[0]
+            (
+                mod,
+                channels,
+                sample_rate,
+                hopsize_ms,
+                ola_ratio,
+                win_oversamp,
+            ) = p
             with self.subTest(p=p):
                 if mod == np:
-                    x = np.random.normal(size=(p[1], p[2] * 1))
+                    x = np.random.normal(size=(channels, sample_rate * 1))
                 else:
-                    x = torch.randn((p[1], p[2] * 1))
+                    x = torch.randn((channels, sample_rate * 1))
 
-                y = tu.stft(x, p[2], p[3], "hann", p[4], p[5])
-                x_hat = tu.istft(y, p[2], p[3], "hann", p[4], p[5])
+                win_len_ms = hopsize_ms * ola_ratio
+                y = tu.stft(x, sample_rate, hopsize_ms, "hann", win_len_ms, win_oversamp)
+                x_hat = tu.istft(y, sample_rate, hopsize_ms, "hann", win_len_ms, win_oversamp)
                 x = x[0, : x_hat.shape[1]]
                 x_hat = x_hat[0, : x.shape[0]]
                 err = mod.abs(x - x_hat).max()
                 with suppress(Exception):
                     err = err.item()
                 self.assertAlmostEqual(err, 0, places=5)
```

### Comparing `torch_utilities-1.0.3/tests/test_augmentation.py` & `torch_utilities-1.0.4/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.3/tests/test_common.py` & `torch_utilities-1.0.4/tests/test_common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Tuple
 from pathimport import set_module_root
+from functools import reduce
+from operator import mul
 from ray import tune
-from torch import nn
 import numpy as np
 import itertools
 import unittest
 import torch
 
 set_module_root("../torch_utils")
 set_module_root(".")
@@ -151,10 +151,32 @@
         params = itertools.product(mod, chl)
         xs = [m.ones((1, c, 16)) for m, c in params]
         for x in xs:
             with self.subTest(x=x):
                 y = tu.pack_complex(x)
                 self.assertEqual(y.shape[1], x.shape[1] // 2)
 
+    def test_phase(self):
+        mod = (np, torch)
+        for m in mod:
+            with self.subTest(m=m):
+                phase = np.array([0, 1, 0.2])
+                phase = np.exp(1j * phase)
+                if m == torch:
+                    phase = torch.from_numpy(phase)
+                x = m.ones_like(phase)
+                x = x * phase
+                phase_hat = tu.phase(x)
+                err_max = m.max(m.abs(phase - phase_hat))
+                self.assertLess(err_max, 1e-12)
+
+    def test_factorize(self):
+        expected = [[3, 7, 11], [3, 17], [2, 2, 2, 7]]
+        for exp in expected:
+            with self.subTest(exp=exp):
+                x = reduce(mul, exp)
+                y = tu.factorize(x)
+                self.assertEqual(y, exp)
+
 
 if __name__ == "__main__":
     unittest.main(verbosity=2)
```

### Comparing `torch_utilities-1.0.3/tests/test_data_loading.py` & `torch_utilities-1.0.4/tests/test_data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.3/tests/test_io.py` & `torch_utilities-1.0.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.3/tests/test_metrics.py` & `torch_utilities-1.0.4/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.3/tests/test_model_trainer.py` & `torch_utilities-1.0.4/tests/test_model_trainer.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.3/tests/test_modules.py` & `torch_utilities-1.0.4/tests/test_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -930,88 +930,95 @@
     def setUpClass(cls):
         _setup()
 
     def setUp(self):
         self.in_channels = (2,)
         self.out_channels = (3,)
         self.kernel_size = (4, (5, 3))
-        self.stride_f = (1, 2, 4)
+        self.stride = (1, 2, 4)
         self.dilation = (1, (2, 3))
         self.bias = (False,)
         self.separable = (False, True)
         self.enable_weight_norm = (False, True)
+        self.upsampling_dim = ("time",)
+        # self.upsampling_dim = ("freq", "time")
         self.in_freqs = (16,)
         # ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~
         self.params = product(
             self.in_channels,
             self.out_channels,
             self.kernel_size,
-            self.stride_f,
+            self.stride,
             self.dilation,
             self.bias,
             self.separable,
             self.enable_weight_norm,
+            self.upsampling_dim,
             self.in_freqs,
         )
 
     def get_instance(self, p: Tuple) -> tu.CausalSubConv2d:
         (
             in_channels,
             out_channels,
             kernel_size,
-            stride_f,
+            stride,
             dilation,
             bias,
             separable,
             enable_weight_norm,
+            upsampling_dim,
             in_freqs,
         ) = p
         instance = tu.CausalSubConv2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
-            stride_f=stride_f,
+            stride=stride,
             dilation=dilation,
             bias=bias,
             separable=separable,
+            upsampling_dim=upsampling_dim,
             enable_weight_norm=enable_weight_norm,
         )
         return instance
 
     def get_input(self, p: Tuple) -> Tensor:
         (
             in_channels,
             out_channels,
             kernel_size,
-            stride_f,
+            stride,
             dilation,
             bias,
             separable,
             enable_weight_norm,
+            upsampling_dim,
             in_freqs,
         ) = p
         x = _get_input(in_channels, in_freqs, None)
         return x
 
     def test_inner_modules(self):
         for p in self.params:
             (
                 in_channels,
                 out_channels,
                 kernel_size,
-                stride_f,
+                stride,
                 dilation,
                 bias,
                 separable,
                 enable_weight_norm,
+                upsampling_dim,
                 in_freqs,
             ) = p
             with self.subTest(p=p):
                 csc = self.get_instance(p)
-                self.assertEqual(len(csc.layers), stride_f)
+                self.assertEqual(len(csc.layers), stride)
                 for layer in csc.layers:
                     self.assertEqual(layer.in_channels, in_channels)
                     self.assertEqual(layer.out_channels, out_channels)
                     self.assertEqual(layer.kernel_size, kernel_size)
                     self.assertEqual(layer.stride_f, 1)
                     self.assertEqual(layer.dilation, dilation)
                     self.assertEqual(layer.bias, bias)
@@ -1020,27 +1027,33 @@
 
     def test_forward(self):
         for p in self.params:
             (
                 in_channels,
                 out_channels,
                 kernel_size,
-                stride_f,
+                stride,
                 dilation,
                 bias,
                 separable,
                 enable_weight_norm,
+                upsampling_dim,
                 in_freqs,
             ) = p
             with self.subTest(p=p):
                 csc = self.get_instance(p)
                 x = self.get_input(p)
                 y = csc(x)
                 B, C, T, F = x.shape
-                self.assertEqual(y.shape, (B, out_channels, T, in_freqs * stride_f))
+                expected_shape = (
+                    (B, out_channels, T, in_freqs * stride)
+                    if upsampling_dim == "freq"
+                    else (B, out_channels, T * stride, in_freqs)
+                )
+                self.assertEqual(y.shape, expected_shape)
 
 
 # = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = =
 
 
 class TestSlidingCausalMultiheadAttention(unittest.TestCase):
     @classmethod
```

### Comparing `torch_utilities-1.0.3/tests/test_pytorch.py` & `torch_utilities-1.0.4/tests/test_pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathimport import set_module_root
-from typing import Tuple
-from torch import nn
+from typing import Iterable, Tuple
+from torch import Tensor, nn
 import numpy as np
 import itertools
 import unittest
 import torch
 
 set_module_root("../torch_utils")
 set_module_root(".")
@@ -68,14 +68,21 @@
         names = ("a", "b")
         scores = (-10.2, 11)
         checkpoints = list(zip(names, scores))
         checkpoints = tu.sort_checkpoints(checkpoints)
         self.assertEqual(checkpoints[0][0], "b")
         self.assertEqual(checkpoints[1][0], "a")
 
+    @torch.set_grad_enabled(True)
+    def test_freeze_model(self):
+        module = nn.Conv2d(2, 2, 1)
+        self.assertTrue(all(p.requires_grad for p in module.parameters()))
+        tu.freeze_model(module)
+        self.assertFalse(all(p.requires_grad for p in module.parameters()))
+
 
 class TestCosineScheduler(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         _setup()
 
     def setUp(self):
```

### Comparing `torch_utilities-1.0.3/torch_utilities/audio.py` & `torch_utilities-1.0.4/torch_utilities/audio.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 import torch.nn.functional as F
 from random import randrange
 from torch import Tensor
 import numpy as np
 import torch
 
 set_module_root(".")
-from torch_utilities.common import get_np_or_torch, TensorOrArray, to_numpy
-from torch_utilities.io import load_audio, load_audio_parallel_itr
-from torch_utilities.pytorch import get_device
+from torch_utilities.common import get_np_or_torch, TensorOrArray, to_numpy, get_device
 
 
 # export list
 __all__ = [
     "stft",
     "istft",
     "MelFilterbank",
@@ -26,15 +24,14 @@
     "energy",
     "rms",
     "snr",
     "fade_sides",
     "random_trim",
     "trim_silence",
     "interleave",
-    "pack_audio_sequences",
 ]
 
 
 def stft(
     x: TensorOrArray,
     sample_rate: int = 16000,
     hopsize_ms: int = 10,
@@ -200,28 +197,40 @@
         pad_ovr = n_fft - win_len
         pad_ctr = win_len // 2
         x = F.pad(x, (pad_ctr, pad_ovr))
     else:
         transform = torch.istft
         x = _transpose(x)
 
-    y = transform(
-        x,
-        n_fft=n_fft,
-        hop_length=hopsize,
-        window=_window,
-        return_complex=is_stft,
-        center=True,
-    )
+    try:
+        y = transform(
+            x,
+            n_fft=n_fft,
+            hop_length=hopsize,
+            window=_window,
+            return_complex=is_stft,
+            center=True,
+        )
+    except RuntimeError as e:
+        # TODO: pytorch bug
+        # for some reason, few configurations do not pass the NOLA check even if
+        # they should pass it. This seems to be a bug related to PyTorch
+        err_msg = "The configuration you provided does not satisfies PyTorch NOLA check"
+        raise RuntimeError(str(e) + "\n" + err_msg)
 
     if is_stft:
         # reshaping
         y = _transpose(y)
         # compensating for center==True
         y = y[:, 1:]
+    else:
+        # compensating for ola ratio
+        # it's still not clear where this shift comes from
+        ola_shift = (win_len // hopsize - 2) * (hopsize // 2)
+        y = y[:, ola_shift:]
 
     if in_type == np.ndarray:
         # converting to numpy
         y = to_numpy(y)
 
     return y
 
@@ -683,89 +692,7 @@
     new_shape[-1] *= stride
     y = mod.zeros(new_shape)
 
     for i, x in enumerate(xs):
         y[..., i::stride] = x
 
     return y
-
-
-def pack_audio_sequences(
-    xs: List[Path],
-    length: float,
-    sample_rate: int,
-    channels: int = 1,
-    tensor: bool = False,
-    delete_last: bool = True,
-    num_workers: int = 1,
-) -> Iterator[TensorOrArray]:
-    """
-    Reads from a list of audio filepaths and generate temporal sequences
-    of a certain length.
-
-    Parameters
-    ----------
-    xs : List[Path]
-        List of audio filepaths
-    length : float
-        Length of the sequences is seconds
-    sample_rate : int
-        Resample at this sample frequency
-    channels : int, optional
-        Number of channels of the sequences, by default 1
-    tensor : bool, optional
-        If False returns a numpy ndarray else a torch Tensor, by default False
-    delete_last : bool, optional
-        If True the last sequence is discarded (since it's typically not complete),
-        by default True
-    num_workers : int, optional
-        Number of parallel processes
-
-    Yields
-    ------
-    Iterator[TensorOrArray]
-        Audio sequence of shape
-        (length, C, T)
-    """
-    # length in samples
-    length = int(length * sample_rate)
-
-    # the container of the sequences to be generated
-    _zeros = torch.zeros if tensor else np.zeros
-    _reset_seq = lambda: _zeros((channels, length))
-
-    # point to the last index consumed
-    sample_ptr = 0
-    seq_ptr = 0
-
-    # utilities
-    _seq_left = lambda: length - seq_ptr
-    _sample_left = lambda x: x.shape[1] - sample_ptr
-    _copy = lambda x: x.clone() if isinstance(x, Tensor) else x.copy()
-
-    # enables multiprocessing ~ ~ ~ ~ ~
-    if num_workers > 1:
-        xs = load_audio_parallel_itr(xs, sample_rate, tensor, num_workers=num_workers)
-    else:
-        xs = (load_audio(x, sample_rate, tensor)[0] for x in xs)
-    # ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~ ~
-
-    seq = _reset_seq()
-    for x in xs:
-        while _sample_left(x) > 0:
-            # copying into the sequence
-            delta = min(_seq_left(), _sample_left(x))
-            seq[:, seq_ptr : seq_ptr + delta] = x[:channels, sample_ptr : sample_ptr + delta]
-            seq_ptr += delta
-            sample_ptr += delta
-
-            if _seq_left() == 0:
-                # sequence complete
-                yield _copy(seq)
-                seq = _reset_seq()
-                seq_ptr = 0
-
-        # sample consumed
-        sample_ptr = 0
-
-    if not delete_last:
-        yield _copy(seq)
```

### Comparing `torch_utilities-1.0.3/torch_utilities/augmentation.py` & `torch_utilities-1.0.4/torch_utilities/augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.3/torch_utilities/data_loading.py` & `torch_utilities-1.0.4/torch_utilities/data_loading.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,15 +234,14 @@
             Total item in an epoch, by default 1024
         overfit_mode : bool, optional
             If True, always returns the first batch at every iteration
         """
         super(HDF5OnlineDataset).__init__()
         self.datasets_paths = dataset_paths
         self.data_layouts = data_layouts
-        self.data_layouts = data_layouts
         self.batch_size = batch_size
         self.total_items = total_items
         self.overfit_mode = overfit_mode
 
         # error handling
         err_msg = f"total_items ({total_items}) must be divisible by batch_size ({batch_size})"
         assert (self.total_items % self.batch_size) == 0, err_msg
@@ -390,16 +389,18 @@
 
 
 def plot_dataset_statistics(
     dataloader: DataLoader,
     iterations: int,
     n_hist_bins: int = 100,
     labels: Optional[List[str]] = None,
+    save_path:Optional[Path] = None,
     figsize: Tuple[int, int] = (8, 6),
     verbose: bool = False,
+
 ) -> List[Tuple[np.ndarray, np.ndarray, float, float, float, float]]:
     """
     Plots the statistics for the data obtained
     from a dataset.
 
     Parameters
     ----------
@@ -407,19 +408,22 @@
         DataLoader to iterate
     iterations : int
         Number of iterations
     n_hist_bins : int, optional
         Number of histogram bins
     labels : Optional[List[str]]
         Names of the dataset outputs
+    save_path : Optional[Path]
+        If specified saves the plots in the specified folder
     figsize : Tuple[int, int], optional
         Size of the plot, by default (8, 6)
     verbose : bool, optional
         If True shows a progress bar for the iterations,
         by default False
+    
 
     Returns
     -------
     List[Tuple[np.ndarray, np.ndarray, float, float, float]]
         List of statistics for each dataset output
         each tuple contains
         (hist_vals, hist_bins, min, max, mean, var)
@@ -429,25 +433,32 @@
     all_stats = get_dataset_statistics(
         dataloader,
         iterations,
         n_hist_bins,
         verbose,
     )
 
-    if labels == None:
-        # default labels
+    # default labels
+    if labels is None:
         labels = [f"feature_{i}" for i in range(len(all_stats))]
 
+    # optional save path
+    if save_path is not None:
+        save_path = Path(save_path)
+
     for stats, name in zip(all_stats, labels):
         hist_vals, hist_bins, min, max, mean, var = stats
         bar_width = np.abs(hist_bins[1] - hist_bins[0])
         plt.figure(figsize=figsize)
         plt.title(f"{name} distribution")
         plt.bar(hist_bins[:-1], hist_vals, width=bar_width)
         plt.vlines(x=mean, ymin=0, ymax=1, colors="red", label="mean")
         plt.ylim([0, hist_vals.max()])
         plt.legend()
         plt.grid()
-        plt.show()
+        if save_path is not None:
+            plt.savefig(save_path / f"{name}.png")
+        else:
+            plt.show()
         plt.close()
 
     return all_stats
```

### Comparing `torch_utilities-1.0.3/torch_utilities/metrics.py` & `torch_utilities-1.0.4/torch_utilities/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,17 +102,14 @@
         Returns
         -------
         Tuple[float, float, float]
             (ovr, sig, bak)
         """
         assert len(x.shape) == 2, "the shape of x should be (C, T)"
 
-        # # Mel transform
-        # x = self.stft(x)
-        # x = self.mel_fb(x)
         if isinstance(x, Tensor):
             x = to_numpy(x)
         x = x.astype("float32")
 
         # keeping the first channel
         x = x[:1]
```

### Comparing `torch_utilities-1.0.3/torch_utilities/model_trainer.py` & `torch_utilities-1.0.4/torch_utilities/model_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,18 +478,18 @@
         """
         self.running_losses = np.zeros(len(self.losses))
         self.running_losses_steps = 0
 
     # = = = = = = = = = = = = = = = = = = = = = =
     #               Callbacks
     # = = = = = = = = = = = = = = = = = = = = = =
-    def on_train_begin(self: int) -> None:
+    def on_train_begin(self) -> None:
         pass
 
-    def on_train_end(self: int) -> None:
+    def on_train_end(self) -> None:
         pass
 
     def on_epoch_begin(self, epoch: int) -> None:
         pass
 
     def on_epoch_end(self, epoch: int) -> None:
         pass
```

### Comparing `torch_utilities-1.0.3/torch_utilities/modules.py` & `torch_utilities-1.0.4/torch_utilities/modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Module parameter
 
     Returns
     -------
     scalar
         Temporal parameter
     """
-    if isinstance(param, tuple):
+    if type(param) in (tuple, list):
         return param[0]
     else:
         return param
 
 
 def get_freq_value(param):
     """
@@ -70,15 +70,15 @@
         Module parameter
 
     Returns
     -------
     scalar
         Temporal parameter
     """
-    if isinstance(param, tuple):
+    if type(param) in (tuple, list):
         return param[1]
     else:
         return param
 
 
 def get_causal_conv_padding(kernel_size: int, dilation: int) -> int:
     """
@@ -207,22 +207,22 @@
 class Reparameterize(Module):
     def __init__(self) -> None:
         super().__init__()
 
     def forward(self, mu: Tensor, logvar: Tensor) -> Tensor:
         """
         Reparameterization trick to sample
-        from N(mu, var) from N(0,1).
+        from N(mu, var) without breaking the gradient path.
 
         Parameters
         ----------
         mu : Tensor
             Mean of the latent normal
         logvar : Tensor
-            Standard deviation of the latent normal in log
+            Standard deviation of the latent normal in log scale
 
         Returns
         -------
         Tensor
             Sample from the normal distribution
         """
         std = torch.exp(0.5 * logvar)
@@ -630,27 +630,27 @@
             layers.append(full_conv)
         else:
             # separable convolution
             # depthwise + pointwise
             depthwise = self._normalize(
                 nn.Conv2d(
                     in_channels=self.in_channels,
-                    out_channels=self.out_channels,
+                    out_channels=self.in_channels,
                     kernel_size=self.kernel_size,
                     stride=(1, stride_f),
                     dilation=self.dilation,
                     bias=self.bias,
                     groups=self.groups,
                     dtype=self.dtype,
                     padding=conv_pad,
                 )
             )
             pointwise = self._normalize(
                 nn.Conv2d(
-                    in_channels=self.out_channels,
+                    in_channels=self.in_channels,
                     out_channels=self.out_channels,
                     kernel_size=1,
                     bias=False,
                     dtype=self.dtype,
                 )
             )
             layers += [depthwise, pointwise]
@@ -692,50 +692,58 @@
 
 class CausalSubConv2d(Module):
     def __init__(
         self,
         in_channels: int,
         out_channels: int,
         kernel_size: OneOrPair[int],
-        stride_f: int = 1,
+        stride: int = 1,
         dilation: OneOrPair[int] = 1,
         bias: bool = True,
         separable: bool = False,
         enable_weight_norm: bool = False,
+        upsampling_dim: str = "freq",
         dtype=None,
     ) -> None:
         """
         Also known as sub pixel convolution, described in
         Dense CNN With Self-Attention for Time-Domain Speech Enhancement
         paper (https://ieeexplore.ieee.org/document/9372863).
 
-        Many convolutions are interleaved to upsample a signal over frequency.
+        Many convolutions are interleaved to upsample a signal over frequency or time.
 
         Parameters
         ----------
         Same parameters as Conv2d plus
 
-        stride_f : int
+        stride : int
             Defines how many interleaved convolutions are present
         separable : bool, optional
             Enable separable convolution (depthwise + pointwise), by default False
         enable_weight_norm : bool, optional
             Enables weight normalization, by default False
+        upsampling_dim : str, optional
+            One between ["freq", "time"]
         """
         super().__init__()
 
+        # error handling
+        err_msg = 'upsampling_dim should be one between ["freq", "time"]'
+        assert upsampling_dim in ["freq", "time"], err_msg
+
         # attributes
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.kernel_size = kernel_size
-        self.stride_f = stride_f
+        self.stride = stride
         self.dilation = dilation
         self.bias = bias
         self.separable = separable
         self.enable_weight_norm = enable_weight_norm
+        self.upsampling_dim = upsampling_dim
         self.dtype = dtype
 
         # inner modules
         _conv = lambda: CausalConv2d(
             in_channels=in_channels,
             out_channels=out_channels,
             kernel_size=kernel_size,
@@ -743,30 +751,37 @@
             padding_f=None,
             dilation=dilation,
             bias=bias,
             separable=separable,
             enable_weight_norm=enable_weight_norm,
             dtype=dtype,
         )
-        self.layers = nn.Sequential(*[_conv() for _ in range(self.stride_f)])
+        self.layers = nn.Sequential(*[_conv() for _ in range(self.stride)])
+        self.transpose = lambda x: x.transpose(2, 3)
 
     def forward(self, x: Tensor) -> Tensor:
         """
         Parameters
         ----------
         x : Tensor
             Input of shape (B, C, T, F)
 
         Returns
         -------
         Tensor
-            Output of shape (B, C, T, F * stride_f)
+            Output of shape (B, C, T, F * stride) -> if upsampling_dim == "freq"
+            Output of shape (B, C, T * stride, F) -> if upsampling_dim == "time"
         """
         xs = [conv(x) for conv in self.layers]
-        x = interleave(*xs)
+        if self.upsampling_dim == "time":
+            xs = [self.transpose(x) for x in xs]
+            x = interleave(*xs)
+            x = self.transpose(x)
+        else:
+            x = interleave(*xs)
         return x
 
 
 # conv2d compositions = = = = = = = = = = = = = = = = =
 class CausalConv2dNormAct(Module):
     def __init__(
         self,
```

### Comparing `torch_utilities-1.0.3/torch_utilities/pytorch.py` & `torch_utilities-1.0.4/torch_utilities/pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,111 +1,49 @@
-from typing import Any, Callable, Iterator, List, Dict, Tuple
+from typing import Iterator, List, Dict, Tuple
 from pathimport import set_module_root
 from torch import autograd as AG
 import torch.nn.functional as F
-from functools import partial
 from torch import nn, Tensor
 from pathlib import Path
-from torch import Tensor
 import numpy as np
 import torch
 import yaml
 
-
 # export list
 __all__ = [
     # pytorch utilities
-    "get_device",
     "enable_anomaly_detection",
-    "set_device",
-    "auto_device",
     "load_model",
     "load_checkpoints",
     "sort_checkpoints",
     "get_submodules",
     "compute_gradients",
     "get_gradients",
     "get_model_parameters",
+    "freeze_model",
     "quantize",
     "one_hot_quantization",
     "invert_one_hot",
     "CosineScheduler",
 ]
 
 
-def get_device() -> str:
-    """
-    Gets the first CUDA device available or CPU
-    if no CUDA device is available.
-
-    Returns
-    -------
-    str
-        Device id
-    """
-    return "cuda" if torch.cuda.is_available() else "cpu"
+set_module_root(".")
+from torch_utilities.common import get_device
 
 
 def enable_anomaly_detection():
     """
     Enable PyTorch anomaly detection
     """
     from torch import autograd
 
     autograd.anomaly_mode.set_detect_anomaly(True)
 
 
-def set_device(device: str, dtype: str = "Float") -> None:
-    """
-    Sets the default pytorch tensor
-    to 'torch.{device}.FloatTensor'
-
-    if device == "auto" it's inferred from get_device()
-
-    Parameters
-    ----------
-    device : str
-        Name of the device or "auto"
-    dtype : str, optional
-        Type of the tensor, by default "Float"
-    """
-    if device == "auto":
-        device = get_device()
-    if device == "cpu":
-        torch.set_default_tensor_type(f"torch.{dtype}Tensor")
-    else:
-        torch.set_default_tensor_type(f"torch.{device}.{dtype}Tensor")
-
-
-def auto_device(dtype: str = "Float") -> Callable:
-    def _auto_device(f: Callable) -> Callable:
-        """
-        Decorator to set the pytorch device to auto.
-
-        Parameters
-        ----------
-        f : Callable
-            Function to decorate
-        dtype : str, optional
-            Type of the tensor, by default "Float"
-
-        Returns
-        -------
-        Callable
-            Decorated function
-        """
-        set_device("auto", dtype)
-        return f
-
-    return _auto_device
-
-
-auto_device = partial(auto_device)
-
-
 def load_model(
     model_path: Path,
     model_class: nn.Module,
     *model_args: List,
     **model_kwargs: Dict,
 ) -> nn.Module:
     """
@@ -127,15 +65,15 @@
     checkpoint_dir = model_path / "checkpoints"
     checkpoint_scores = checkpoint_dir / "ckpt.yml"
     checkpoint_scores = load_checkpoints(checkpoint_scores)
     best_checkpoint = checkpoint_dir / checkpoint_scores[0][0]
     config = model_path / "config.yml"
     model_state = torch.load(best_checkpoint, map_location=get_device())
     model_state = model_state["model_state"]
-    
+
     # initializing the model
     model = model_class(config, *model_args, **model_kwargs)
     model.load_state_dict(model_state)
     model.eval()
     return model
 
 
@@ -282,14 +220,27 @@
     -------
     int
         Total number of parameters
     """
     return sum(p.numel() for p in model.parameters())
 
 
+def freeze_model(model: nn.Module) -> None:
+    """
+    Freezed the weights of a target module.
+
+    Parameters
+    ----------
+    model : nn.Module
+        Model to freeze
+    """
+    for p in model.parameters():
+        p.requires_grad = False
+
+
 def quantize(x: Tensor, steps: int, min: float = -1, max: float = 1) -> Tensor:
     """
     Quantize a real signal.
 
     Parameters
     ----------
     x : Tensor
```

### Comparing `torch_utilities-1.0.3/torch_utilities.egg-info/PKG-INFO` & `torch_utilities-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: torch-utilities
-Version: 1.0.3
+Name: torch_utilities
+Version: 1.0.4
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -26,16 +26,17 @@
 ```bash
 python torch_utilities/scripts/run_tests.py
 ```
 This will run a suite of tests to ensure that the module is functioning as expected. If any tests fail, it may indicate that there is a bug in the code or that some aspect of the API has changed. In such cases, we encourage you to open an issue on the repository so that we can help resolve the problem.
 
 
 ## Module Documentation
-To read the API documentation of the module run the following line.
+To read the API documentation of the module you need to clone the repository locally and run pdoc.
 ```bash
+git clone git@github.com:FedericoDiMarzo/torch_utilities.git
 pdoc --docformat numpy torch_utilities/torch_utilities
 ```
 The documentation will then be accessible at the address http://localhost:8080 .
 
 ## Audio Tools
 **Torch Utilities**  includes a comprehensive set of tools for handling audio signals, making it easy for you to preprocess, augment, and manipulate audio data. With simplified *IO utilities*, you can quickly and easily load audio data from disk and save the processed results, without worrying about low level details such as handling PyTorch devices. The module also includes functions for processing and extracting features from audio signals, allowing you to quickly transform raw audio into a format suitable for use with deep learning models.
 These tools support both numpy ndarrays and PyTorch tensors, making it effortless to switch between the two and use the best tool for the job.
```

### Comparing `torch_utilities-1.0.3/torch_utilities.egg-info/SOURCES.txt` & `torch_utilities-1.0.4/torch_utilities.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,33 +4,37 @@
 setup.cfg
 ./tests/__init__.py
 ./tests/generate_test_data.py
 ./tests/test_audio.py
 ./tests/test_augmentation.py
 ./tests/test_common.py
 ./tests/test_data_loading.py
+./tests/test_features.py
 ./tests/test_io.py
 ./tests/test_metrics.py
 ./tests/test_model_trainer.py
 ./tests/test_modules.py
 ./tests/test_pytorch.py
 ./torch_utilities/__init__.py
 ./torch_utilities/audio.py
 ./torch_utilities/augmentation.py
 ./torch_utilities/common.py
 ./torch_utilities/data_loading.py
+./torch_utilities/features.py
 ./torch_utilities/io.py
+./torch_utilities/losses.py
 ./torch_utilities/metrics.py
 ./torch_utilities/model_trainer.py
 ./torch_utilities/modules.py
 ./torch_utilities/pytorch.py
 tests/test_audio.py
 tests/test_augmentation.py
 tests/test_common.py
 tests/test_data_loading.py
+tests/test_features.py
 tests/test_io.py
 tests/test_metrics.py
 tests/test_model_trainer.py
 tests/test_modules.py
 tests/test_pytorch.py
 torch_utilities.egg-info/PKG-INFO
 torch_utilities.egg-info/SOURCES.txt
```

