# Comparing `tmp/scipion-em-cryodrgn-3.9.tar.gz` & `tmp/scipion-em-cryodrgn-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryodrgn-3.9.tar", last modified: Mon Mar  6 14:05:39 2023, max compression
+gzip compressed data, was "scipion-em-cryodrgn-3.9.1.tar", last modified: Thu Mar 23 09:30:54 2023, max compression
```

## Comparing `scipion-em-cryodrgn-3.9.tar` & `scipion-em-cryodrgn-3.9.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:05:39.211039 scipion-em-cryodrgn-3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-03-06 14:05:39.211039 scipion-em-cryodrgn-3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:05:39.207039 scipion-em-cryodrgn-3.9/cryodrgn/
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/cryodrgn_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:05:39.207039 scipion-em-cryodrgn-3.9/cryodrgn/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/protocols/protocol_abinitio.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/protocols/protocol_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/protocols/protocol_train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:05:39.207039 scipion-em-cryodrgn-3.9/cryodrgn/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/tests/test_protocols_cryodrgn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/cryodrgn/viewers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:05:39.207039 scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-03-06 14:05:39.000000 scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-06 14:05:39.000000 scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:05:39.000000 scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 14:05:39.000000 scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-06 14:05:39.000000 scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-06 14:05:39.000000 scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 14:05:39.211039 scipion-em-cryodrgn-3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-03-06 14:04:00.000000 scipion-em-cryodrgn-3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:30:54.170326 scipion-em-cryodrgn-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-03-23 09:30:54.170326 scipion-em-cryodrgn-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:30:54.170326 scipion-em-cryodrgn-3.9.1/cryodrgn/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24306 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/cryodrgn_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:30:54.170326 scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/protocol_abinitio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/protocol_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/protocol_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:30:54.170326 scipion-em-cryodrgn-3.9.1/cryodrgn/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/tests/test_protocols_cryodrgn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9773 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/cryodrgn/viewers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 09:30:54.170326 scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-03-23 09:30:54.000000 scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-23 09:30:54.000000 scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 09:30:54.000000 scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 09:30:54.000000 scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-23 09:30:54.000000 scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 09:30:54.000000 scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 09:30:54.170326 scipion-em-cryodrgn-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-03-23 09:28:27.000000 scipion-em-cryodrgn-3.9.1/setup.py
```

### Comparing `scipion-em-cryodrgn-3.9/CHANGES.txt` & `scipion-em-cryodrgn-3.9.1/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-3.9: 
+3.9.1:
+    - use max-threads=1 for train_vae until it's fixed: https://github.com/zhonge/cryodrgn/issues/245
+3.9:
     - add cryoDRGN2 protocol for ab initio reconstruction
     - fix chimera viewer
 3.8: fixing a bug related to zvalues and particle IDs: when the particle set is created from a subset and the ids of the set are not consecutive, cryodrgn fails
 3.7:
     - drop support for v<1.0.0
     - remove emtable requirement
     - update citations
```

### Comparing `scipion-em-cryodrgn-3.9/LICENSE` & `scipion-em-cryodrgn-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/PKG-INFO` & `scipion-em-cryodrgn-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryodrgn
-Version: 3.9
+Version: 3.9.1
 Summary: Plugin to use cryoDRGN within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryodrgn
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryodrgn/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryodrgn/
```

### Comparing `scipion-em-cryodrgn-3.9/README.rst` & `scipion-em-cryodrgn-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/__init__.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import pwem
 import pyworkflow.utils as pwutils
 from pyworkflow import Config
 
 from .constants import *
 
 
-__version__ = '3.9'
+__version__ = '3.9.1'
 _references = ['Zhong2020', 'Zhong2021', 'Zhong2021b', 'Kinman2022']
 _logo = "cryodrgn_logo.png"
 
 
 class Plugin(pwem.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-cryodrgn"
     _supportedVersions = VERSIONS
```

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/bibtex.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/constants.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/cryodrgn_logo.png` & `scipion-em-cryodrgn-3.9.1/cryodrgn/cryodrgn_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/objects.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/protocols/__init__.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/protocols/protocol_abinitio.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/protocol_abinitio.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/protocols/protocol_base.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/protocol_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 import pyworkflow.object as pwobj
 from pwem.protocols import ProtProcessParticles
 import pwem.objects as emobj
 
-from cryodrgn import Plugin
-from cryodrgn.constants import *
+from .. import Plugin
+from ..constants import *
 
 
 class CryoDrgnProtBase(ProtProcessParticles):
     _label = None
 
     def _createFilenameTemplates(self):
         """ Centralize how files are called within the protocol. """
```

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/protocols/protocol_preprocess.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/protocol_preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 import pyworkflow.utils as pwutils
 from pyworkflow.plugin import Domain
 from pyworkflow.constants import PROD
 import pyworkflow.protocol.params as params
 from pwem.constants import ALIGN_PROJ, ALIGN_NONE
 from pwem.protocols import ProtProcessParticles
 
-from cryodrgn import Plugin
-from cryodrgn.objects import CryoDrgnParticles
+from .. import Plugin
+from ..objects import CryoDrgnParticles
 
 convert = Domain.importFromPlugin('relion.convert', doRaise=True)
 
 
 class outputs(Enum):
     outputCryoDrgnParticles = CryoDrgnParticles
```

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/protocols/protocol_train.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/protocols/protocol_train.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pyworkflow.utils as pwutils
+import pyworkflow.object as pwobj
 from pyworkflow.constants import PROD
 import pyworkflow.protocol.params as params
 
 from .protocol_base import CryoDrgnProtBase
 
 
 class CryoDrgnProtTrain(CryoDrgnProtBase):
@@ -37,14 +38,15 @@
     """
     _label = 'training VAE'
     _devStatus = PROD
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         CryoDrgnProtBase._defineParams(self, form)
+        form.getParam('numberOfThreads').default = pwobj.Integer(1)
 
     def _defineAdvancedParams(self, form):
         form.addSection(label='Advanced')
         group = form.addGroup('Encoder')
         group.addParam('qLayers', params.IntParam, default=3,
                        label='Number of hidden layers')
         group.addParam('qDim', params.IntParam, default=1024,
```

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/tests/__init__.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/tests/test_protocols_cryodrgn.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/tests/test_protocols_cryodrgn.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/utils.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/cryodrgn/viewers.py` & `scipion-em-cryodrgn-3.9.1/cryodrgn/viewers.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from pyworkflow.protocol.params import (LabelParam, EnumParam,
                                         IntParam, BooleanParam)
 from pyworkflow.protocol.executor import StepExecutor
 from pyworkflow.viewer import DESKTOP_TKINTER
 from pwem.viewers import ObjectView, ChimeraView, EmProtocolViewer
 
-from cryodrgn import Plugin
+from . import Plugin
 from .protocols import CryoDrgnProtTrain, CryoDrgnProtAbinitio
 from .constants import *
 
 
 class CryoDrgnViewer(EmProtocolViewer):
     """ Visualization of cryoDRGN results. """
```

### Comparing `scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/PKG-INFO` & `scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryodrgn
-Version: 3.9
+Version: 3.9.1
 Summary: Plugin to use cryoDRGN within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryodrgn
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryodrgn/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryodrgn/
```

### Comparing `scipion-em-cryodrgn-3.9/scipion_em_cryodrgn.egg-info/SOURCES.txt` & `scipion-em-cryodrgn-3.9.1/scipion_em_cryodrgn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-cryodrgn-3.9/setup.py` & `scipion-em-cryodrgn-3.9.1/setup.py`

 * *Files identical despite different names*

