# Comparing `tmp/multi-scale-expansion-0.1.1.tar.gz` & `tmp/multi-scale-expansion-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi-scale-expansion-0.1.1.tar", last modified: Sat Apr  1 23:28:20 2023, max compression
+gzip compressed data, was "multi-scale-expansion-0.1.2.tar", last modified: Tue May  9 23:41:31 2023, max compression
```

## Comparing `multi-scale-expansion-0.1.1.tar` & `multi-scale-expansion-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,35 @@
-drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-04-01 23:28:20.642557 multi-scale-expansion-0.1.1/
--rw-r--r--   0 angelmancera   (501) staff       (20)      310 2023-03-27 03:24:56.000000 multi-scale-expansion-0.1.1/.bumpversion.cfg
--rw-r--r--   0 angelmancera   (501) staff       (20)     2016 2023-03-26 23:03:52.000000 multi-scale-expansion-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 angelmancera   (501) staff       (20)     1070 2023-02-21 06:14:34.000000 multi-scale-expansion-0.1.1/LICENSE
--rw-r--r--   0 angelmancera   (501) staff       (20)      361 2023-03-22 23:40:28.000000 multi-scale-expansion-0.1.1/MANIFEST.in
--rw-r--r--   0 angelmancera   (501) staff       (20)     2320 2023-03-22 23:40:28.000000 multi-scale-expansion-0.1.1/Makefile
--rw-r--r--   0 angelmancera   (501) staff       (20)     4534 2023-04-01 23:28:20.642159 multi-scale-expansion-0.1.1/PKG-INFO
--rw-r--r--   0 angelmancera   (501) staff       (20)     2853 2023-03-26 23:03:52.000000 multi-scale-expansion-0.1.1/README.md
-drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-04-01 23:28:20.638289 multi-scale-expansion-0.1.1/multi_scale_expansion/
--rw-r--r--   0 angelmancera   (501) staff       (20)      218 2023-03-30 00:34:33.000000 multi-scale-expansion-0.1.1/multi_scale_expansion/__init__.py
--rw-r--r--   0 angelmancera   (501) staff       (20)     2059 2023-03-06 08:22:24.000000 multi-scale-expansion-0.1.1/multi_scale_expansion/__main__.py
--rw-r--r--   0 angelmancera   (501) staff       (20)     3460 2023-03-23 00:03:33.000000 multi-scale-expansion-0.1.1/multi_scale_expansion/classification.py
--rw-r--r--   0 angelmancera   (501) staff       (20)     3497 2023-03-22 23:45:10.000000 multi-scale-expansion-0.1.1/multi_scale_expansion/dataset.py
--rw-r--r--   0 angelmancera   (501) staff       (20)      566 2023-03-22 23:45:07.000000 multi-scale-expansion-0.1.1/multi_scale_expansion/model.py
-drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-04-01 23:28:20.641034 multi-scale-expansion-0.1.1/multi_scale_expansion/tests/
--rw-r--r--   0 angelmancera   (501) staff       (20)     5825 2023-03-23 00:32:31.000000 multi-scale-expansion-0.1.1/multi_scale_expansion/tests/test_all.py
-drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-04-01 23:28:20.640670 multi-scale-expansion-0.1.1/multi_scale_expansion.egg-info/
--rw-r--r--   0 angelmancera   (501) staff       (20)     4534 2023-04-01 23:28:20.000000 multi-scale-expansion-0.1.1/multi_scale_expansion.egg-info/PKG-INFO
--rw-r--r--   0 angelmancera   (501) staff       (20)      531 2023-04-01 23:28:20.000000 multi-scale-expansion-0.1.1/multi_scale_expansion.egg-info/SOURCES.txt
--rw-r--r--   0 angelmancera   (501) staff       (20)        1 2023-04-01 23:28:20.000000 multi-scale-expansion-0.1.1/multi_scale_expansion.egg-info/dependency_links.txt
--rw-r--r--   0 angelmancera   (501) staff       (20)      198 2023-04-01 23:28:20.000000 multi-scale-expansion-0.1.1/multi_scale_expansion.egg-info/requires.txt
--rw-r--r--   0 angelmancera   (501) staff       (20)       22 2023-04-01 23:28:20.000000 multi-scale-expansion-0.1.1/multi_scale_expansion.egg-info/top_level.txt
--rw-r--r--   0 angelmancera   (501) staff       (20)     1915 2023-03-27 03:24:56.000000 multi-scale-expansion-0.1.1/pyproject.toml
--rw-r--r--   0 angelmancera   (501) staff       (20)       38 2023-04-01 23:28:20.642632 multi-scale-expansion-0.1.1/setup.cfg
--rw-r--r--   0 angelmancera   (501) staff       (20)       39 2023-04-01 23:14:27.000000 multi-scale-expansion-0.1.1/setup.py
+drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-05-09 23:41:31.046370 multi-scale-expansion-0.1.2/
+-rw-r--r--   0 angelmancera   (501) staff       (20)      310 2023-05-09 22:18:48.000000 multi-scale-expansion-0.1.2/.bumpversion.cfg
+-rw-r--r--   0 angelmancera   (501) staff       (20)     2016 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 angelmancera   (501) staff       (20)     1070 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/LICENSE
+-rw-r--r--   0 angelmancera   (501) staff       (20)      513 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/MANIFEST.in
+-rw-r--r--   0 angelmancera   (501) staff       (20)     2851 2023-05-09 23:25:31.000000 multi-scale-expansion-0.1.2/Makefile
+-rw-r--r--   0 angelmancera   (501) staff       (20)     4337 2023-05-09 23:41:31.046038 multi-scale-expansion-0.1.2/PKG-INFO
+-rw-r--r--   0 angelmancera   (501) staff       (20)     2656 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/README.md
+drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-05-09 23:41:31.037142 multi-scale-expansion-0.1.2/docs/
+-rw-r--r--   0 angelmancera   (501) staff       (20)      638 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/docs/Makefile
+-rw-r--r--   0 angelmancera   (501) staff       (20)      804 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/docs/make.bat
+drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-05-09 23:41:31.040035 multi-scale-expansion-0.1.2/docs/source/
+-rw-r--r--   0 angelmancera   (501) staff       (20)     1291 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/docs/source/conf.py
+-rw-r--r--   0 angelmancera   (501) staff       (20)     1371 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/docs/source/examples.md
+-rw-r--r--   0 angelmancera   (501) staff       (20)      531 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/docs/source/index.rst
+-rw-r--r--   0 angelmancera   (501) staff       (20)      332 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/docs/source/installation.md
+-rw-r--r--   0 angelmancera   (501) staff       (20)      100 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/docs/source/modules.rst
+-rw-r--r--   0 angelmancera   (501) staff       (20)      768 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/docs/source/multi_scale_expansion.rst
+drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-05-09 23:41:31.042804 multi-scale-expansion-0.1.2/multi_scale_expansion/
+-rw-r--r--   0 angelmancera   (501) staff       (20)      225 2023-05-09 22:18:48.000000 multi-scale-expansion-0.1.2/multi_scale_expansion/__init__.py
+-rw-r--r--   0 angelmancera   (501) staff       (20)     1088 2023-05-09 21:45:29.000000 multi-scale-expansion-0.1.2/multi_scale_expansion/__main__.py
+-rw-r--r--   0 angelmancera   (501) staff       (20)     5926 2023-05-09 20:21:28.000000 multi-scale-expansion-0.1.2/multi_scale_expansion/classification.py
+-rw-r--r--   0 angelmancera   (501) staff       (20)     5954 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/multi_scale_expansion/dataset.py
+-rw-r--r--   0 angelmancera   (501) staff       (20)     1566 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/multi_scale_expansion/model.py
+drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-05-09 23:41:31.045364 multi-scale-expansion-0.1.2/multi_scale_expansion/tests/
+-rw-r--r--   0 angelmancera   (501) staff       (20)     7414 2023-05-09 20:21:28.000000 multi-scale-expansion-0.1.2/multi_scale_expansion/tests/test_all.py
+drwxr-xr-x   0 angelmancera   (501) staff       (20)        0 2023-05-09 23:41:31.045023 multi-scale-expansion-0.1.2/multi_scale_expansion.egg-info/
+-rw-r--r--   0 angelmancera   (501) staff       (20)     4337 2023-05-09 23:41:30.000000 multi-scale-expansion-0.1.2/multi_scale_expansion.egg-info/PKG-INFO
+-rw-r--r--   0 angelmancera   (501) staff       (20)      715 2023-05-09 23:41:31.000000 multi-scale-expansion-0.1.2/multi_scale_expansion.egg-info/SOURCES.txt
+-rw-r--r--   0 angelmancera   (501) staff       (20)        1 2023-05-09 23:41:30.000000 multi-scale-expansion-0.1.2/multi_scale_expansion.egg-info/dependency_links.txt
+-rw-r--r--   0 angelmancera   (501) staff       (20)      198 2023-05-09 23:41:30.000000 multi-scale-expansion-0.1.2/multi_scale_expansion.egg-info/requires.txt
+-rw-r--r--   0 angelmancera   (501) staff       (20)       22 2023-05-09 23:41:30.000000 multi-scale-expansion-0.1.2/multi_scale_expansion.egg-info/top_level.txt
+-rw-r--r--   0 angelmancera   (501) staff       (20)     1915 2023-05-09 22:18:48.000000 multi-scale-expansion-0.1.2/pyproject.toml
+-rw-r--r--   0 angelmancera   (501) staff       (20)       38 2023-05-09 23:41:31.046505 multi-scale-expansion-0.1.2/setup.cfg
+-rw-r--r--   0 angelmancera   (501) staff       (20)       39 2023-05-09 16:40:59.000000 multi-scale-expansion-0.1.2/setup.py
```

### Comparing `multi-scale-expansion-0.1.1/CONTRIBUTING.md` & `multi-scale-expansion-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `multi-scale-expansion-0.1.1/LICENSE` & `multi-scale-expansion-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multi-scale-expansion-0.1.1/Makefile` & `multi-scale-expansion-0.1.2/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -91,8 +91,28 @@
 .DEFAULT_GOAL := help
 help:
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | sort | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
 
 print-%:
 	@echo '$*=$($*)'
 
-.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+.PHONY: develop build install lint lints format fix check checks annotate test coverage show-coverage tests show-version patch minor major dist-build dist-check dist publish deep-clean clean help
+
+
+############################################################################################
+#DOCS
+############################################################################################
+TMPREPO=/tmp/docs/bt
+
+docs: 
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages: 
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages git@github.com:ColumbiaMancera/multi-scale-expansion.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
```

### Comparing `multi-scale-expansion-0.1.1/PKG-INFO` & `multi-scale-expansion-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-scale-expansion
-Version: 0.1.1
+Version: 0.1.2
 Summary: Check whether your plants are healthy using image classification
 Author-email: Angel Mancera <aem2283@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Angel Mancera
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,18 +30,20 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # Multi Scale Expansion
 Repository to create framework for image classification computer vision models in tensorflow. <br>
+[![PyPI](https://img.shields.io/pypi/v/multi-scale-expansion)](https://pypi.org/project/multi-scale-expansion/)
 ![image](https://img.shields.io/pypi/l/tensorflow)
 ![image](https://img.shields.io/github/issues/ColumbiaMancera/multi-scale-expansion)
 ![Build Status](https://github.com/ColumbiaMancera/multi-scale-expansion/actions/workflows/build.yml/badge.svg)
 [![codecov](https://codecov.io/gh/ColumbiaMancera/multi-scale-expansion/branch/main/graph/badge.svg)](https://codecov.io/gh/ColumbiaMancera/multi-scale-expansion)
+[![Docs](https://img.shields.io/badge/docs-passing-success)](https://columbiamancera.github.io/multi-scale-expansion/)
 
 ## Overview
 `multi-scale-expansion` is a library for automating the set up of an image classification model. The user provides their data, and the library creates and trains a ready-to-use model to complete the image classification task and apply it to any image further. The objective is that this framework can be automated and applied for recognizing whether a plant is healthy or not, through the use of the models we train. 
 
 ## Contributions
 For instructions on how to contribute, go to the [Contribution Guidelines Page](https://github.com/ColumbiaMancera/multi-scale-expansion/blob/main/CONTRIBUTING.md). 
 
@@ -63,54 +65,37 @@
 ```
 
 To install library: 
 ```bash
 $ pip install multi-scale-expansion
 ```
 
-## Quick-Start Example
+## Quick-Start Example 
 ```python 
-import torch
-from torchvision import models
-import numpy as np
-import matplotlib
-from PIL import Image
-import importlib
-
-ms_model = importlib.import_module("multi-scale-expansion.model")
-ms_datasets = importlib.import_module("multi-scale-expansion.dataset")
-ms = importlib.import_module("multi-scale-expansion.classification")
 
-device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-mock_model = models.resnet18(weights='DEFAULT')
+# Provide a pytorch pre-trained image classification model! 
 mock_model = ms_model.get_plant_model(mock_model, list(range(6))
 
-mock_lr = 0.001
-mock_momentum = 0.9
-mock_step_size = 7
-mock_gamma = 0.1
+# Specify these values - fine-tune at your will!
 mock_criterion, mock_optimizer, mock_lr_scheduler = get_train_loss_needs(
     mock_model, mock_lr, mock_momentum, mock_step_size, mock_gamma
 )
 
-mock_datasets = {
-    "train": FakeData(num_classes=6, transform=mock_transforms["train"]),
-    "test": FakeData(num_classes=6, transform=mock_transforms["test"]),
-}
-
-mock_dataset_sizes = {x: len(mock_datasets[x]) for x in ['train', 'test']}
+# Get dataloaders from datasets
 mock_dataloaders = ms_datasets.get_dataloaders(mock_datasets)
 
+# Fine-tune your pre-trained model! 
 model, train_losses, train_accuracies, val_losses, val_accuracies = ms.train_model(
     device,
     mock_dataset_sizes,
     mock_dataloaders,
     mock_model,
     mock_criterion,
     mock_optimizer,
     mock_lr_scheduler,
     num_epochs=1,
     testing=True,
 )
 ```
 
-And now your model is ready-to-use! 
+And now your model is ready-to-use for your image classification task! 
+Soon, you'll be able to just call a single method and the library will set up the whole classification task for you!
```

### Comparing `multi-scale-expansion-0.1.1/README.md` & `multi-scale-expansion-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Multi Scale Expansion
 Repository to create framework for image classification computer vision models in tensorflow. <br>
+[![PyPI](https://img.shields.io/pypi/v/multi-scale-expansion)](https://pypi.org/project/multi-scale-expansion/)
 ![image](https://img.shields.io/pypi/l/tensorflow)
 ![image](https://img.shields.io/github/issues/ColumbiaMancera/multi-scale-expansion)
 ![Build Status](https://github.com/ColumbiaMancera/multi-scale-expansion/actions/workflows/build.yml/badge.svg)
 [![codecov](https://codecov.io/gh/ColumbiaMancera/multi-scale-expansion/branch/main/graph/badge.svg)](https://codecov.io/gh/ColumbiaMancera/multi-scale-expansion)
+[![Docs](https://img.shields.io/badge/docs-passing-success)](https://columbiamancera.github.io/multi-scale-expansion/)
 
 ## Overview
 `multi-scale-expansion` is a library for automating the set up of an image classification model. The user provides their data, and the library creates and trains a ready-to-use model to complete the image classification task and apply it to any image further. The objective is that this framework can be automated and applied for recognizing whether a plant is healthy or not, through the use of the models we train. 
 
 ## Contributions
 For instructions on how to contribute, go to the [Contribution Guidelines Page](https://github.com/ColumbiaMancera/multi-scale-expansion/blob/main/CONTRIBUTING.md). 
 
@@ -29,54 +31,37 @@
 ```
 
 To install library: 
 ```bash
 $ pip install multi-scale-expansion
 ```
 
-## Quick-Start Example
+## Quick-Start Example 
 ```python 
-import torch
-from torchvision import models
-import numpy as np
-import matplotlib
-from PIL import Image
-import importlib
-
-ms_model = importlib.import_module("multi-scale-expansion.model")
-ms_datasets = importlib.import_module("multi-scale-expansion.dataset")
-ms = importlib.import_module("multi-scale-expansion.classification")
 
-device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-mock_model = models.resnet18(weights='DEFAULT')
+# Provide a pytorch pre-trained image classification model! 
 mock_model = ms_model.get_plant_model(mock_model, list(range(6))
 
-mock_lr = 0.001
-mock_momentum = 0.9
-mock_step_size = 7
-mock_gamma = 0.1
+# Specify these values - fine-tune at your will!
 mock_criterion, mock_optimizer, mock_lr_scheduler = get_train_loss_needs(
     mock_model, mock_lr, mock_momentum, mock_step_size, mock_gamma
 )
 
-mock_datasets = {
-    "train": FakeData(num_classes=6, transform=mock_transforms["train"]),
-    "test": FakeData(num_classes=6, transform=mock_transforms["test"]),
-}
-
-mock_dataset_sizes = {x: len(mock_datasets[x]) for x in ['train', 'test']}
+# Get dataloaders from datasets
 mock_dataloaders = ms_datasets.get_dataloaders(mock_datasets)
 
+# Fine-tune your pre-trained model! 
 model, train_losses, train_accuracies, val_losses, val_accuracies = ms.train_model(
     device,
     mock_dataset_sizes,
     mock_dataloaders,
     mock_model,
     mock_criterion,
     mock_optimizer,
     mock_lr_scheduler,
     num_epochs=1,
     testing=True,
 )
 ```
 
-And now your model is ready-to-use! 
+And now your model is ready-to-use for your image classification task! 
+Soon, you'll be able to just call a single method and the library will set up the whole classification task for you!
```

### Comparing `multi-scale-expansion-0.1.1/multi_scale_expansion.egg-info/PKG-INFO` & `multi-scale-expansion-0.1.2/multi_scale_expansion.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-scale-expansion
-Version: 0.1.1
+Version: 0.1.2
 Summary: Check whether your plants are healthy using image classification
 Author-email: Angel Mancera <aem2283@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Angel Mancera
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,18 +30,20 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # Multi Scale Expansion
 Repository to create framework for image classification computer vision models in tensorflow. <br>
+[![PyPI](https://img.shields.io/pypi/v/multi-scale-expansion)](https://pypi.org/project/multi-scale-expansion/)
 ![image](https://img.shields.io/pypi/l/tensorflow)
 ![image](https://img.shields.io/github/issues/ColumbiaMancera/multi-scale-expansion)
 ![Build Status](https://github.com/ColumbiaMancera/multi-scale-expansion/actions/workflows/build.yml/badge.svg)
 [![codecov](https://codecov.io/gh/ColumbiaMancera/multi-scale-expansion/branch/main/graph/badge.svg)](https://codecov.io/gh/ColumbiaMancera/multi-scale-expansion)
+[![Docs](https://img.shields.io/badge/docs-passing-success)](https://columbiamancera.github.io/multi-scale-expansion/)
 
 ## Overview
 `multi-scale-expansion` is a library for automating the set up of an image classification model. The user provides their data, and the library creates and trains a ready-to-use model to complete the image classification task and apply it to any image further. The objective is that this framework can be automated and applied for recognizing whether a plant is healthy or not, through the use of the models we train. 
 
 ## Contributions
 For instructions on how to contribute, go to the [Contribution Guidelines Page](https://github.com/ColumbiaMancera/multi-scale-expansion/blob/main/CONTRIBUTING.md). 
 
@@ -63,54 +65,37 @@
 ```
 
 To install library: 
 ```bash
 $ pip install multi-scale-expansion
 ```
 
-## Quick-Start Example
+## Quick-Start Example 
 ```python 
-import torch
-from torchvision import models
-import numpy as np
-import matplotlib
-from PIL import Image
-import importlib
-
-ms_model = importlib.import_module("multi-scale-expansion.model")
-ms_datasets = importlib.import_module("multi-scale-expansion.dataset")
-ms = importlib.import_module("multi-scale-expansion.classification")
 
-device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-mock_model = models.resnet18(weights='DEFAULT')
+# Provide a pytorch pre-trained image classification model! 
 mock_model = ms_model.get_plant_model(mock_model, list(range(6))
 
-mock_lr = 0.001
-mock_momentum = 0.9
-mock_step_size = 7
-mock_gamma = 0.1
+# Specify these values - fine-tune at your will!
 mock_criterion, mock_optimizer, mock_lr_scheduler = get_train_loss_needs(
     mock_model, mock_lr, mock_momentum, mock_step_size, mock_gamma
 )
 
-mock_datasets = {
-    "train": FakeData(num_classes=6, transform=mock_transforms["train"]),
-    "test": FakeData(num_classes=6, transform=mock_transforms["test"]),
-}
-
-mock_dataset_sizes = {x: len(mock_datasets[x]) for x in ['train', 'test']}
+# Get dataloaders from datasets
 mock_dataloaders = ms_datasets.get_dataloaders(mock_datasets)
 
+# Fine-tune your pre-trained model! 
 model, train_losses, train_accuracies, val_losses, val_accuracies = ms.train_model(
     device,
     mock_dataset_sizes,
     mock_dataloaders,
     mock_model,
     mock_criterion,
     mock_optimizer,
     mock_lr_scheduler,
     num_epochs=1,
     testing=True,
 )
 ```
 
-And now your model is ready-to-use! 
+And now your model is ready-to-use for your image classification task! 
+Soon, you'll be able to just call a single method and the library will set up the whole classification task for you!
```

### Comparing `multi-scale-expansion-0.1.1/pyproject.toml` & `multi-scale-expansion-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "multi-scale-expansion"
 authors = [{name = "Angel Mancera", email = "aem2283@columbia.edu"}]
 description="Check whether your plants are healthy using image classification"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Programming Language :: Python :: 3.10",
 ]
```

