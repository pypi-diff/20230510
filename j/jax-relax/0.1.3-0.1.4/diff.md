# Comparing `tmp/jax-relax-0.1.3.tar.gz` & `tmp/jax-relax-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-relax-0.1.3.tar", last modified: Wed May  3 01:54:30 2023, max compression
+gzip compressed data, was "jax-relax-0.1.4.tar", last modified: Wed May 10 18:35:03 2023, max compression
```

## Comparing `jax-relax-0.1.3.tar` & `jax-relax-0.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.571084 jax-relax-0.1.3/
--rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-01-17 02:27:26.000000 jax-relax-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 birk      (1000) birk      (1000)    11558 2023-01-17 02:27:26.000000 jax-relax-0.1.3/LICENSE
--rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-01-17 02:27:26.000000 jax-relax-0.1.3/MANIFEST.in
--rw-r--r--   0 birk      (1000) birk      (1000)     3355 2023-05-03 01:54:30.571084 jax-relax-0.1.3/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)     2515 2023-05-03 01:52:41.000000 jax-relax-0.1.3/README.md
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.561084 jax-relax-0.1.3/jax_relax.egg-info/
--rw-r--r--   0 birk      (1000) birk      (1000)     3355 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/PKG-INFO
--rw-r--r--   0 birk      (1000) birk      (1000)      820 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/SOURCES.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/dependency_links.txt
--rw-r--r--   0 birk      (1000) birk      (1000)       32 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/entry_points.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-01-17 02:38:00.000000 jax-relax-0.1.3/jax_relax.egg-info/not-zip-safe
--rw-r--r--   0 birk      (1000) birk      (1000)      199 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/requires.txt
--rw-r--r--   0 birk      (1000) birk      (1000)        6 2023-05-03 01:54:30.000000 jax-relax-0.1.3/jax_relax.egg-info/top_level.txt
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.571084 jax-relax-0.1.3/relax/
--rw-r--r--   0 birk      (1000) birk      (1000)       21 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3855 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/_ckpt_manager.py
--rw-r--r--   0 birk      (1000) birk      (1000)    79877 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/_modidx.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.571084 jax-relax-0.1.3/relax/data/
--rw-r--r--   0 birk      (1000) birk      (1000)      117 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/data/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7842 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/data/loader.py
--rw-r--r--   0 birk      (1000) birk      (1000)    17786 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/data/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9776 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/data/scm.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6199 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/docs.py
--rw-r--r--   0 birk      (1000) birk      (1000)    15503 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/evaluate.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1296 2023-04-19 16:19:35.000000 jax-relax-0.1.3/relax/import_essentials.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1985 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/logger.py
-drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-03 01:54:30.571084 jax-relax-0.1.3/relax/methods/
--rw-r--r--   0 birk      (1000) birk      (1000)      196 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/__init__.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1959 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/base.py
--rw-r--r--   0 birk      (1000) birk      (1000)    11115 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/cchvae.py
--rw-r--r--   0 birk      (1000) birk      (1000)    14082 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/clue.py
--rw-r--r--   0 birk      (1000) birk      (1000)    12537 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/counternet.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6298 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/diverse.py
--rw-r--r--   0 birk      (1000) birk      (1000)     9273 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/proto.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7548 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/sphere.py
--rw-r--r--   0 birk      (1000) birk      (1000)    11112 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/vaecf.py
--rw-r--r--   0 birk      (1000) birk      (1000)     3958 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/methods/vanilla.py
--rw-r--r--   0 birk      (1000) birk      (1000)     7736 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/module.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4797 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/plots.py
--rw-r--r--   0 birk      (1000) birk      (1000)     4788 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/trainer.py
--rw-r--r--   0 birk      (1000) birk      (1000)     6738 2023-05-03 01:54:10.000000 jax-relax-0.1.3/relax/utils.py
--rw-r--r--   0 birk      (1000) birk      (1000)     1112 2023-05-03 01:53:37.000000 jax-relax-0.1.3/settings.ini
--rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-05-03 01:54:30.571084 jax-relax-0.1.3/setup.cfg
--rw-r--r--   0 birk      (1000) birk      (1000)     2598 2023-01-17 02:27:26.000000 jax-relax-0.1.3/setup.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/
+-rw-r--r--   0 birk      (1000) birk      (1000)     2381 2023-01-17 02:27:26.000000 jax-relax-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 birk      (1000) birk      (1000)    11558 2023-01-17 02:27:26.000000 jax-relax-0.1.4/LICENSE
+-rw-r--r--   0 birk      (1000) birk      (1000)      116 2023-01-17 02:27:26.000000 jax-relax-0.1.4/MANIFEST.in
+-rw-r--r--   0 birk      (1000) birk      (1000)     3356 2023-05-10 18:35:03.853624 jax-relax-0.1.4/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)     2515 2023-05-04 04:04:49.000000 jax-relax-0.1.4/README.md
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/jax_relax.egg-info/
+-rw-r--r--   0 birk      (1000) birk      (1000)     3356 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/PKG-INFO
+-rw-r--r--   0 birk      (1000) birk      (1000)      820 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/SOURCES.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/dependency_links.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)       32 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/entry_points.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        1 2023-01-17 02:38:00.000000 jax-relax-0.1.4/jax_relax.egg-info/not-zip-safe
+-rw-r--r--   0 birk      (1000) birk      (1000)      208 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/requires.txt
+-rw-r--r--   0 birk      (1000) birk      (1000)        6 2023-05-10 18:35:03.000000 jax-relax-0.1.4/jax_relax.egg-info/top_level.txt
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/relax/
+-rw-r--r--   0 birk      (1000) birk      (1000)       21 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3855 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/_ckpt_manager.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    83777 2023-05-10 18:28:51.000000 jax-relax-0.1.4/relax/_modidx.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/relax/data/
+-rw-r--r--   0 birk      (1000) birk      (1000)      117 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/data/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7842 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/data/loader.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    19263 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/data/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9776 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/data/scm.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6199 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/docs.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    19678 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/evaluate.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1341 2023-05-03 15:57:46.000000 jax-relax-0.1.4/relax/import_essentials.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1985 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/logger.py
+drwxr-xr-x   0 birk      (1000) birk      (1000)        0 2023-05-10 18:35:03.853624 jax-relax-0.1.4/relax/methods/
+-rw-r--r--   0 birk      (1000) birk      (1000)      361 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/__init__.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     2319 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/base.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    11533 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/cchvae.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    13916 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/clue.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    12640 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/counternet.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     6125 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/diverse.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     9245 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/proto.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7204 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/sphere.py
+-rw-r--r--   0 birk      (1000) birk      (1000)    11619 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/vaecf.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     3699 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/methods/vanilla.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     7736 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/module.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4797 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/plots.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     4788 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/trainer.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     8433 2023-05-10 18:24:18.000000 jax-relax-0.1.4/relax/utils.py
+-rw-r--r--   0 birk      (1000) birk      (1000)     1159 2023-05-10 18:24:07.000000 jax-relax-0.1.4/settings.ini
+-rw-r--r--   0 birk      (1000) birk      (1000)       38 2023-05-10 18:35:03.853624 jax-relax-0.1.4/setup.cfg
+-rw-r--r--   0 birk      (1000) birk      (1000)     2603 2023-05-03 15:57:46.000000 jax-relax-0.1.4/setup.py
```

### Comparing `jax-relax-0.1.3/CONTRIBUTING.md` & `jax-relax-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/LICENSE` & `jax-relax-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/PKG-INFO` & `jax-relax-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jax-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/relax/tree/master/
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: Jax,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # ReLax
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `jax-relax-0.1.3/README.md` & `jax-relax-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/jax_relax.egg-info/PKG-INFO` & `jax-relax-0.1.4/jax_relax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: jax-relax
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jax-based Recourse Explanation Library
 Home-page: https://github.com/birkhoffg/relax/tree/master/
 Author: BirkhoffG
 Author-email: 26811230+BirkhoffG@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: Jax,Recourse,Explanation,Interpretability,Machine Learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # ReLax
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
```

### Comparing `jax-relax-0.1.3/jax_relax.egg-info/SOURCES.txt` & `jax-relax-0.1.4/jax_relax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/_ckpt_manager.py` & `jax-relax-0.1.4/relax/_ckpt_manager.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/_modidx.py` & `jax-relax-0.1.4/relax/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,49 +209,71 @@
                             'relax.docs._return_mdlist': ('docs.html#_return_mdlist', 'relax/docs.py'),
                             'relax.docs._show_param': ('docs.html#_show_param', 'relax/docs.py'),
                             'relax.docs._show_params_return': ('docs.html#_show_params_return', 'relax/docs.py')},
             'relax.evaluate': { 'relax.evaluate.BaseEvalMetrics': ('evaluate.html#baseevalmetrics', 'relax/evaluate.py'),
                                 'relax.evaluate.BaseEvalMetrics.__call__': ('evaluate.html#baseevalmetrics.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate.BaseEvalMetrics.__init__': ('evaluate.html#baseevalmetrics.__init__', 'relax/evaluate.py'),
                                 'relax.evaluate.BaseEvalMetrics.__str__': ('evaluate.html#baseevalmetrics.__str__', 'relax/evaluate.py'),
+                                'relax.evaluate.BaseGenerationStrategy': ('evaluate.html#basegenerationstrategy', 'relax/evaluate.py'),
+                                'relax.evaluate.BaseGenerationStrategy.__call__': ( 'evaluate.html#basegenerationstrategy.__call__',
+                                                                                    'relax/evaluate.py'),
                                 'relax.evaluate.Explanation': ('evaluate.html#explanation', 'relax/evaluate.py'),
                                 'relax.evaluate.Explanation.__post_init__': ( 'evaluate.html#explanation.__post_init__',
                                                                               'relax/evaluate.py'),
+                                'relax.evaluate.IterativeGenerationStrategy': ( 'evaluate.html#iterativegenerationstrategy',
+                                                                                'relax/evaluate.py'),
+                                'relax.evaluate.IterativeGenerationStrategy.__call__': ( 'evaluate.html#iterativegenerationstrategy.__call__',
+                                                                                         'relax/evaluate.py'),
                                 'relax.evaluate.ManifoldDist': ('evaluate.html#manifolddist', 'relax/evaluate.py'),
                                 'relax.evaluate.ManifoldDist.__call__': ('evaluate.html#manifolddist.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate.ManifoldDist.__init__': ('evaluate.html#manifolddist.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.PmapGenerationStrategy': ('evaluate.html#pmapgenerationstrategy', 'relax/evaluate.py'),
+                                'relax.evaluate.PmapGenerationStrategy.__call__': ( 'evaluate.html#pmapgenerationstrategy.__call__',
+                                                                                    'relax/evaluate.py'),
+                                'relax.evaluate.PmapGenerationStrategy.__init__': ( 'evaluate.html#pmapgenerationstrategy.__init__',
+                                                                                    'relax/evaluate.py'),
                                 'relax.evaluate.PredictiveAccuracy': ('evaluate.html#predictiveaccuracy', 'relax/evaluate.py'),
                                 'relax.evaluate.PredictiveAccuracy.__call__': ( 'evaluate.html#predictiveaccuracy.__call__',
                                                                                 'relax/evaluate.py'),
                                 'relax.evaluate.PredictiveAccuracy.__init__': ( 'evaluate.html#predictiveaccuracy.__init__',
                                                                                 'relax/evaluate.py'),
                                 'relax.evaluate.Proximity': ('evaluate.html#proximity', 'relax/evaluate.py'),
                                 'relax.evaluate.Proximity.__call__': ('evaluate.html#proximity.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate.Proximity.__init__': ('evaluate.html#proximity.__init__', 'relax/evaluate.py'),
                                 'relax.evaluate.Runtime': ('evaluate.html#runtime', 'relax/evaluate.py'),
                                 'relax.evaluate.Runtime.__call__': ('evaluate.html#runtime.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate.Runtime.__init__': ('evaluate.html#runtime.__init__', 'relax/evaluate.py'),
                                 'relax.evaluate.Sparsity': ('evaluate.html#sparsity', 'relax/evaluate.py'),
                                 'relax.evaluate.Sparsity.__call__': ('evaluate.html#sparsity.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate.Sparsity.__init__': ('evaluate.html#sparsity.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.StrategyFactory': ('evaluate.html#strategyfactory', 'relax/evaluate.py'),
+                                'relax.evaluate.StrategyFactory.__init__': ('evaluate.html#strategyfactory.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.StrategyFactory.get_default_strategy': ( 'evaluate.html#strategyfactory.get_default_strategy',
+                                                                                         'relax/evaluate.py'),
+                                'relax.evaluate.StrategyFactory.get_strategy': ( 'evaluate.html#strategyfactory.get_strategy',
+                                                                                 'relax/evaluate.py'),
                                 'relax.evaluate.Validity': ('evaluate.html#validity', 'relax/evaluate.py'),
                                 'relax.evaluate.Validity.__call__': ('evaluate.html#validity.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate.Validity.__init__': ('evaluate.html#validity.__init__', 'relax/evaluate.py'),
+                                'relax.evaluate.VmapGenerationStrategy': ('evaluate.html#vmapgenerationstrategy', 'relax/evaluate.py'),
+                                'relax.evaluate.VmapGenerationStrategy.__call__': ( 'evaluate.html#vmapgenerationstrategy.__call__',
+                                                                                    'relax/evaluate.py'),
                                 'relax.evaluate._AuxPredFn': ('evaluate.html#_auxpredfn', 'relax/evaluate.py'),
                                 'relax.evaluate._AuxPredFn.__call__': ('evaluate.html#_auxpredfn.__call__', 'relax/evaluate.py'),
                                 'relax.evaluate._AuxPredFn.__init__': ('evaluate.html#_auxpredfn.__init__', 'relax/evaluate.py'),
                                 'relax.evaluate._check_aux_pred_fn_args': ('evaluate.html#_check_aux_pred_fn_args', 'relax/evaluate.py'),
                                 'relax.evaluate._check_pred_fn': ('evaluate.html#_check_pred_fn', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_acc': ('evaluate.html#_compute_acc', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_manifold_dist': ('evaluate.html#_compute_manifold_dist', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_proximity': ('evaluate.html#_compute_proximity', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_spar': ('evaluate.html#_compute_spar', 'relax/evaluate.py'),
                                 'relax.evaluate._compute_val': ('evaluate.html#_compute_val', 'relax/evaluate.py'),
                                 'relax.evaluate._create_second_order_cfs': ('evaluate.html#_create_second_order_cfs', 'relax/evaluate.py'),
                                 'relax.evaluate._get_metric': ('evaluate.html#_get_metric', 'relax/evaluate.py'),
+                                'relax.evaluate._pad_divisible_X': ('evaluate.html#_pad_divisible_x', 'relax/evaluate.py'),
                                 'relax.evaluate._prepare_module': ('evaluate.html#_prepare_module', 'relax/evaluate.py'),
                                 'relax.evaluate._train_parametric_module': ('evaluate.html#_train_parametric_module', 'relax/evaluate.py'),
                                 'relax.evaluate._validate_configs': ('evaluate.html#_validate_configs', 'relax/evaluate.py'),
                                 'relax.evaluate.benchmark_cfs': ('evaluate.html#benchmark_cfs', 'relax/evaluate.py'),
                                 'relax.evaluate.compute_so_proximity': ('evaluate.html#compute_so_proximity', 'relax/evaluate.py'),
                                 'relax.evaluate.compute_so_sparsity': ('evaluate.html#compute_so_sparsity', 'relax/evaluate.py'),
                                 'relax.evaluate.compute_so_validity': ('evaluate.html#compute_so_validity', 'relax/evaluate.py'),
@@ -272,14 +294,16 @@
                               'relax.logger.TensorboardLogger.on_epoch_started': ( 'logger.html#tensorboardlogger.on_epoch_started',
                                                                                    'relax/logger.py'),
                               'relax.logger.TensorboardLogger.save_hyperparams': ( 'logger.html#tensorboardlogger.save_hyperparams',
                                                                                    'relax/logger.py')},
             'relax.methods.base': { 'relax.methods.base.BaseCFModule': ('methods.base.html#basecfmodule', 'relax/methods/base.py'),
                                     'relax.methods.base.BaseCFModule.data_module': ( 'methods.base.html#basecfmodule.data_module',
                                                                                      'relax/methods/base.py'),
+                                    'relax.methods.base.BaseCFModule.generate_cf': ( 'methods.base.html#basecfmodule.generate_cf',
+                                                                                     'relax/methods/base.py'),
                                     'relax.methods.base.BaseCFModule.generate_cfs': ( 'methods.base.html#basecfmodule.generate_cfs',
                                                                                       'relax/methods/base.py'),
                                     'relax.methods.base.BaseCFModule.hook_data_module': ( 'methods.base.html#basecfmodule.hook_data_module',
                                                                                           'relax/methods/base.py'),
                                     'relax.methods.base.BaseCFModule.name': ( 'methods.base.html#basecfmodule.name',
                                                                               'relax/methods/base.py'),
                                     'relax.methods.base.BaseParametricCFModule': ( 'methods.base.html#baseparametriccfmodule',
@@ -293,14 +317,16 @@
                                     'relax.methods.base.BasePredFnCFModule.pred_fn': ( 'methods.base.html#basepredfncfmodule.pred_fn',
                                                                                        'relax/methods/base.py')},
             'relax.methods.cchvae': { 'relax.methods.cchvae.CCHVAE': ('methods/cchvae.html#cchvae', 'relax/methods/cchvae.py'),
                                       'relax.methods.cchvae.CCHVAE.__init__': ( 'methods/cchvae.html#cchvae.__init__',
                                                                                 'relax/methods/cchvae.py'),
                                       'relax.methods.cchvae.CCHVAE._is_module_trained': ( 'methods/cchvae.html#cchvae._is_module_trained',
                                                                                           'relax/methods/cchvae.py'),
+                                      'relax.methods.cchvae.CCHVAE.generate_cf': ( 'methods/cchvae.html#cchvae.generate_cf',
+                                                                                   'relax/methods/cchvae.py'),
                                       'relax.methods.cchvae.CCHVAE.generate_cfs': ( 'methods/cchvae.html#cchvae.generate_cfs',
                                                                                     'relax/methods/cchvae.py'),
                                       'relax.methods.cchvae.CCHVAE.train': ('methods/cchvae.html#cchvae.train', 'relax/methods/cchvae.py'),
                                       'relax.methods.cchvae.CCHVAEConfigs': ( 'methods/cchvae.html#cchvaeconfigs',
                                                                               'relax/methods/cchvae.py'),
                                       'relax.methods.cchvae.CHVAE': ('methods/cchvae.html#chvae', 'relax/methods/cchvae.py'),
                                       'relax.methods.cchvae.CHVAE.__init__': ( 'methods/cchvae.html#chvae.__init__',
@@ -383,14 +409,16 @@
                                     'relax.methods.clue.kl_divergence': ('methods/clue.html#kl_divergence', 'relax/methods/clue.py')},
             'relax.methods.counternet': { 'relax.methods.counternet.CounterNet': ( 'methods/counternet.html#counternet',
                                                                                    'relax/methods/counternet.py'),
                                           'relax.methods.counternet.CounterNet.__init__': ( 'methods/counternet.html#counternet.__init__',
                                                                                             'relax/methods/counternet.py'),
                                           'relax.methods.counternet.CounterNet._is_module_trained': ( 'methods/counternet.html#counternet._is_module_trained',
                                                                                                       'relax/methods/counternet.py'),
+                                          'relax.methods.counternet.CounterNet.generate_cf': ( 'methods/counternet.html#counternet.generate_cf',
+                                                                                               'relax/methods/counternet.py'),
                                           'relax.methods.counternet.CounterNet.generate_cfs': ( 'methods/counternet.html#counternet.generate_cfs',
                                                                                                 'relax/methods/counternet.py'),
                                           'relax.methods.counternet.CounterNet.pred_fn': ( 'methods/counternet.html#counternet.pred_fn',
                                                                                            'relax/methods/counternet.py'),
                                           'relax.methods.counternet.CounterNet.train': ( 'methods/counternet.html#counternet.train',
                                                                                          'relax/methods/counternet.py'),
                                           'relax.methods.counternet.CounterNetConfigs': ( 'methods/counternet.html#counternetconfigs',
@@ -523,14 +551,16 @@
                                                                                'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.Encoder.__init__': ( 'methods/vaecf.html#encoder.__init__',
                                                                                'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.VAECF': ('methods/vaecf.html#vaecf', 'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.VAECF.__init__': ('methods/vaecf.html#vaecf.__init__', 'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.VAECF._is_module_trained': ( 'methods/vaecf.html#vaecf._is_module_trained',
                                                                                        'relax/methods/vaecf.py'),
+                                     'relax.methods.vaecf.VAECF.generate_cf': ( 'methods/vaecf.html#vaecf.generate_cf',
+                                                                                'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.VAECF.generate_cfs': ( 'methods/vaecf.html#vaecf.generate_cfs',
                                                                                  'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.VAECF.train': ('methods/vaecf.html#vaecf.train', 'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.VAECFConfigs': ('methods/vaecf.html#vaecfconfigs', 'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.VAECFModule': ('methods/vaecf.html#vaecfmodule', 'relax/methods/vaecf.py'),
                                      'relax.methods.vaecf.VAECFModule.__init__': ( 'methods/vaecf.html#vaecfmodule.__init__',
                                                                                    'relax/methods/vaecf.py'),
@@ -628,15 +658,17 @@
                                'relax.trainer.train_model_with_states': ('learning.html#train_model_with_states', 'relax/trainer.py')},
             'relax.utils': { 'relax.utils.Config': ('utils.html#config', 'relax/utils.py'),
                              'relax.utils.Config.default': ('utils.html#config.default', 'relax/utils.py'),
                              'relax.utils.ParserMarkdownRenderer': ('utils.html#parsermarkdownrenderer', 'relax/utils.py'),
                              'relax.utils.ParserMarkdownRenderer.__init__': ( 'utils.html#parsermarkdownrenderer.__init__',
                                                                               'relax/utils.py'),
                              'relax.utils._docment_parser': ('utils.html#_docment_parser', 'relax/utils.py'),
+                             'relax.utils._reshape_x': ('utils.html#_reshape_x', 'relax/utils.py'),
                              'relax.utils.accuracy': ('utils.html#accuracy', 'relax/utils.py'),
+                             'relax.utils.auto_reshaping': ('utils.html#auto_reshaping', 'relax/utils.py'),
                              'relax.utils.binary_cross_entropy': ('utils.html#binary_cross_entropy', 'relax/utils.py'),
                              'relax.utils.cat_normalize': ('utils.html#cat_normalize', 'relax/utils.py'),
                              'relax.utils.check_cat_info': ('utils.html#check_cat_info', 'relax/utils.py'),
                              'relax.utils.dist': ('utils.html#dist', 'relax/utils.py'),
                              'relax.utils.get_config': ('utils.html#get_config', 'relax/utils.py'),
                              'relax.utils.grad_update': ('utils.html#grad_update', 'relax/utils.py'),
                              'relax.utils.init_net_opt': ('utils.html#init_net_opt', 'relax/utils.py'),
```

### Comparing `jax-relax-0.1.3/relax/data/loader.py` & `jax-relax-0.1.4/relax/data/loader.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/data/module.py` & `jax-relax-0.1.4/relax/data/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -463,14 +463,58 @@
     'heloc': {
         'data': 'assets/data/s_home.csv',
         'conf': 'assets/configs/data_configs/home.json'
     },
     'oulad': {
         'data': 'assets/data/s_student.csv',
         'conf': 'assets/configs/data_configs/student.json'
+    },
+    'credit': {
+        'data': 'assets/data/extra/s_credit_card.csv',
+        'conf': 'assets/configs/data_configs/credit_card.json'
+    },
+    'cancer': {
+        'data': 'assets/data/extra/s_breast_cancer.csv',
+        'conf': 'assets/configs/data_configs/breast_cancer.json'
+    },
+    'student_performance': {
+        'data': 'assets/data/extra/s_student_performance.csv',
+        'conf': 'assets/configs/data_configs/student_performance.json'
+    },
+    'titanic': {
+        'data': 'assets/data/extra/s_titanic.csv',
+        'conf': 'assets/configs/data_configs/titanic.json'
+    },
+    'german': {
+        'data': 'assets/data/extra/s_german_credit.csv',
+        'conf': 'assets/configs/data_configs/german_credit.json'
+    },
+    'spam': {
+        'data': 'assets/data/s_spam.csv',
+        'conf': 'assets/configs/data_configs/spam.json'
+    },
+    'ozone': {
+        'data': 'assets/data/s_ozone.csv',
+        'conf': 'assets/configs/data_configs/ozone.json'
+    },
+    'qsar': {
+        'data': 'assets/data/s_qsar.csv',
+        'conf': 'assets/configs/data_configs/qsar.json'
+    },
+    'bioresponse': {
+        'data': 'assets/data/s_bioresponse.csv',
+        'conf': 'assets/configs/data_configs/bioresponse.json'
+    },
+    'churn': {
+        'data': 'assets/data/s_churn.csv',
+        'conf': 'assets/configs/data_configs/churn.json'
+    },
+    'road': {
+        'data': 'assets/data/s_road.csv',
+        'conf': 'assets/configs/data_configs/road.json'
     }
 }
 
 # %% ../../nbs/01_data.module.ipynb 48
 def _validate_dataname(data_name: str):
     if data_name not in DEFAULT_DATA_CONFIGS.keys():
         raise ValueError(f'`data_name` must be one of {DEFAULT_DATA_CONFIGS.keys()}, '
@@ -496,14 +540,15 @@
     # create new dir
     data_dir = Path(os.getcwd()) / "cf_data"
     if not data_dir.exists():
         os.makedirs(data_dir)
     data_path = data_dir / f'{data_name}.csv'
     conf_path = data_dir / f'{data_name}.json'
 
+
     # download data/configs
     if not data_path.is_file():
         urlretrieve(data_url, data_path)    
     if not conf_path.is_file():
         urlretrieve(conf_url, conf_path)
 
     # read config
```

### Comparing `jax-relax-0.1.3/relax/data/scm.py` & `jax-relax-0.1.4/relax/data/scm.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/docs.py` & `jax-relax-0.1.4/relax/docs.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/evaluate.py` & `jax-relax-0.1.4/relax/evaluate.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 from .methods.base import BaseCFModule, BaseParametricCFModule, BasePredFnCFModule
 from .methods.counternet import CounterNet
 from copy import deepcopy
 from sklearn.neighbors import NearestNeighbors
 from fastcore.test import test_fail
 
 # %% auto 0
-__all__ = ['CFExplanationResults', 'METRICS_CALLABLE', 'METRICS', 'DEFAULT_METRICS', 'Explanation', 'generate_cf_explanations',
-           'BaseEvalMetrics', 'PredictiveAccuracy', 'Validity', 'Proximity', 'Sparsity', 'ManifoldDist', 'Runtime',
-           'compute_so_validity', 'compute_so_proximity', 'compute_so_sparsity', 'evaluate_cfs', 'benchmark_cfs']
+__all__ = ['CFExplanationResults', 'METRICS_CALLABLE', 'METRICS', 'DEFAULT_METRICS', 'Explanation', 'BaseGenerationStrategy',
+           'IterativeGenerationStrategy', 'VmapGenerationStrategy', 'PmapGenerationStrategy', 'StrategyFactory',
+           'generate_cf_explanations', 'BaseEvalMetrics', 'PredictiveAccuracy', 'Validity', 'Proximity', 'Sparsity',
+           'ManifoldDist', 'Runtime', 'compute_so_validity', 'compute_so_proximity', 'compute_so_sparsity',
+           'evaluate_cfs', 'benchmark_cfs']
 
 # %% ../nbs/06_evaluate.ipynb 4
 @dataclass
 class Explanation:
     """Generated CF Explanations class."""
     cf_name: str  # cf method's name
     data_module: TabularDataModule  # data module
@@ -39,14 +41,128 @@
                 self.X = test_X
             if self.y is None:
                 self.y = label
 
 CFExplanationResults = Explanation
 
 # %% ../nbs/06_evaluate.ipynb 8
+class BaseGenerationStrategy:
+    """Base class for mapping strategy."""
+    
+    def __call__(
+        self, 
+        fn: Callable, # Function to generate cf for a single input
+        X: jnp.ndarray, # Input instances to be explained
+        pred_fn: Callable[[Array], Array],
+        **kwargs
+    ) -> Array: # Generated counterfactual explanations
+        raise NotImplementedError
+
+# %% ../nbs/06_evaluate.ipynb 9
+class IterativeGenerationStrategy(BaseGenerationStrategy):
+    """Iterativly generate counterfactuals."""
+
+    def __call__(
+        self, 
+        fn: Callable, # Function to generate cf for a single input
+        X: jnp.ndarray, # Input instances to be explained
+        pred_fn: Callable[[Array], Array],
+        **kwargs
+    ) -> Array: # Generated counterfactual explanations
+        
+        assert X.ndim == 2
+        cfs = jnp.stack([fn(X[i], pred_fn=pred_fn, **kwargs) for i in range(X.shape[0])])
+        assert X.shape == cfs.shape
+        return cfs
+
+# %% ../nbs/06_evaluate.ipynb 10
+class VmapGenerationStrategy(BaseGenerationStrategy):
+    """Generate counterfactuals via `jax.vmap`."""
+
+    def __call__(
+        self, 
+        fn: Callable, # Function to generate cf for a single input
+        X: jnp.ndarray, # Input instances to be explained
+        pred_fn: Callable[[Array], Array],
+        **kwargs
+    ) -> Array: # Generated counterfactual explanations
+        
+        assert X.ndim == 2
+        partial_fn = partial(fn, pred_fn=pred_fn, **kwargs)
+        cfs = jax.vmap(partial_fn)(X)
+        return cfs
+
+# %% ../nbs/06_evaluate.ipynb 11
+def _pad_divisible_X(
+    X: Array,
+    n_devices: int
+):
+    """Pad `X` to be divisible by `n_devices`."""
+    if X.shape[0] % n_devices != 0:
+        pad_size = n_devices - X.shape[0] % n_devices
+        X = jnp.concatenate([X, jnp.zeros((pad_size, *X.shape[1:]))])
+    X_padded = X.reshape(n_devices, -1, *X.shape[1:])
+    return X_padded
+
+# %% ../nbs/06_evaluate.ipynb 13
+class PmapGenerationStrategy(BaseGenerationStrategy):
+    def __init__(
+        self, 
+        n_devices: int = None, # Number of devices. If None, use all available devices
+        strategy: str = 'auto', # Strategy to generate counterfactuals
+        **kwargs
+    ):
+        self.strategy = strategy
+        self.n_devices = n_devices or jax.device_count()
+
+    def __call__(
+        self, 
+        fn: Callable, # Function to generate cf for a single input
+        X: jnp.ndarray, # Input instances to be explained
+        pred_fn: Callable[[Array], Array],
+        **kwargs
+    ) -> Array: # Generated counterfactual explanations
+        
+        assert X.ndim == 2
+        X_padded = _pad_divisible_X(X, self.n_devices)
+        partial_fn = partial(fn, pred_fn=pred_fn, **kwargs)
+        cfs = jax.pmap(jax.vmap(partial_fn))(X_padded)
+        cfs = cfs.reshape(-1, *cfs.shape[2:])
+        cfs = cfs[:X.shape[0]]
+        return cfs
+
+# %% ../nbs/06_evaluate.ipynb 19
+class StrategyFactory(object):
+    """Factory class for Parallelism Strategy."""
+
+    __strategy_map = {
+        'iter': IterativeGenerationStrategy(),
+        'vmap': VmapGenerationStrategy(),
+        'pmap': PmapGenerationStrategy(),
+    }
+
+    def __init__(self) -> None:
+        raise ValueError("This class should not be instantiated.")
+        
+    @staticmethod
+    def get_default_strategy() -> BaseGenerationStrategy:
+        """Get default strategy."""
+        return VmapGenerationStrategy()
+
+    @classmethod
+    def get_strategy(cls, strategy: str | BaseGenerationStrategy) -> BaseGenerationStrategy:
+        """Get strategy."""
+        if isinstance(strategy, BaseGenerationStrategy):
+            return strategy
+        elif isinstance(strategy, str) and strategy in cls.__strategy_map:
+            return cls.__strategy_map[strategy]
+        else:
+            raise ValueError(f"Invalid strategy: {strategy}")
+
+# %% ../nbs/06_evaluate.ipynb 22
 def _validate_configs(
     cf_module: BaseCFModule,
     datamodule: TabularDataModule,
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray] = None,
     t_configs=None
 ):
     if (pred_fn is None) and (not isinstance(cf_module, BasePredFnCFModule)):
@@ -70,15 +186,15 @@
 ):
     if not cf_module._is_module_trained():
         print(f'{type(cf_module).__name__} contains parametric models. '
             'Starts training before generating explanations...')
         cf_module.train(datamodule, t_configs, pred_fn=pred_fn)
     return cf_module
 
-# %% ../nbs/06_evaluate.ipynb 9
+# %% ../nbs/06_evaluate.ipynb 23
 def _check_aux_pred_fn_args(pred_fn_args: dict | None):
     if pred_fn_args is None:
         return dict()
     elif isinstance(pred_fn_args, dict):
         return pred_fn_args
     else:
         raise ValueError(f'`pred_fn_args` should be a `dict`,',
@@ -109,54 +225,56 @@
                     f"and `{type(cf_module).__name__}` has not attribute `pred_fn`."
             )
     elif isinstance(cf_module, BasePredFnCFModule):
         # override pred_fn if `cf_module` has `pred_fn`
         pred_fn = cf_module.pred_fn
     return pred_fn
 
-# %% ../nbs/06_evaluate.ipynb 10
+# %% ../nbs/06_evaluate.ipynb 24
 def generate_cf_explanations(
     cf_module: BaseCFModule, # CF Explanation Module
     datamodule: TabularDataModule, # Data Module
     pred_fn: callable = None, # Predictive function
+    strategy: str | BaseGenerationStrategy = 'vmap', # Parallelism Strategy for generating CFs
     t_configs: TrainingConfigs = None, # training configs for `BaseParametricCFModule`
     pred_fn_args: dict = None # auxiliary arguments for `pred_fn` 
 ) -> Explanation:
     """Generate CF explanations."""
 
     _validate_configs(cf_module, datamodule, pred_fn, t_configs)
     cf_module = _prepare_module(cf_module, datamodule)
 
+    # create `pred_fn` which only takes `x` as an input
+    if pred_fn is not None:
+        pred_fn = _AuxPredFn(pred_fn, pred_fn_args=pred_fn_args)
+
     if isinstance(cf_module, BaseParametricCFModule):
         cf_module = _train_parametric_module(
             cf_module, datamodule, t_configs=t_configs, pred_fn=pred_fn
         )
     X, _ = datamodule.test_dataset[:]
-    
-    # create `pred_fn` which only takes `x` as an input
-    if pred_fn is not None:
-        pred_fn = _AuxPredFn(pred_fn, pred_fn_args=pred_fn_args)
 
-    # generate cfs
+    strategy = StrategyFactory.get_strategy(strategy)
     current_time = time.time()
-    cfs = cf_module.generate_cfs(X, pred_fn=pred_fn)
+    cfs = strategy(cf_module.generate_cf, X, pred_fn=pred_fn)
     total_time = time.time() - current_time
+
     # check pred_fn
     pred_fn = _check_pred_fn(pred_fn, cf_module)
 
     return Explanation(
         cf_name=cf_module.name,
         data_module=datamodule,
         cfs=cfs,
         total_time=total_time,
         pred_fn=pred_fn,
     )
 
 
-# %% ../nbs/06_evaluate.ipynb 18
+# %% ../nbs/06_evaluate.ipynb 32
 class BaseEvalMetrics(ABC):
     """Base evaluation metrics class."""
 
     def __init__(self, name: str = None):
         if name is None: name = type(self).__name__
         self.name = name
 
@@ -167,138 +285,138 @@
                 "EvalMetrics must have a name. Add the following as the first line in your "
                 f"__init__ method:\n\nsuper({self.__name__}, self).__init__()")
         return self.name
 
     def __call__(self, cf_explanations: Explanation) -> Any:
         raise NotImplementedError
 
-# %% ../nbs/06_evaluate.ipynb 19
+# %% ../nbs/06_evaluate.ipynb 33
 def _compute_acc(
     input: jnp.DeviceArray, # input dim: [N, k]
     label: jnp.DeviceArray, # label dim: [N] or [N, 1]
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray]
 ) -> float:
     y_pred = pred_fn(input).reshape(-1, 1).round()
     label = label.reshape(-1, 1)
     return accuracy(y_pred, label).item()
 
-# %% ../nbs/06_evaluate.ipynb 21
+# %% ../nbs/06_evaluate.ipynb 35
 class PredictiveAccuracy(BaseEvalMetrics):
     """Compute the accuracy of the predict function."""
     
     def __init__(self, name: str = "accuracy"):
         super().__init__(name=name)
 
     def __call__(self, cf_explanations: Explanation) -> float:
         X, y = cf_explanations.data_module.test_dataset[:]
         return _compute_acc(X, y, cf_explanations.pred_fn)
 
-# %% ../nbs/06_evaluate.ipynb 23
+# %% ../nbs/06_evaluate.ipynb 37
 def _compute_val(
     input: jnp.DeviceArray, # input dim: [N, k]
     cfs: jnp.DeviceArray, # cfs dim: [N, k]
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray]
 ):
     y_pred = pred_fn(input).reshape(-1, 1).round()
     y_prime = jnp.ones_like(y_pred) - y_pred
     cf_y = pred_fn(cfs).reshape(-1, 1).round()
     return accuracy(y_prime, cf_y).item()
 
-# %% ../nbs/06_evaluate.ipynb 25
+# %% ../nbs/06_evaluate.ipynb 39
 class Validity(BaseEvalMetrics):
     """Compute fraction of input instances on which CF explanation methods output valid CF examples."""
     
     def __init__(self, name: str = "validity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_val(
             X, cf_explanations.cfs, cf_explanations.pred_fn
         )
 
-# %% ../nbs/06_evaluate.ipynb 26
+# %% ../nbs/06_evaluate.ipynb 40
 def _compute_proximity(
     inputs: jnp.DeviceArray, # input dim: [N, k]
     cfs: jnp.DeviceArray, # cfs dim: [N, k]
 ):
     prox = jnp.linalg.norm(inputs - cfs, ord=1, axis=1).mean()
     return prox.item()
 
-# %% ../nbs/06_evaluate.ipynb 28
+# %% ../nbs/06_evaluate.ipynb 42
 class Proximity(BaseEvalMetrics):
     """Compute L1 norm distance between input datasets and CF examples divided by the number of features."""
     def __init__(self, name: str = "proximity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_proximity(X, cf_explanations.cfs)
 
-# %% ../nbs/06_evaluate.ipynb 29
+# %% ../nbs/06_evaluate.ipynb 43
 def _compute_spar(
     input: jnp.DeviceArray,
     cfs: jnp.DeviceArray,
     cat_idx: int
 ):
     # calculate sparsity
     cat_sparsity = proximity(input[:, cat_idx:], cfs[:, cat_idx:]) / 2
     cont_sparsity = jnp.linalg.norm(
         jnp.abs(input[:, :cat_idx] - cfs[:, :cat_idx]), ord=0, axis=1
     ).mean()
     return (cont_sparsity + cat_sparsity).item()
 
 
-# %% ../nbs/06_evaluate.ipynb 30
+# %% ../nbs/06_evaluate.ipynb 44
 class Sparsity(BaseEvalMetrics):
     """Compute the number of feature changes between input datasets and CF examples."""
 
     def __init__(self, name: str = "sparsity"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_spar(X, cf_explanations.cfs, cf_explanations.cat_idx)
 
-# %% ../nbs/06_evaluate.ipynb 31
+# %% ../nbs/06_evaluate.ipynb 45
 def _compute_manifold_dist(
     input: jnp.DeviceArray,
     cfs: jnp.DeviceArray,
     n_neighbors: int = 1,
     p: int = 2
 ):
     knn = NearestNeighbors(n_neighbors=n_neighbors, p=p)
     knn.fit(input)
     nearest_dist, nearest_points = knn.kneighbors(cfs, 1, return_distance=True)
     return jnp.mean(nearest_dist).item()
 
-# %% ../nbs/06_evaluate.ipynb 32
+# %% ../nbs/06_evaluate.ipynb 46
 class ManifoldDist(BaseEvalMetrics):
     """Compute the L1 distance to the n-nearest neighbor for all CF examples."""
     def __init__(self, n_neighbors: int = 1, p: int = 2, name: str = "manifold_dist"):
         super().__init__(name=name)
         self.n_neighbors = n_neighbors
         self.p = p
         
     def __call__(self, cf_explanations: Explanation) -> float:
         X, _ = cf_explanations.data_module.test_dataset[:]
         return _compute_manifold_dist(
             X, cf_explanations.cfs, self.n_neighbors, self.p
         )
 
-# %% ../nbs/06_evaluate.ipynb 33
+# %% ../nbs/06_evaluate.ipynb 47
 class Runtime(BaseEvalMetrics):
     """Get the running time to generate CF examples."""
     def __init__(self, name: str = "runtime"):
         super().__init__(name=name)
     
     def __call__(self, cf_explanations: Explanation) -> float:
         return cf_explanations.total_time
 
-# %% ../nbs/06_evaluate.ipynb 35
+# %% ../nbs/06_evaluate.ipynb 49
 def _create_second_order_cfs(cf_results: CFExplanationResults, threshold: float = 2.0):
     X, y = cf_results.data_module.test_dataset[:]
     cfs = cf_results.cfs
     scaler = cf_results.data_module.normalizer
     cat_idx = cf_results.data_module.cat_idx
 
     # get normalized threshold = threshold / (max - min)
@@ -337,15 +455,15 @@
     cfs_hat = _create_second_order_cfs(cf_results, threshold)
     cf_results_so = deepcopy(cf_results)
     cf_results_so.cfs = cfs_hat
     compute_sparsity = Sparsity()
     return compute_sparsity(cf_results_so)
 
 
-# %% ../nbs/06_evaluate.ipynb 37
+# %% ../nbs/06_evaluate.ipynb 51
 def fake_explanations():
     """Generate sudo explanations for testing."""
     from relax.data import load_data
 
     dm = load_data("adult")
     X, y = dm.test_dataset[:]
     cfs = X
@@ -353,15 +471,15 @@
     pred_fn = lambda x: jax.random.bernoulli(jax.random.PRNGKey(0), 0.5, (x.shape[0], 1)).astype(float)
     assert y.shape == pred_fn(X).shape
     return Explanation(
         cf_name='sudo', data_module=dm, cfs=cfs, pred_fn=pred_fn, total_time=0.0, dataset_name=dn
     )
 
 
-# %% ../nbs/06_evaluate.ipynb 38
+# %% ../nbs/06_evaluate.ipynb 52
 # METRICS = dict(
 #     acc=PredictiveAccuracy(),
 #     accuracy=PredictiveAccuracy(),
 #     validity=Validity(),
 #     proximity=Proximity(),
 #     runtime=Runtime(),
 #     manifold_dist=ManifoldDist(),
@@ -379,15 +497,15 @@
     ManifoldDist(),
 ]
 
 METRICS = { m.name: m for m in METRICS_CALLABLE }
 
 DEFAULT_METRICS = ["acc", "validity", "proximity"]
 
-# %% ../nbs/06_evaluate.ipynb 40
+# %% ../nbs/06_evaluate.ipynb 54
 def _get_metric(metric: str | BaseEvalMetrics, cf_exp: Explanation):
     if isinstance(metric, str):
         if metric not in METRICS.keys():
             raise ValueError(f"'{metric}' is not supported. Must be one of {METRICS.keys()}")
         res = METRICS[metric](cf_exp)
     elif callable(metric):
         # f(cf_exp) not supported for now
@@ -397,15 +515,15 @@
     else:
         raise ValueError(f"{type(metric).__name__} is not supported as a metric.")
     
     if isinstance(res, jnp.ndarray) and res.shape == (1,):
         res = res.item()
     return res
 
-# %% ../nbs/06_evaluate.ipynb 42
+# %% ../nbs/06_evaluate.ipynb 56
 def evaluate_cfs(
     cf_exp: Explanation, # CF Explanations
     metrics: Iterable[Union[str, BaseEvalMetrics]] = None, # A list of Metrics. Can be `str` or a subclass of `BaseEvalMetrics`
     return_dict: bool = True, # return a dictionary or not (default: True)
     return_df: bool = False # return a pandas Dataframe or not (default: False)
 ):
     cf_name = cf_exp.cf_name
@@ -421,15 +539,15 @@
     result_df = pd.DataFrame.from_dict(result_dict, orient="index")
     
     if return_dict and return_df:
         return (result_dict, result_df)
     elif return_dict or return_df:
         return result_df if return_df else result_dict
 
-# %% ../nbs/06_evaluate.ipynb 44
+# %% ../nbs/06_evaluate.ipynb 58
 def benchmark_cfs(
     cf_results_list: Iterable[CFExplanationResults],
     metrics: Optional[Iterable[str]] = None,
 ):
     dfs = [
         evaluate_cfs(
             cf_exp=cf_results, metrics=metrics, return_dict=False, return_df=True
```

### Comparing `jax-relax-0.1.3/relax/import_essentials.py` & `jax-relax-0.1.4/relax/import_essentials.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,12 +24,13 @@
 from deprecation import deprecated
 from functools import partial
 
 # jax related
 import jax
 from jax import pmap, vmap, random, device_put, lax, jit, Array
 import jax.numpy as jnp, jax.random as jrand
+from jax_tqdm import loop_tqdm, scan_tqdm
 
 # nn related
 import haiku as hk
 import optax
-import chex
+import chex
```

### Comparing `jax-relax-0.1.3/relax/logger.py` & `jax-relax-0.1.4/relax/logger.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/methods/base.py` & `jax-relax-0.1.4/relax/methods/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,26 @@
         """Name of the CF Explanation Module."""
         raise NotImplementedError
     
     @property
     def data_module(self) -> TabularDataModule:
         """Binded `DataModule`."""
         return self._data_module
+    
+    @abstractmethod
+    def generate_cf(
+        self, 
+        x: Array, # Input to be explained
+        pred_fn: Callable = None, # Predictive function 
+        **kwargs
+    ) -> jnp.ndarray: # Generated counterfactual
+        """Abstract method to generate one counterfactual"""
+        raise NotImplementedError
 
+    @deprecated(deprecated_in='0.1.4')
     @abstractmethod
     def generate_cfs(
         self,
         X: jnp.ndarray, # Input to be explained
         pred_fn: Callable = None # Predictive function 
     ) -> jnp.ndarray: # Generated counterfactuals
         """Abstract method to generate counterfactuals"""
```

### Comparing `jax-relax-0.1.3/relax/methods/cchvae.py` & `jax-relax-0.1.4/relax/methods/cchvae.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,15 +58,16 @@
     def __init__(self, m_config: Dict):
         self.save_hyperparameters(m_config)
         self.m_config = validate_configs(m_config, CHVAEConfigs)
         self.opt = optax.adam(self.m_config.lr)
 
     def init_net_opt(self, dm, key):
         X, _ = dm.train_dataset[:128]
-        Z = jnp.ones((X.shape[0], self.m_config.encoded_size))
+        encoded_size = self.m_config.enc_sizes[-1]
+        Z = jnp.ones((X.shape[0], encoded_size))
 
         self.encoder = make_hk_module(
             Encoder, sizes=self.m_config.enc_sizes, 
         )
         self.decoder = make_hk_module(
             Decoder, sizes=self.m_config.dec_sizes,
             input_size=X.shape[-1]
@@ -161,14 +162,15 @@
     norm_p = jnp.linalg.norm(delta, ord=p_norm, axis=1)
     d_norm = jnp.divide(dist, norm_p).reshape(-1, 1)  # rescale/normalize factor
     delta = jnp.multiply(delta, d_norm)
     candidates = x + delta
     return candidates
 
 # %% ../../nbs/methods/06_cchvae.ipynb 8
+@auto_reshaping('x')
 def _cchvae_generate(
     x: Array,
     rng_key: random.PRNGKey,
     pred_fn: Callable,
     max_steps: int,
     n_search_samples: int,
     step_size: float,
@@ -206,61 +208,54 @@
             lambda _: x_ce[jnp.argmin(distances)].reshape(1, -1),
             lambda _: candidate_cf,
             None
         )
 
         count += 1
         return count, candidate_cf, rng_key
-
-    x_size = x.shape
-    if len(x_size) > 1 and x_size[0] != 1:
-        raise ValueError(
-            f"Invalid Input Shape: Require `x.shape` = (1, k) or (k, ), "
-            f"but got `x.shape` = {x.shape}. This method expects a single input instance."
-        )
-    if len(x_size) == 1:
-        x = x.reshape(1, -1)
     
     y_pred = pred_fn(x).round().reshape(-1)
     z, _ = cchvae_module.encode(cchvae_params[0], rng_key, x)
     # z_rep = jnp.repeat(z.reshape(1, -1), n_search_samples, axis=0)
     z_rep = z.reshape(1, -1)
     rng_key, _ = jrand.split(rng_key)
     state = (0, x, rng_key) # (count, candidate_cf, rng_key)
     count, candidate_cf, rng_key = jax.lax.while_loop(cond_fn, body_fn, state)
     # while cond_fn(state):
     #     count, candidate_cf, rng_key = body_fn(state)
     # print(count)
-    return candidate_cf.reshape(x_size)
+    return candidate_cf
 
 # %% ../../nbs/methods/06_cchvae.ipynb 9
 class CCHVAEConfigs(BaseParser):
     enc_sizes: List[int] = Field(
         [20, 16, 14, 12], description="Encoder hidden sizes"
     ) 
     dec_sizes: List[int] = Field(
         [12, 14, 16, 20], description="Decoder hidden sizes"
     )
     encoded_size: int = Field(5, description="Encoded size")
     lr: float = Field(0.001, description="Learning rate")
     max_steps: int = Field(1000, description="Max steps")
     n_search_samples: int = Field(300, description="Number of generated candidate counterfactuals.")
     step_size: float = Field(0.1, description="Step size")
+    seed: int = Field(0, description="Seed for random number generator")
 
 # %% ../../nbs/methods/06_cchvae.ipynb 10
 class CCHVAE(BaseCFModule, BaseParametricCFModule):
     params: Tuple[hk.Params, hk.Params] = None
     module: CHVAE
     name: str = 'C-CHVAE'
 
-    def __init__(self, m_config: Dict | CCHVAEConfigs = None):
-        if m_config is None:
-            m_config = CCHVAEConfigs()
-        self.m_config = m_config
-        self.module = CHVAE(m_config.dict())
+    def __init__(self, configs: Dict | CCHVAEConfigs = None):
+        if configs is None:
+            configs = CCHVAEConfigs()
+        self.configs = validate_configs(configs, CCHVAEConfigs)
+        self.module = CHVAE(self.configs.dict())
+        self.rng_key = random.PRNGKey(self.configs.seed)
 
     def _is_module_trained(self) -> bool:
         return not (self.params is None)
     
     def train(
         self, 
         datamodule: TabularDataModule, # data module
@@ -269,27 +264,40 @@
     ):
         _default_t_configs = dict(
             n_epochs=10, batch_size=128
         )
         if t_configs is None: t_configs = _default_t_configs
         params, _ = train_model(self.module, datamodule, t_configs)
         self.params = params
+
+    def generate_cf(self, x: Array, pred_fn: Callable = None) -> jnp.ndarray:
+        _cchvae_generate_fn_partial = partial(
+            _cchvae_generate,
+            pred_fn=pred_fn,
+            max_steps=self.configs.max_steps,
+            n_search_samples=self.configs.n_search_samples,
+            step_size=self.configs.step_size,
+            cchvae_module=self.module,
+            cchvae_params=self.params,
+            apply_fn=self.data_module.apply_constraints,
+        )
+        return _cchvae_generate_fn_partial(x, self.rng_key)
     
     def generate_cfs(self, X: Array, pred_fn: Callable = None) -> jnp.ndarray:
         _cchvae_generate_fn_partial = partial(
             _cchvae_generate,
             pred_fn=pred_fn,
-            max_steps=self.m_config.max_steps,
-            n_search_samples=self.m_config.n_search_samples,
-            step_size=self.m_config.step_size,
+            max_steps=self.configs.max_steps,
+            n_search_samples=self.configs.n_search_samples,
+            step_size=self.configs.step_size,
             cchvae_module=self.module,
             cchvae_params=self.params,
             apply_fn=self.data_module.apply_constraints,
         )
-        rngs = lax.broadcast(random.PRNGKey(0), (X.shape[0], ))
+        rngs = lax.broadcast(self.rng_key, (X.shape[0], ))
         return jax.vmap(_cchvae_generate_fn_partial)(X, rngs)
         # for i in tqdm(range(X.shape[0])):
         #     rng = random.PRNGKey(i)
         #     cf = _cchvae_generate_fn_partial(X[i], rng)
         #     if i == 0:
         #         cfs = cf
         #     else:
```

### Comparing `jax-relax-0.1.3/relax/methods/clue.py` & `jax-relax-0.1.4/relax/methods/clue.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,14 +234,15 @@
         rng_key: random.PRNGKey,
         batch: Tuple[jnp.array, jnp.array],
     ) -> Tuple[hk.Params, optax.OptState]:
         pass
 
 
 # %% ../../nbs/methods/08_clue.ipynb 8
+@auto_reshaping('x')
 def _clue_generate(
     x: Array,
     rng_key: jrand.PRNGKey,
     pred_fn: Callable,
     max_steps: int,
     step_size: float,
     vae_module: VAEGaussCat,
@@ -297,33 +298,24 @@
     
     def step(i, z_opt_state):
         z, opt_state = z_opt_state
         z_grad = jax.grad(compute_loss)(z, dec_params)
         z, opt_state = grad_update(z_grad, z, opt_state, opt)
         return z, opt_state
     
-    x_size = x.shape
-    if len(x_size) > 1 and x_size[0] != 1:
-        raise ValueError(
-            f"Invalid Input Shape: Require `x.shape` = (1, k) or (k, ), "
-            f"but got `x.shape` = {x.shape}. This method expects a single input instance."
-        )
-    if len(x_size) == 1:
-        x = x.reshape(1, -1)
-    
     enc_params, dec_params = vae_params
     key_1, _ = jax.random.split(rng_key)
     z = sample_latent_from_x(x, enc_params, key_1)
     opt = optax.adam(step_size)
     opt_state = opt.init(z)
     y_targets = 1 - pred_fn(x)
 
     # Write a loop to optimize z using lax.fori_loop
     z, opt_state = lax.fori_loop(0, max_steps, step, (z, opt_state))
-    cf = generate_from_z(z, dec_params, hard=True).reshape(x_size)
+    cf = generate_from_z(z, dec_params, hard=True)
     return cf
 
 
 # %% ../../nbs/methods/08_clue.ipynb 9
 class CLUEConfigs(BaseParser):
     enc_sizes: List[int] = Field(
         [20, 16, 14, 12], description="Sequence of Encoder layer sizes."
@@ -333,25 +325,27 @@
     )
     encoded_size: int = Field(5, description="Encoded size")
     lr: float = Field(0.001, description="Learning rate")
     max_steps: int = Field(500, description="Max steps")
     step_size: float = Field(0.01, description="Step size")
     vae_n_epochs: int = Field(10, description="Number of epochs for VAE")
     vae_batch_size: int = Field(128, description="Batch size for VAE")
+    seed: int = Field(0, description="Seed for random number generator")
 
 # %% ../../nbs/methods/08_clue.ipynb 10
 class CLUE(BaseCFModule, BaseParametricCFModule):
     params: Tuple[hk.Params, hk.Params] = None
     module: VAEGaussCat
     name: str = 'CLUE'
 
     def __init__(self, m_config: Dict | CLUEConfigs = None):
         if m_config is None: m_config = CLUEConfigs()
         self.m_config = m_config
         self.module = VAEGaussCat(m_config.dict())
+        self.rng_key = random.PRNGKey(self.m_config.seed)
 
     def _is_module_trained(self) -> bool:
         return not (self.params is None)
     
     def train(
         self, 
         datamodule: TabularDataModule, # data module
@@ -361,17 +355,19 @@
         _default_t_configs = dict(
             n_epochs=10, batch_size=128
         )
         if t_configs is None: t_configs = _default_t_configs
         params, _ = train_model(self.module, datamodule, t_configs)
         self.params = params
 
-    def generate_cf(self, x, rng_key, pred_fn: Callable = None) -> Array:
+    def generate_cf(self, x, pred_fn: Callable = None) -> Array:
         return _clue_generate(
-            x, rng_key=rng_key, pred_fn=pred_fn,
+            x, 
+            rng_key=self.rng_key, 
+            pred_fn=pred_fn,
             max_steps=self.m_config.max_steps,
             step_size=self.m_config.step_size,
             vae_module=self.module,
             vae_params=self.params,
             uncertainty_weight=.0,
             aleatoric_weight=0.0,
             prior_weight=0.0,
```

### Comparing `jax-relax-0.1.3/relax/methods/counternet.py` & `jax-relax-0.1.4/relax/methods/counternet.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # %% ../../nbs/methods/04_counternet.ipynb 3
 from __future__ import annotations
 from ..import_essentials import *
 from ..module import MLP, BaseTrainingModule
 from .base import BaseCFModule, BaseParametricCFModule, BasePredFnCFModule
 from ..trainer import TrainingConfigs, train_model
 from ..data import TabularDataModule
-from ..utils import validate_configs, sigmoid, accuracy, proximity, make_model, init_net_opt, grad_update
+from ..utils import *
 from functools import partial
 
 # %% auto 0
 __all__ = ['CounterNetModel', 'partition_trainable_params', 'project_immutable_features', 'CounterNetTrainingModuleConfigs',
            'CounterNetTrainingModule', 'CounterNetConfigs', 'CounterNet']
 
 # %% ../../nbs/methods/04_counternet.ipynb 5
@@ -312,14 +312,18 @@
         _default_t_configs = dict(
             n_epochs=100, batch_size=128
         )
         if t_configs is None: t_configs = _default_t_configs
         params, _ = train_model(self.module, datamodule, t_configs)
         self.params = params
 
+    @auto_reshaping('x')
+    def generate_cf(self, x: jnp.ndarray, pred_fn = None) -> jnp.ndarray:
+        return self.module.generate_cfs(x, self.params, rng_key=jax.random.PRNGKey(0))
+
     def generate_cfs(self, X: jnp.ndarray, pred_fn = None) -> jnp.ndarray:
         return self.module.generate_cfs(X, self.params, rng_key=jax.random.PRNGKey(0))
     
     def pred_fn(self, X: jnp.DeviceArray):
         rng_key = jax.random.PRNGKey(0)
         y_pred = self.module.predict(self.params, rng_key, X)
         return y_pred
```

### Comparing `jax-relax-0.1.3/relax/methods/diverse.py` & `jax-relax-0.1.4/relax/methods/diverse.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # %% auto 0
 __all__ = ['DiverseCFConfig', 'DiverseCF']
 
 # %% ../../nbs/methods/02_diverse.ipynb 3
 from ..import_essentials import *
 from .base import BaseCFModule
-from ..utils import validate_configs, dist, grad_update
+from ..utils import *
 
 # %% ../../nbs/methods/02_diverse.ipynb 4
 def hinge_loss(input: jnp.DeviceArray, target: jnp.DeviceArray):
     """
     reference:
     - https://github.com/interpretml/DiCE/blob/a772c8d4fcd88d1cab7f2e02b0bcc045dc0e2eab/dice_ml/explainer_interfaces/dice_pytorch.py#L196-L202
     - https://en.wikipedia.org/wiki/Hinge_loss
@@ -52,80 +52,80 @@
             regularization_loss += jnp.power(
                 (jnp.sum(cfs[i][cat_idx:cat_idx_end]) - 1.0), 2
             )
     return regularization_loss
 
 
 # %% ../../nbs/methods/02_diverse.ipynb 8
+@auto_reshaping('x')
 def _diverse_cf(
     x: jnp.DeviceArray,  # `x` shape: (k,), where `k` is the number of features
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray],  # y = pred_fn(x)
     n_cfs: int,
     n_steps: int,
     lr: float,  # learning rate for each `cf` optimization step
     lambda_: float,  #  loss = validity_loss + lambda_params * cost
     key: jax.random.PRNGKey,
     projection_fn: Callable,
     regularization_fn: Callable
 ) -> jnp.DeviceArray:  # return `cf` shape: (k,)
-    def loss_fn_1(cf_y: jnp.DeviceArray, y_prime: jnp.DeviceArray):
+    @jit
+    def loss_fn_1(cf_y: Array, y_prime: Array):
         return jnp.mean(hinge_loss(input=cf_y, target=y_prime))
 
-    def loss_fn_2(x: jnp.DeviceArray, cf: jnp.DeviceArray):
+    @jit
+    def loss_fn_2(x: Array, cf: Array):
         return jnp.mean(jnp.abs(cf - x))
 
+    @partial(jit, static_argnums=(1,))
     def loss_fn_3(cfs: jnp.DeviceArray, n_cfs: int):
         return dpp_style(cfs, n_cfs)
 
-    def loss_fn_4(x: jnp.DeviceArray, cfs: jnp.DeviceArray):
+    @jit
+    def loss_fn_4(x: Array, cfs: Array):
         # return _compute_regularization_loss(cfs, cat_idx, cat_arrays, n_cfs)
         reg_loss = 0.
         for i in range(n_cfs):
             reg_loss += regularization_fn(x, cfs[i])
         return reg_loss
 
+    @partial(jit, static_argnums=(2,))
     def loss_fn(
         cf: jnp.DeviceArray,  # `cf` shape: (k, n_cfs)
         x: jnp.DeviceArray,  # `x` shape: (k, 1)
-        pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray],
+        pred_fn: Callable[[Array], Array],
     ):
         y_pred = pred_fn(x)
         y_prime = 1.0 - y_pred
         cf_y = pred_fn(cf)
 
         loss_1 = loss_fn_1(cf_y, y_prime)
         loss_2 = loss_fn_2(x, cf)
         loss_3 = loss_fn_3(cf, n_cfs)
         loss_4 = loss_fn_4(x, cfs)
         return loss_1 + loss_2 + loss_3 + loss_4
 
-    @jax.jit
+    @loop_tqdm(n_steps)
     def gen_cf_step(
-        x: jnp.DeviceArray, cf: jnp.DeviceArray, opt_state: optax.OptState
-    ) -> Tuple[jnp.DeviceArray, optax.OptState]:
+        i, cf_opt_state: Tuple[Array, optax.OptState]
+    ) -> Tuple[Array, optax.OptState]:
+        cf, opt_state = cf_opt_state
         cf_grads = jax.grad(loss_fn)(cf, x, pred_fn)
         cf, opt_state = grad_update(cf_grads, cf, opt_state, opt)
         return cf, opt_state
 
-    x_size = x.shape
-    if len(x_size) > 1 and x_size[0] != 1:
-        raise ValueError(
-            f"""Invalid Input Shape: Require `x.shape` = (1, k) or (k, ),
-but got `x.shape` = {x.shape}. This method expects a single input instance."""
-        )
-    if len(x_size) == 1:
-        x = x.reshape(1, -1)
+    key, subkey = jax.random.split(key)
     cfs = jax.random.normal(key, shape=(n_cfs, x.shape[-1]))
     opt = optax.rmsprop(lr)
     opt_state = opt.init(cfs)
-    for _ in tqdm(range(n_steps)):
-        cfs, opt_state = gen_cf_step(x, cfs, opt_state)
+    cfs, opt_state = lax.fori_loop(0, n_steps, gen_cf_step, (cfs, opt_state))
+    # for _ in tqdm(range(n_steps)):
+    #     cfs, opt_state = gen_cf_step(x, cfs, opt_state)
     cf = projection_fn(x, cfs[:1, :], hard=True)
-    return cf.reshape(x_size)
-
+    return cf
 
 # %% ../../nbs/methods/02_diverse.ipynb 9
 class DiverseCFConfig(BaseParser):
     n_cfs: int = 5
     n_steps: int = 1000
     lr: float = 0.01
     lambda_: float = 0.01  # loss = validity_loss + lambda_params * cost
```

### Comparing `jax-relax-0.1.3/relax/methods/proto.py` & `jax-relax-0.1.4/relax/methods/proto.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # %% ../../nbs/methods/03_prototype.ipynb 3
 from __future__ import annotations
 from ..import_essentials import *
 from .base import BaseCFModule, BaseParametricCFModule
 from ..data import TabularDataModule
 from ..module import BaseTrainingModule, MLP
 from ..trainer import train_model, TrainingConfigs
-from ..utils import validate_configs, binary_cross_entropy, make_model, init_net_opt, grad_update
+from ..utils import *
 from functools import partial
 
 # %% auto 0
 __all__ = ['ProtoCFConfig', 'ProtoCF']
 
 # %% ../../nbs/methods/03_prototype.ipynb 4
 class AEConfigs(BaseParser):
@@ -58,117 +58,122 @@
         )
         return params, opt_state
 
     @partial(jax.jit, static_argnames=['self', 'is_training'])
     def forward(self, params, rng_key, x, is_training: bool = True):
         return self.net.apply(params, rng_key, x, is_training = is_training)
 
+    @partial(jax.jit, static_argnames=['self', ])
     def encode(self, params, rng_key, x):
         _, z = self.forward(params, rng_key, x, is_training=False)
         return z
 
+    @partial(jax.jit, static_argnames=['self', 'is_training'])
     def loss_fn(self, params, rng_key, batch, is_training=True):
         x, y = batch
         x_hat, z = self.forward(params, rng_key, x, is_training)
         return jnp.mean(vmap(optax.l2_loss)(x, x_hat))
 
-    @partial(jax.jit, static_argnames=['self'])
+    @partial(jit, static_argnames=['self'])
     def _training_step(self, params, opt_state, rng_key, batch):
-        grads = jax.grad(self.loss_fn)(params, rng_key, batch)
+        loss, grads = jax.value_and_grad(self.loss_fn)(params, rng_key, batch)
         upt_params, opt_state = grad_update(grads, params, opt_state, self.opt)
-        return upt_params, opt_state
+        return loss, upt_params, opt_state
 
     def training_step(
         self,
         params: hk.Params,
         opt_state: optax.OptState,
         rng_key: random.PRNGKey,
         batch: Tuple[jnp.array, jnp.array]
     ) -> Tuple[hk.Params, optax.OptState]:
-        upt_params, opt_state = self._training_step(params, opt_state, rng_key, batch)
+        loss, upt_params, opt_state = self._training_step(params, opt_state, rng_key, batch)
 
-        loss = self.loss_fn(params, rng_key, batch)
+        # loss = self.loss_fn(params, rng_key, batch)
         self.log_dict({
             'train/train_loss_1': loss.item()
         })
-        return params, opt_state
+        return upt_params, opt_state
 
     def validation_step(self, params, rng_key, batch):
         x, y = batch
         loss = self.loss_fn(params, rng_key, batch, is_training=False)
         logs = {
             'val/val_loss': loss.item(),
         }
         self.log_dict(logs)
 
 # %% ../../nbs/methods/03_prototype.ipynb 6
+@auto_reshaping('x')
 def _proto_cf(
     x: jnp.DeviceArray, # `x` shape: (k,), where `k` is the number of features
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray], # y = pred_fn(x)
     n_steps: int,
     lr: float, # learning rate for each `cf` optimization step
     lambda_: float, #  loss = validity_loss + lambda_params * cost
     ae: AETrainingModule,
     ae_params: hk.Params,
     sampled_data_pos: jnp.DeviceArray,
     sampled_data_neg: jnp.DeviceArray,
     sampled_label: jnp.DeviceArray,
     apply_constraints_fn: Callable
 ) -> jnp.DeviceArray: # return `cf` shape: (k,)
+    @jit
     def proto(data):
         return ae.encode(ae_params, jax.random.PRNGKey(0), data)
 
+    @jit
     def loss_fn_1(cf_y: jnp.DeviceArray, y_prime: jnp.DeviceArray):
         return jnp.mean(binary_cross_entropy(preds=cf_y, labels=y_prime))
 
+    @jit
     def loss_fn_2(x: jnp.DeviceArray, cf: jnp.DeviceArray):
         return jnp.mean(optax.l2_loss(cf, x)) + 0.1 * jnp.mean(jnp.mean(jnp.abs(x - cf)))
 
+    @jit
     def loss_fn_3(cf, data):
         error = proto(cf) - proto(data)
         return jnp.mean(0.5 * (error) ** 2)
 
+    @partial(jit, static_argnames=['pred_fn'])
     def loss_fn(
         cf: jnp.DeviceArray, # `cf` shape: (k, 1)
         x: jnp.DeviceArray,  # `x` shape: (k, 1)
         pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray]
     ):
         y_pred = pred_fn(x)
         y_prime = 1. - y_pred
         cf_y = pred_fn(cf)
 
         y_prime_round = jnp.mean(jnp.round(y_prime))
 
         return loss_fn_1(cf_y, y_prime) + loss_fn_2(x, cf) \
             + loss_fn_3(cf, sampled_data_pos) * y_prime_round + loss_fn_3(cf, sampled_data_neg) * (1 - y_prime_round)
 
-    @jax.jit
+    @loop_tqdm(n_steps)
     def gen_cf_step(
-        x: jnp.DeviceArray, cf: jnp.DeviceArray, opt_state: optax.OptState
-    ) -> Tuple[jnp.DeviceArray, optax.OptState]:
+        i, cf_opt_state: Tuple[Array, optax.OptState]
+    ) -> Tuple[Array, optax.OptState]:
+        cf, opt_state = cf_opt_state
         cf_grads = jax.grad(loss_fn)(cf, x, pred_fn)
         cf, opt_state = grad_update(cf_grads, cf, opt_state, opt)
         cf = apply_constraints_fn(x, cf, hard=False)
         # cf = jnp.clip(cf, 0., 1.)
         return cf, opt_state
 
-    x_size = x.shape
-    if len(x_size) > 1 and x_size[0] != 1:
-        raise ValueError(f"""Invalid Input Shape: Require `x.shape` = (1, k) or (k, ),
-but got `x.shape` = {x.shape}. This method expects a single input instance.""")
-    if len(x_size) == 1:
-        x = x.reshape(1, -1)
     cf = jnp.array(x, copy=True)
     opt = optax.rmsprop(lr)
     opt_state = opt.init(cf)
-    for _ in tqdm(range(n_steps)):
-        cf, opt_state = gen_cf_step(x, cf, opt_state)
+    
+    cf, opt_state = lax.fori_loop(0, n_steps, gen_cf_step, (cf, opt_state))
+    # for _ in tqdm(range(n_steps)):
+    #     cf, opt_state = gen_cf_step(x, cf, opt_state)
 
     cf = apply_constraints_fn(x, cf, hard=True)
-    return cf.reshape(x_size)
+    return cf
 
 # %% ../../nbs/methods/03_prototype.ipynb 7
 class ProtoCFConfig(BaseParser):
     
     n_steps: int = 1000
     lr: float = 0.01
     lambda_: float = 0.01 # loss = validity_loss + lambda_params * cost
```

### Comparing `jax-relax-0.1.3/relax/methods/sphere.py` & `jax-relax-0.1.4/relax/methods/sphere.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     for col in cat_arrays:
         rng_key, cat_sample = sample_categorical(rng_key, col)
         candidates.append(cat_sample)
     candidates = jnp.concatenate(candidates, axis=1)
     return candidates
 
 # %% ../../nbs/methods/05_sphere.ipynb 6
+@auto_reshaping('x')
 def _growing_spheres(
     rng_key: jrand.PRNGKey, # Random number generator key
     x: Array, # Input instance. Shape: (n_features)
     pred_fn: Callable, # Prediction function
     n_steps: int, # Number of steps
     n_samples: int,  # Number of samples to sample
     cat_idx: int, # Index of categorical features
@@ -112,32 +113,22 @@
         # if jnp.any(jnp.logical_not(jnp.isinf(candidates))):
         #     # Find the closest counterfactual
         #     closest_idx = dist.argmin()
         #     candidate_cf = candidates[closest_idx].reshape(1, -1)
 
         return candidate_cf, count + 1, rng_key
     
-
-    x_size = x.shape
-    if len(x_size) > 1 and x_size[0] != 1:
-        raise ValueError(
-            f"Invalid Input Shape: Require `x.shape` = (1, k) or (k, ), "
-            f"but got `x.shape` = {x.shape}. This method expects a single input instance."
-        )
-    if len(x_size) == 1:
-        x = x.reshape(1, -1)
-
     y_pred = pred_fn(x).round().reshape(-1)
     candidate_cf = jnp.ones_like(x) * jnp.inf
     count = 0
     state = (candidate_cf, count, rng_key)
     candidate_cf, _, _ = lax.while_loop(cond_fn, body_fn, state)
     # if `inf` is found, return the original input
     candidate_cf = jnp.where(jnp.isinf(candidate_cf), x, candidate_cf)
-    return candidate_cf.reshape(x_size)
+    return candidate_cf
 
 # %% ../../nbs/methods/05_sphere.ipynb 7
 def apply_immutable(x: Array, cf: Array, immutable_idx: List[int]):
     if immutable_idx is not None:
         cf = cf.at[:, immutable_idx].set(x[:, immutable_idx])
     return cf
 
@@ -157,27 +148,26 @@
     def __init__(
         self,
         configs: Dict | GSConfig = None
     ):
         if configs is None:
             configs = GSConfig()
         self.configs = validate_configs(configs, GSConfig)
+        self.rng = jrand.PRNGKey(self.configs.seed)
     
     def generate_cf(
         self,
         x: Array,
-        rng_key: jrand.PRNGKey,
         pred_fn: Callable,
     ):
-        # rng_key = jrand.PRNGKey(self.configs.seed)
         cat_idx = self.data_module.cat_idx
         apply_immutable_partial = partial(
             apply_immutable, immutable_idx=self.data_module._imutable_idx_list)
         cf = _growing_spheres(
-            rng_key,
+            self.rng,
             x,
             pred_fn,
             self.configs.n_steps,
             self.configs.n_samples,
             cat_idx,
             self.data_module._cat_arrays,
             self.configs.step_size,
@@ -187,12 +177,12 @@
         return cf
     
     def generate_cfs(
         self, 
         X: Array, 
         pred_fn: Callable = None
     ) -> jnp.ndarray:
-        rng_keys = jrand.split(jrand.PRNGKey(self.configs.seed), X.shape[0])
+        rng_keys = jrand.split(jrand.PRNGKey(self.configs.seed), num=X.shape[0])
         generate_cf_partial = jit(partial(self.generate_cf, pred_fn=pred_fn))
         cfs = jax.vmap(generate_cf_partial)(X, rng_keys)
         # cfs = generate_cf_partial(X[0], rng_keys[0])
         return cfs
```

### Comparing `jax-relax-0.1.3/relax/methods/vaecf.py` & `jax-relax-0.1.4/relax/methods/vaecf.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,16 +281,32 @@
         )
         if t_configs is None: t_configs = _default_t_configs
         
         setattr(self.module, 'pred_fn', pred_fn)
         params, _ = train_model(self.module, datamodule, t_configs)
         self.params = params
     
+    @auto_reshaping('x')
+    @partial(jax.jit, static_argnums=[0, 2])
+    def generate_cf(
+        self, 
+        x: Array, 
+        pred_fn: Callable = None
+    ) -> jnp.ndarray:
+        y = pred_fn(x).round().reshape(-1, 1)
+        inputs = jnp.concatenate([x, y], axis=-1)
+        _, _, cfs = self.module.sample(
+            self.params, random.PRNGKey(0), inputs, self.m_config.mu_samples,
+            is_training=False
+        )
+        return self.data_module.apply_constraints(x, cfs[0], hard=True)
+
+
     def generate_cfs(self, X: Array, pred_fn: Callable = None) -> jnp.ndarray:
         y = pred_fn(X).round().reshape(-1, 1)
         inputs = jnp.concatenate([X, y], axis=-1)
         _, _, cfs = self.module.sample(
             self.params, random.PRNGKey(0), inputs, self.m_config.mu_samples,
             is_training=False
         )
-        return self.data_module.apply_constraints(X, cfs[0], hard=False)
+        return self.data_module.apply_constraints(X, cfs[0], hard=True)
```

### Comparing `jax-relax-0.1.3/relax/methods/vanilla.py` & `jax-relax-0.1.4/relax/methods/vanilla.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/methods/01_vanilla.ipynb.
 
 # %% ../../nbs/methods/01_vanilla.ipynb 3
 from __future__ import annotations
 from ..import_essentials import *
 from .base import BaseCFModule
-from ..utils import validate_configs, binary_cross_entropy, grad_update
+from ..utils import *
 
 # %% auto 0
 __all__ = ['VanillaCFConfig', 'VanillaCF']
 
 # %% ../../nbs/methods/01_vanilla.ipynb 4
+@auto_reshaping('x')
 def _vanilla_cf(
     x: jnp.DeviceArray,  # `x` shape: (k,), where `k` is the number of features
     pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray],  # y = pred_fn(x)
     n_steps: int,
     lr: float,  # learning rate for each `cf` optimization step
     lambda_: float,  #  loss = validity_loss + lambda_params * cost
     apply_fn: Callable
 ) -> jnp.DeviceArray:  # return `cf` shape: (k,)
-    def loss_fn_1(cf_y: jnp.DeviceArray, y_prime: jnp.DeviceArray):
+    @jit
+    def loss_fn_1(cf_y: Array, y_prime: Array):
         return jnp.mean(binary_cross_entropy(preds=cf_y, labels=y_prime))
 
-    def loss_fn_2(x: jnp.DeviceArray, cf: jnp.DeviceArray):
+    @jit
+    def loss_fn_2(x: Array, cf: Array):
         return jnp.mean(optax.l2_loss(cf, x))
 
+    @partial(jit, static_argnums=(2,))
     def loss_fn(
-        cf: jnp.DeviceArray,  # `cf` shape: (k, 1)
-        x: jnp.DeviceArray,  # `x` shape: (k, 1)
-        pred_fn: Callable[[jnp.DeviceArray], jnp.DeviceArray],
+        cf: Array,  # `cf` shape: (k, 1)
+        x: Array,  # `x` shape: (k, 1)
+        pred_fn: Callable[[Array], Array],
     ):
         y_pred = pred_fn(x)
         y_prime = 1.0 - y_pred
         cf_y = pred_fn(cf)
         return loss_fn_1(cf_y, y_prime) + lambda_ * loss_fn_2(x, cf)
 
-    @jax.jit
+    @loop_tqdm(n_steps)
     def gen_cf_step(
-        x: jnp.DeviceArray, cf: jnp.DeviceArray, opt_state: optax.OptState
+        i, cf_opt_state: Tuple[Array, optax.OptState] #x: Array, cf: Array, opt_state: optax.OptState
     ) -> Tuple[jnp.DeviceArray, optax.OptState]:
+        cf, opt_state = cf_opt_state
         cf_grads = jax.grad(loss_fn)(cf, x, pred_fn)
         cf, opt_state = grad_update(cf_grads, cf, opt_state, opt)
         cf = apply_fn(x, cf, hard=False)
-        # cf = jnp.clip(cf, 0.0, 1.0)
         return cf, opt_state
 
-    x_size = x.shape
-    if len(x_size) > 1 and x_size[0] != 1:
-        raise ValueError(
-            f"""Invalid Input Shape: Require `x.shape` = (1, k) or (k, ),
-but got `x.shape` = {x.shape}. This method expects a single input instance."""
-        )
-    if len(x_size) == 1:
-        x = x.reshape(1, -1)
     cf = jnp.array(x, copy=True)
     opt = optax.rmsprop(lr)
     opt_state = opt.init(cf)
-    for _ in tqdm(range(n_steps)):
-        cf, opt_state = gen_cf_step(x, cf, opt_state)
+    # for _ in tqdm(range(n_steps)):
+    #     cf, opt_state = gen_cf_step(x, cf, opt_state)
+    cf, opt_state = lax.fori_loop(0, n_steps, gen_cf_step, (cf, opt_state))
 
-    cf = apply_fn(x, cf, hard=False)
-    return cf.reshape(x_size)
+    cf = apply_fn(x, cf, hard=True)
+    return cf
 
 
 # %% ../../nbs/methods/01_vanilla.ipynb 5
 class VanillaCFConfig(BaseParser):
     n_steps: int = 1000
     lr: float = 0.001
     lambda_: float = 0.01  # loss = validity_loss + lambda_ * cost
```

### Comparing `jax-relax-0.1.3/relax/module.py` & `jax-relax-0.1.4/relax/module.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/plots.py` & `jax-relax-0.1.4/relax/plots.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/trainer.py` & `jax-relax-0.1.4/relax/trainer.py`

 * *Files identical despite different names*

### Comparing `jax-relax-0.1.3/relax/utils.py` & `jax-relax-0.1.4/relax/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 # %% ../nbs/00_utils.ipynb 3
 from __future__ import annotations
 from .import_essentials import *
 import nbdev
 from fastcore.basics import AttrDict
 from nbdev.showdoc import BasicMarkdownRenderer
 from inspect import isclass
+from fastcore.test import *
+from jax.core import InconclusiveDimensionOperation
 
 # %% auto 0
-__all__ = ['validate_configs', 'cat_normalize', 'make_model', 'make_hk_module', 'init_net_opt', 'grad_update', 'check_cat_info',
-           'load_json', 'binary_cross_entropy', 'sigmoid', 'accuracy', 'dist', 'proximity', 'get_config']
+__all__ = ['validate_configs', 'cat_normalize', 'auto_reshaping', 'make_model', 'make_hk_module', 'init_net_opt', 'grad_update',
+           'check_cat_info', 'load_json', 'binary_cross_entropy', 'sigmoid', 'accuracy', 'dist', 'proximity',
+           'get_config']
 
 # %% ../nbs/00_utils.ipynb 5
 def validate_configs(
     configs: dict | BaseParser,  # A configuration of the model/dataset.
     config_cls: BaseParser,  # The desired configuration class.
 ) -> BaseParser:
     """return a valid configuration object."""
@@ -87,125 +90,167 @@
 
         cat_idx = cat_end_idx
         normalized_cf.append(cf_cat)
     return jnp.concatenate(normalized_cf, axis=-1)
 
 
 # %% ../nbs/00_utils.ipynb 33
+def _reshape_x(x: Array):
+    x_size = x.shape
+    if len(x_size) > 1 and x_size[0] != 1:
+        raise ValueError(
+            f"""Invalid Input Shape: Require `x.shape` = (1, k) or (k, ),
+but got `x.shape` = {x.shape}. This method expects a single input instance."""
+        )
+    if len(x_size) == 1:
+        x = x.reshape(1, -1)
+    return x, x_size
+
+# %% ../nbs/00_utils.ipynb 34
+def auto_reshaping(reshape_argname: str):
+    """
+    Decorator to automatically reshape function's input into (1, k), 
+    and out to input's shape.
+    """
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            kwargs = inspect.getcallargs(func, *args, **kwargs)
+            if reshape_argname in kwargs:
+                reshaped_x, x_shape = _reshape_x(kwargs[reshape_argname])
+                kwargs[reshape_argname] = reshaped_x
+            else:
+                raise ValueError(
+                    f"Invalid argument name: `{reshape_argname}` is not a valid argument name.")
+            cf = func(**kwargs)
+            if not isinstance(cf, Array): 
+                raise ValueError(
+                    f"Invalid return type: must be a `jax.Array`, but got `{type(cf).__name__}`.")
+            try: 
+                cf = cf.reshape(x_shape)
+            except InconclusiveDimensionOperation:
+                raise ValueError(
+                    f"Invalid return shape: Require `cf.shape` = {cf.shape} "
+                    f"is not compatible with `x.shape` = {x_shape}.")
+            return cf
+
+        return wrapper
+    return decorator
+
+# %% ../nbs/00_utils.ipynb 39
 def make_model(
     m_configs: Dict[str, Any], model: hk.Module  # model configs
 ) -> hk.Transformed:
     # example:
     # net = make_model(PredictiveModel)
     # params = net.init(...)
     def model_fn(x, is_training: bool = True):
         return model(m_configs)(x, is_training)
 
     return hk.transform(model_fn)
 
 
-# %% ../nbs/00_utils.ipynb 34
+# %% ../nbs/00_utils.ipynb 40
 def make_hk_module(
     module: hk.Module, # haiku module 
     *args, # haiku module arguments
     **kargs, # haiku module arguments
 ) -> hk.Transformed:
 
     def model_fn(x, is_training: bool = True):
         return module(*args, **kargs)(x, is_training)
     
     return hk.transform(model_fn)
 
 
-# %% ../nbs/00_utils.ipynb 35
+# %% ../nbs/00_utils.ipynb 41
 def init_net_opt(
     net: hk.Transformed,
     opt: optax.GradientTransformation,
     X: jnp.DeviceArray,
     key: random.PRNGKey,
 ) -> Tuple[hk.Params, optax.OptState]:
     X = device_put(X)
     params = net.init(key, X, is_training=True)
     opt_state = opt.init(params)
     return params, opt_state
 
 
-# %% ../nbs/00_utils.ipynb 36
+# %% ../nbs/00_utils.ipynb 42
 def grad_update(
     grads: Dict[str, jnp.ndarray],
     params: hk.Params,
     opt_state: optax.OptState,
     opt: optax.GradientTransformation,
 ) -> Tuple[hk.Params, optax.OptState]:
     updates, opt_state = opt.update(grads, opt_state)
     upt_params = optax.apply_updates(params, updates)
     return upt_params, opt_state
 
 
-# %% ../nbs/00_utils.ipynb 37
+# %% ../nbs/00_utils.ipynb 43
 def check_cat_info(method):
     def inner(cf_module, *args, **kwargs):
         warning_msg = f"""This CFExplanationModule might not be updated with categorical information.
 You should try `{cf_module.name}.update_cat_info(dm)` before generating cfs.
         """
         if cf_module.cat_idx == 0 and cf_module.cat_arrays == []:
             warnings.warn(warning_msg, RuntimeWarning)
         return method(cf_module, *args, **kwargs)
 
     return inner
 
 
-# %% ../nbs/00_utils.ipynb 39
+# %% ../nbs/00_utils.ipynb 45
 def load_json(f_name: str) -> Dict[str, Any]:  # file name
     with open(f_name) as f:
         return json.load(f)
 
 
-# %% ../nbs/00_utils.ipynb 41
+# %% ../nbs/00_utils.ipynb 47
 def binary_cross_entropy(
     preds: jnp.DeviceArray, # The predicted values
     labels: jnp.DeviceArray # The ground-truth labels
 ) -> jnp.DeviceArray: # Loss value
     """Per-sample binary cross-entropy loss function."""
 
     # Clip the predictions to avoid NaNs in the log
     preds = jnp.clip(preds, 1e-7, 1 - 1e-7)
 
     # Compute the binary cross-entropy
     loss = -labels * jnp.log(preds) - (1 - labels) * jnp.log(1 - preds)
 
     return loss
 
-# %% ../nbs/00_utils.ipynb 42
+# %% ../nbs/00_utils.ipynb 48
 def sigmoid(x):
     # https://stackoverflow.com/a/68293931
     return 0.5 * (jnp.tanh(x / 2) + 1)
 
-# %% ../nbs/00_utils.ipynb 44
+# %% ../nbs/00_utils.ipynb 50
 def accuracy(y_true: jnp.ndarray, y_pred: jnp.ndarray) -> jnp.DeviceArray:
     y_true, y_pred = map(jnp.round, (y_true, y_pred))
     return jnp.mean(jnp.equal(y_true, y_pred))
 
 
 def dist(x: jnp.ndarray, cf: jnp.ndarray, ord: int = 2) -> jnp.DeviceArray:
     dist = jnp.linalg.norm(x - cf, ord=ord, axis=-1, keepdims=True)
     return jnp.mean(vmap(jnp.sum)(dist))
 
 
 def proximity(x: jnp.ndarray, cf: jnp.ndarray) -> jnp.DeviceArray:
     return dist(x, cf, ord=1)
 
-# %% ../nbs/00_utils.ipynb 47
+# %% ../nbs/00_utils.ipynb 53
 @dataclass
 class Config:
     rng_reserve_size: int
     global_seed: int
 
     @classmethod
     def default(cls) -> Config:
         return cls(rng_reserve_size=1, global_seed=42)
 
 main_config = Config.default()
 
-# %% ../nbs/00_utils.ipynb 48
+# %% ../nbs/00_utils.ipynb 54
 def get_config() -> Config: 
     return main_config
```

### Comparing `jax-relax-0.1.3/setup.py` & `jax-relax-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'mit': ('MIT License', 'OSI Approved :: MIT License'),
     'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
     'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
     'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
+py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
 
 requirements = cfg.get('requirements','').split()
 if cfg.get('pip_requirements'): requirements += cfg.get('pip_requirements','').split()
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 dev_requirements = (cfg.get('dev_requirements') or '').split()
```

