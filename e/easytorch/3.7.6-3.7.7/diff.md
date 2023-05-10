# Comparing `tmp/easytorch-3.7.6.tar.gz` & `tmp/easytorch-3.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytorch-3.7.6.tar", last modified: Tue Apr 25 18:53:48 2023, max compression
+gzip compressed data, was "easytorch-3.7.7.tar", last modified: Wed May 10 18:11:51 2023, max compression
```

## Comparing `easytorch-3.7.6.tar` & `easytorch-3.7.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:48.936197 easytorch-3.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 18:53:33.000000 easytorch-3.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-25 18:53:48.932197 easytorch-3.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-25 18:53:33.000000 easytorch-3.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:48.932197 easytorch-3.7.6/easytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:48.932197 easytorch-3.7.6/easytorch/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/config/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:48.932197 easytorch-3.7.6/easytorch/data/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/data/datautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/data/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/easytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:48.932197 easytorch-3.7.6/easytorch/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/metrics/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:48.932197 easytorch-3.7.6/easytorch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/utils/ddp_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/utils/tensorutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:48.932197 easytorch-3.7.6/easytorch/vision/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/vision/imageutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/vision/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 18:53:33.000000 easytorch-3.7.6/easytorch/vision/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:48.932197 easytorch-3.7.6/easytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-04-25 18:53:48.000000 easytorch-3.7.6/easytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-25 18:53:48.000000 easytorch-3.7.6/easytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:53:48.000000 easytorch-3.7.6/easytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 18:53:48.000000 easytorch-3.7.6/easytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 18:53:48.000000 easytorch-3.7.6/easytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:53:48.936197 easytorch-3.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-25 18:53:33.000000 easytorch-3.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 18:11:40.000000 easytorch-3.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-10 18:11:51.100686 easytorch-3.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-10 18:11:40.000000 easytorch-3.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.096686 easytorch-3.7.7/easytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/config/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/data/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/data/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12745 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/easytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/metrics/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/utils/ddp_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/utils/tensorutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.100686 easytorch-3.7.7/easytorch/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/vision/imageutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/vision/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-10 18:11:40.000000 easytorch-3.7.7/easytorch/vision/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:11:51.096686 easytorch-3.7.7/easytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 18:11:51.000000 easytorch-3.7.7/easytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:11:51.100686 easytorch-3.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-10 18:11:40.000000 easytorch-3.7.7/setup.py
```

### Comparing `easytorch-3.7.6/LICENSE` & `easytorch-3.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/PKG-INFO` & `easytorch-3.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.6
+Version: 3.7.7
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.6/README.md` & `easytorch-3.7.7/README.md`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/config/__init__.py` & `easytorch-3.7.7/easytorch/config/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/config/state.py` & `easytorch-3.7.7/easytorch/config/state.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/data/data.py` & `easytorch-3.7.7/easytorch/data/data.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/data/datautils.py` & `easytorch-3.7.7/easytorch/data/datautils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/data/multiproc.py` & `easytorch-3.7.7/easytorch/data/multiproc.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/easytorch.py` & `easytorch-3.7.7/easytorch/easytorch.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/metrics/loss.py` & `easytorch-3.7.7/easytorch/metrics/loss.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/metrics/metrics.py` & `easytorch-3.7.7/easytorch/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/runner.py` & `easytorch-3.7.7/easytorch/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,23 +373,24 @@
 
             if not self.conf['use_ddp']:
                 """Plot only in non-ddp mode to maintain consistency"""
                 self.cache[LogKey.TRAIN_LOG].append(running_meter.get())
 
             running_meter.reset()
 
+    def _inference_output_name():
+        return f"{self.conf['save_dir']}{_sep}INFERENCE_{self.conf['RUN-ID']}.csv"
     @_torch.no_grad()
     def inference(self, dataloader):
         self.mode = Phase.INFERENCE
 
         first_model = list(self.nn.keys())[0]
         self.nn[first_model].eval()
 
-        self.cache['output_csv'] = f"{self.conf['save_dir']}{_sep}CHUNK-{self.conf['world_rank']}." \
-                                   f"{self.conf['name']}.csv"
+        self.cache['output_csv'] = self._inference_output_name()
         with open(self.cache['output_csv'], 'w') as fw:
             for i, batch in enumerate(dataloader, 1):
                 self.batch_index = i
                 it = self.iteration(batch)
                 self.save_predictions(dataloader.dataset, it, writer=fw)
                 info(f"{self.conf['name']}, batch {i}/{len(dataloader)} done", self.conf['verbose'])
```

### Comparing `easytorch-3.7.6/easytorch/utils/__init__.py` & `easytorch-3.7.7/easytorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/utils/ddp_check.py` & `easytorch-3.7.7/easytorch/utils/ddp_check.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/utils/tensorutils.py` & `easytorch-3.7.7/easytorch/utils/tensorutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/vision/imageutils.py` & `easytorch-3.7.7/easytorch/vision/imageutils.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/vision/plotter.py` & `easytorch-3.7.7/easytorch/vision/plotter.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch/vision/transforms.py` & `easytorch-3.7.7/easytorch/vision/transforms.py`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/easytorch.egg-info/PKG-INFO` & `easytorch-3.7.7/easytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytorch
-Version: 3.7.6
+Version: 3.7.7
 Summary: Easy Neural Network Experiments with pytorch
 Home-page: https://github.com/sraashis/easytorch
 Author: Aashis Khana1
 Author-email: sraashis@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `easytorch-3.7.6/easytorch.egg-info/SOURCES.txt` & `easytorch-3.7.7/easytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easytorch-3.7.6/setup.py` & `easytorch-3.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     import cv2
 except:
     _requires.append('opencv-contrib-python-headless')
 
 # This call to setup() does all the work
 setup(
     name="easytorch",
-    version="3.7.6",
+    version="3.7.7",
     description="Easy Neural Network Experiments with pytorch",
     long_description=_README,
     long_description_content_type="text/markdown",
     url="https://github.com/sraashis/easytorch",
     author="Aashis Khana1",
     author_email="sraashis@gmail.com",
     license="MIT",
```

