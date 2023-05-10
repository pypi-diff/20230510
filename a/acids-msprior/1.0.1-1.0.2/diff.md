# Comparing `tmp/acids-msprior-1.0.1.tar.gz` & `tmp/acids-msprior-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-msprior-1.0.1.tar", last modified: Wed May 10 14:08:56 2023, max compression
+gzip compressed data, was "acids-msprior-1.0.2.tar", last modified: Wed May 10 14:21:34 2023, max compression
```

## Comparing `acids-msprior-1.0.1.tar` & `acids-msprior-1.0.2.tar`

### file list

```diff
@@ -1,41 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:08:56.051090 acids-msprior-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 14:08:56.051090 acids-msprior-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:08:56.047089 acids-msprior-1.0.1/acids_msprior.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 14:08:56.000000 acids-msprior-1.0.1/acids_msprior.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-10 14:08:56.000000 acids-msprior-1.0.1/acids_msprior.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:08:56.000000 acids-msprior-1.0.1/acids_msprior.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 14:08:56.000000 acids-msprior-1.0.1/acids_msprior.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 14:08:56.000000 acids-msprior-1.0.1/acids_msprior.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 14:08:56.000000 acids-msprior-1.0.1/acids_msprior.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:08:56.047089 acids-msprior-1.0.1/msprior/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:08:56.051090 acids-msprior-1.0.1/msprior/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/configs/decoder_only.gin
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/configs/encoder_decoder.gin
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/configs/encoder_decoder_continuous.gin
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/configs/recurrent.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/scripted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:08:56.051090 acids-msprior-1.0.1/msprior_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior_scripts/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior_scripts/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior_scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior_scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior_scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior_scripts/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/msprior_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:08:56.051090 acids-msprior-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:08:56.051090 acids-msprior-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-10 14:05:43.000000 acids-msprior-1.0.1/tests/test_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.074957 acids-msprior-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 14:21:34.074957 acids-msprior-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.066957 acids-msprior-1.0.2/acids_msprior.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 14:21:34.000000 acids-msprior-1.0.2/acids_msprior.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.070957 acids-msprior-1.0.2/msprior/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.070957 acids-msprior-1.0.2/msprior/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/configs/decoder_only.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/configs/encoder_decoder.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/configs/encoder_decoder_continuous.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/configs/recurrent.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9798 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/scripted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.070957 acids-msprior-1.0.2/msprior_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/msprior_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:21:34.074957 acids-msprior-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:21:34.070957 acids-msprior-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-10 14:18:25.000000 acids-msprior-1.0.2/tests/test_configs.py
```

### Comparing `acids-msprior-1.0.1/PKG-INFO` & `acids-msprior-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.1
+Version: 1.0.2
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.1 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.2 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.1/README.md` & `acids-msprior-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/acids_msprior.egg-info/PKG-INFO` & `acids-msprior-1.0.2/acids_msprior.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.0.1
+Version: 1.0.2
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.1 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.0.2 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.0.1/acids_msprior.egg-info/SOURCES.txt` & `acids-msprior-1.0.2/acids_msprior.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 msprior/utils.py
 msprior/configs/decoder_only.gin
 msprior/configs/encoder_decoder.gin
 msprior/configs/encoder_decoder_continuous.gin
 msprior/configs/recurrent.gin
 msprior_scripts/__init__.py
 msprior_scripts/compact.py
-msprior_scripts/eval.py
 msprior_scripts/export.py
 msprior_scripts/main_cli.py
 msprior_scripts/preprocess.py
-msprior_scripts/tokenize.py
 msprior_scripts/train.py
 tests/__init__.py
 tests/test_attention.py
 tests/test_cache.py
 tests/test_configs.py
```

### Comparing `acids-msprior-1.0.1/msprior/attention.py` & `acids-msprior-1.0.2/msprior/attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior/configs/decoder_only.gin` & `acids-msprior-1.0.2/msprior/configs/decoder_only.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior/configs/encoder_decoder.gin` & `acids-msprior-1.0.2/msprior/configs/encoder_decoder.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior/configs/encoder_decoder_continuous.gin` & `acids-msprior-1.0.2/msprior/configs/encoder_decoder_continuous.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior/dataset.py` & `acids-msprior-1.0.2/msprior/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior/preprocessor.py` & `acids-msprior-1.0.2/msprior/preprocessor.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior/scripted.py` & `acids-msprior-1.0.2/msprior/scripted.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,19 +69,18 @@
                 num_inputs += 1
                 self.encoder_num_tokens = gin.get_bindings(
                     "encoder/attention.Embedding")["num_embeddings"]
                 self.encoder_input_type = "discrete"
             elif isinstance(encoder_embedder(), FeatureEmbedding):
                 if vae_path is not None:
                     self.encoder_input_type = "vae"
-                    self.feature_vae = torch.jit.load(
-                        vae_path).eval()
+                    self.feature_vae = torch.jit.load(vae_path).eval()
                     num_inputs += self.feature_vae.latent_size
                 else:
-                    num_inputs += 163 # TODO: put that somewhere in configuration files
+                    num_inputs += 163  # TODO: put that somewhere in configuration files
                     self.encoder_input_type = "full"
             else:
                 raise ValueError(
                     f"Unknown encoder embedder {encoder_embedder}")
 
             self.encoder_ratio = gin.get_bindings(
                 "decoder/attention.TransformerLayer")["encoder_out_ratio"]
```

### Comparing `acids-msprior-1.0.1/msprior/task.py` & `acids-msprior-1.0.2/msprior/task.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior/utils.py` & `acids-msprior-1.0.2/msprior/utils.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior_scripts/compact.py` & `acids-msprior-1.0.2/msprior_scripts/compact.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior_scripts/export.py` & `acids-msprior-1.0.2/msprior_scripts/export.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior_scripts/main_cli.py` & `acids-msprior-1.0.2/msprior_scripts/main_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import importlib
 import sys
 
 from absl import app
 
-AVAILABLE_SCRIPTS = [
-    'preprocess', 'train', 'export', 'compact', 'eval', 'tokenize'
-]
+AVAILABLE_SCRIPTS = ['preprocess', 'train', 'export', 'compact']
 
 
 def help():
     print(f"""usage: msprior [ {' | '.join(AVAILABLE_SCRIPTS)} ]
 
 positional arguments:
   command     Command to launch with msprior.
@@ -23,8 +21,8 @@
     elif sys.argv[1] not in AVAILABLE_SCRIPTS:
         help()
 
     command = sys.argv[1]
 
     module = importlib.import_module("msprior_scripts." + command)
     sys.argv[0] = module.__name__
-    app.run(module.main)
+    app.run(module.main)
```

### Comparing `acids-msprior-1.0.1/msprior_scripts/preprocess.py` & `acids-msprior-1.0.2/msprior_scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/msprior_scripts/train.py` & `acids-msprior-1.0.2/msprior_scripts/train.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/setup.py` & `acids-msprior-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/tests/test_attention.py` & `acids-msprior-1.0.2/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/tests/test_cache.py` & `acids-msprior-1.0.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.0.1/tests/test_configs.py` & `acids-msprior-1.0.2/tests/test_configs.py`

 * *Files identical despite different names*

