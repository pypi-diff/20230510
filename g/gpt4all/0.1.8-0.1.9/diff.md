# Comparing `tmp/gpt4all-0.1.8-py3-none-win_amd64.whl.zip` & `tmp/gpt4all-0.1.9-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,32 @@
-Zip file size: 9162 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat       76 b- defN 23-May-09 16:44 gpt4all/__init__.py
--rw-rw-rw-  2.0 fat    11187 b- defN 23-May-09 16:44 gpt4all/gpt4all.py
--rw-rw-rw-  2.0 fat     7513 b- defN 23-May-09 16:44 gpt4all/pyllmodel.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-May-09 16:44 tests/__init__.py
--rw-rw-rw-  2.0 fat     1863 b- defN 23-May-09 16:44 tests/test_gpt4all.py
--rw-rw-rw-  2.0 fat     1172 b- defN 23-May-09 16:44 tests/test_pyllmodel.py
--rw-rw-rw-  2.0 fat     1072 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      733 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      845 b- defN 23-May-09 16:45 gpt4all-0.1.8.dist-info/RECORD
-11 files, 24573 bytes uncompressed, 7742 bytes compressed:  68.5%
+Zip file size: 2560445 bytes, number of entries: 30
+-rw-rw-rw-  2.0 fat       76 b- defN 23-May-10 20:02 gpt4all/__init__.py
+-rw-rw-rw-  2.0 fat    11325 b- defN 23-May-10 20:02 gpt4all/gpt4all.py
+-rw-rw-rw-  2.0 fat     7686 b- defN 23-May-10 20:02 gpt4all/pyllmodel.py
+-rw-rw-rw-  2.0 fat     3476 b- defN 23-May-10 20:05 gpt4all/llmodel_DO_NOT_MODIFY/common.h
+-rw-rw-rw-  2.0 fat     2378 b- defN 23-May-10 20:05 gpt4all/llmodel_DO_NOT_MODIFY/ggml-cuda.h
+-rw-rw-rw-  2.0 fat      663 b- defN 23-May-10 20:05 gpt4all/llmodel_DO_NOT_MODIFY/ggml-opencl.h
+-rw-rw-rw-  2.0 fat    30753 b- defN 23-May-10 20:05 gpt4all/llmodel_DO_NOT_MODIFY/ggml.h
+-rw-rw-rw-  2.0 fat     1006 b- defN 23-May-10 20:02 gpt4all/llmodel_DO_NOT_MODIFY/gptj.h
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-10 20:05 gpt4all/llmodel_DO_NOT_MODIFY/llama.h
+-rw-rw-rw-  2.0 fat    12387 b- defN 23-May-10 20:05 gpt4all/llmodel_DO_NOT_MODIFY/llama_util.h
+-rw-rw-rw-  2.0 fat     1042 b- defN 23-May-10 20:02 gpt4all/llmodel_DO_NOT_MODIFY/llamamodel.h
+-rw-rw-rw-  2.0 fat     1800 b- defN 23-May-10 20:02 gpt4all/llmodel_DO_NOT_MODIFY/llmodel.h
+-rw-rw-rw-  2.0 fat     6149 b- defN 23-May-10 20:02 gpt4all/llmodel_DO_NOT_MODIFY/llmodel_c.h
+-rw-rw-rw-  2.0 fat      998 b- defN 23-May-10 20:02 gpt4all/llmodel_DO_NOT_MODIFY/mpt.h
+-rw-rw-rw-  2.0 fat     2410 b- defN 23-May-10 20:02 gpt4all/llmodel_DO_NOT_MODIFY/utils.h
+-rw-rw-rw-  2.0 fat    32768 b- defN 22-Dec-08 23:38 gpt4all/llmodel_DO_NOT_MODIFY/build/libatomic-1.dll
+-rw-rw-rw-  2.0 fat   101376 b- defN 22-Dec-08 23:38 gpt4all/llmodel_DO_NOT_MODIFY/build/libgcc_s_seh-1.dll
+-rw-rw-rw-  2.0 fat  3094016 b- defN 22-Dec-08 23:38 gpt4all/llmodel_DO_NOT_MODIFY/build/libgfortran-5.dll
+-rw-rw-rw-  2.0 fat   258048 b- defN 22-Dec-08 23:38 gpt4all/llmodel_DO_NOT_MODIFY/build/libgomp-1.dll
+-rw-rw-rw-  2.0 fat   459057 b- defN 23-May-10 20:06 gpt4all/llmodel_DO_NOT_MODIFY/build/libllama.dll
+-rw-rw-rw-  2.0 fat   582869 b- defN 23-May-10 20:06 gpt4all/llmodel_DO_NOT_MODIFY/build/libllmodel.dll
+-rw-rw-rw-  2.0 fat   365568 b- defN 22-Dec-08 23:38 gpt4all/llmodel_DO_NOT_MODIFY/build/libquadmath-0.dll
+-rw-rw-rw-  2.0 fat    16896 b- defN 22-Dec-08 23:38 gpt4all/llmodel_DO_NOT_MODIFY/build/libssp-0.dll
+-rw-rw-rw-  2.0 fat  2020352 b- defN 22-Dec-08 23:38 gpt4all/llmodel_DO_NOT_MODIFY/build/libstdc++-6.dll
+-rw-rw-rw-  2.0 fat    54784 b- defN 22-Dec-08 23:38 gpt4all/llmodel_DO_NOT_MODIFY/build/libwinpthread-1.dll
+-rw-rw-rw-  2.0 fat     1072 b- defN 23-May-10 20:06 gpt4all-0.1.9.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      733 b- defN 23-May-10 20:06 gpt4all-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-May-10 20:06 gpt4all-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-10 20:06 gpt4all-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2865 b- defN 23-May-10 20:06 gpt4all-0.1.9.dist-info/RECORD
+30 files, 7072669 bytes uncompressed, 2555745 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -3,32 +3,89 @@
 
 Filename: gpt4all/gpt4all.py
 Comment: 
 
 Filename: gpt4all/pyllmodel.py
 Comment: 
 
-Filename: tests/__init__.py
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/common.h
 Comment: 
 
-Filename: tests/test_gpt4all.py
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/ggml-cuda.h
 Comment: 
 
-Filename: tests/test_pyllmodel.py
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/ggml-opencl.h
 Comment: 
 
-Filename: gpt4all-0.1.8.dist-info/LICENSE.txt
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/ggml.h
 Comment: 
 
-Filename: gpt4all-0.1.8.dist-info/METADATA
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/gptj.h
 Comment: 
 
-Filename: gpt4all-0.1.8.dist-info/WHEEL
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/llama.h
 Comment: 
 
-Filename: gpt4all-0.1.8.dist-info/top_level.txt
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/llama_util.h
 Comment: 
 
-Filename: gpt4all-0.1.8.dist-info/RECORD
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/llamamodel.h
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/llmodel.h
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/llmodel_c.h
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/mpt.h
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/utils.h
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libatomic-1.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libgcc_s_seh-1.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libgfortran-5.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libgomp-1.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libllama.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libllmodel.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libquadmath-0.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libssp-0.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libstdc++-6.dll
+Comment: 
+
+Filename: gpt4all/llmodel_DO_NOT_MODIFY/build/libwinpthread-1.dll
+Comment: 
+
+Filename: gpt4all-0.1.9.dist-info/LICENSE.txt
+Comment: 
+
+Filename: gpt4all-0.1.9.dist-info/METADATA
+Comment: 
+
+Filename: gpt4all-0.1.9.dist-info/WHEEL
+Comment: 
+
+Filename: gpt4all-0.1.9.dist-info/top_level.txt
+Comment: 
+
+Filename: gpt4all-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gpt4all/gpt4all.py

```diff
@@ -8,15 +8,15 @@
 
 import requests
 from tqdm import tqdm
 
 from . import pyllmodel
 
 # TODO: move to config
-DEFAULT_MODEL_DIRECTORY = os.path.join(str(Path.home()), ".cache", "gpt4all")
+DEFAULT_MODEL_DIRECTORY = os.path.join(str(Path.home()), ".cache", "gpt4all").replace("\\", "\\\\")
 
 class GPT4All():
     """Python API for retrieving and interacting with GPT4All models
     
     Attribuies:
         model: Pointer to underlying C model.
     """
@@ -83,17 +83,19 @@
             model_path = DEFAULT_MODEL_DIRECTORY
             if not os.path.exists(DEFAULT_MODEL_DIRECTORY):
                 try:
                     os.makedirs(DEFAULT_MODEL_DIRECTORY)
                 except:
                     raise ValueError("Failed to create model download directory at ~/.cache/gpt4all/. \
                     Please specify download_dir.")
+        else:
+            model_path = model_path.replace("\\", "\\\\")
 
         if os.path.exists(model_path):
-            model_dest = os.path.join(model_path, model_filename)
+            model_dest = os.path.join(model_path, model_filename).replace("\\", "\\\\")
             if os.path.exists(model_dest):
                 print("Found model file.")
                 return model_dest
 
             # If model file does not exist, download
             elif allow_download: 
                 # Make sure valid model filename before attempting download
@@ -112,15 +114,15 @@
         
     @staticmethod
     def download_model(model_filename, model_path):
         def get_download_url(model_filename):
             return f"https://gpt4all.io/models/{model_filename}"
     
         # Download model
-        download_path = os.path.join(model_path, model_filename)
+        download_path = os.path.join(model_path, model_filename).replace("\\", "\\\\")
         download_url = get_download_url(model_filename)
 
         response = requests.get(download_url, stream=True)
         total_size_in_bytes = int(response.headers.get("content-length", 0))
         block_size = 1048576  # 1 MB
         progress_bar = tqdm(total=total_size_in_bytes, unit="iB", unit_scale=True)
         with open(download_path, "wb") as file:
@@ -174,15 +176,14 @@
                 as "assistant". Right now, only one choice is returned by model.
             
         """
        
         full_prompt = self._build_prompt(messages, 
                                         default_prompt_header=default_prompt_header, 
                                         default_prompt_footer=default_prompt_footer)
-
         if verbose:
             print(full_prompt)
 
         response = self.model.generate(full_prompt)
 
         if verbose:
             print(response)
```

## gpt4all/pyllmodel.py

```diff
@@ -3,35 +3,39 @@
 import ctypes
 import os
 import platform
 import re
 import sys
 
 # TODO: provide a config file to make this more robust
-LLMODEL_PATH = "llmodel_DO_NOT_MODIFY/build/"
+LLMODEL_PATH = os.path.join("llmodel_DO_NOT_MODIFY", "build").replace("\\", "\\\\")
 
 def load_llmodel_library():
     system = platform.system()
 
     def get_c_shared_lib_extension():
         if system == "Darwin":
             return "dylib"
         elif system == "Linux":
             return "so"
         elif system == "Windows":
             return "dll"
         else:
             raise Exception("Operating System not supported")
-        
+
     c_lib_ext = get_c_shared_lib_extension()
-    
+
     llmodel_file = "libllmodel" + '.' + c_lib_ext
     llama_file = "libllama" + '.' + c_lib_ext
-    llama_dir = str(pkg_resources.resource_filename('gpt4all', LLMODEL_PATH + llama_file))
-    llmodel_dir = str(pkg_resources.resource_filename('gpt4all', LLMODEL_PATH + llmodel_file))
+    llama_dir = str(pkg_resources.resource_filename('gpt4all', os.path.join(LLMODEL_PATH, llama_file)))
+    llmodel_dir = str(pkg_resources.resource_filename('gpt4all', os.path.join(LLMODEL_PATH, llmodel_file)))
+
+    # For windows
+    llama_dir = llama_dir.replace("\\", "\\\\")
+    llmodel_dir = llmodel_dir.replace("\\", "\\\\")
 
     llama_lib = ctypes.CDLL(llama_dir, mode=ctypes.RTLD_GLOBAL)
     llmodel_lib = ctypes.CDLL(llmodel_dir)
 
     return llmodel_lib, llama_lib
 
 
@@ -70,15 +74,14 @@
 llmodel.llmodel_prompt.argtypes = [ctypes.c_void_p, 
                                    ctypes.c_char_p, 
                                    ResponseCallback, 
                                    ResponseCallback, 
                                    RecalculateCallback, 
                                    ctypes.POINTER(LLModelPromptContext)]
 
-
 class LLModel:
     """
     Base class and universal wrapper for GPT4All language models
     built around llmodel C-API.
 
     Attributes
     ----------
```

## Comparing `gpt4all-0.1.8.dist-info/LICENSE.txt` & `gpt4all-0.1.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `gpt4all-0.1.8.dist-info/METADATA` & `gpt4all-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt4all
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python bindings for GPT4All
 Home-page: https://pypi.org/project/gpt4all/
 Author: Richard Guo
 Author-email: richard@nomic.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

