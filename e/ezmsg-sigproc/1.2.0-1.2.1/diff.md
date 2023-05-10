# Comparing `tmp/ezmsg-sigproc-1.2.0.tar.gz` & `tmp/ezmsg-sigproc-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmsg-sigproc-1.2.0.tar", last modified: Wed Mar 29 20:03:05 2023, max compression
+gzip compressed data, was "ezmsg-sigproc-1.2.1.tar", last modified: Wed May 10 14:22:15 2023, max compression
```

## Comparing `ezmsg-sigproc-1.2.0.tar` & `ezmsg-sigproc-1.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:05.303068 ezmsg-sigproc-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-29 20:03:05.303068 ezmsg-sigproc-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:05.291067 ezmsg-sigproc-1.2.0/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:05.299068 ezmsg-sigproc-1.2.0/ezmsg/sigproc/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/butterworthfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/ewmfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/synth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/ezmsg/sigproc/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:05.299068 ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-29 20:03:05.000000 ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-29 20:03:05.000000 ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 20:03:05.000000 ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 20:03:05.000000 ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-29 20:03:05.000000 ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-29 20:03:05.000000 ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-29 20:03:05.303068 ezmsg-sigproc-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 20:03:05.303068 ezmsg-sigproc-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/tests/test_butterworth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/tests/test_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-03-29 20:02:53.000000 ezmsg-sigproc-1.2.0/tests/test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:22:15.342675 ezmsg-sigproc-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 14:22:15.342675 ezmsg-sigproc-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:22:15.330675 ezmsg-sigproc-1.2.1/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:22:15.338675 ezmsg-sigproc-1.2.1/ezmsg/sigproc/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/butterworthfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/ewmfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/ezmsg/sigproc/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:22:15.338675 ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 14:22:15.000000 ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-10 14:22:15.000000 ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:22:15.000000 ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:22:15.000000 ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 14:22:15.000000 ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-10 14:22:15.000000 ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-10 14:22:15.342675 ezmsg-sigproc-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:22:15.342675 ezmsg-sigproc-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/tests/test_butterworth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/tests/test_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-10 14:22:00.000000 ezmsg-sigproc-1.2.1/tests/test_window.py
```

### Comparing `ezmsg-sigproc-1.2.0/LICENSE.txt` & `ezmsg-sigproc-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/PKG-INFO` & `ezmsg-sigproc-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg-sigproc
-Version: 1.2.0
+Version: 1.2.1
 Summary: Timeseries signal processing implementations in ezmsg
 Home-page: https://github.com/iscoe/ezmsg
 Author: Griffin Milsap
 Author-email: griffin.milsap@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/butterworthfilter.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/butterworthfilter.py`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/decimate.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/decimate.py`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/downsample.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/downsample.py`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/ewmfilter.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/ewmfilter.py`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/filter.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class FilterState(ez.State):
     axis: Optional[str] = None
     zi: Optional[np.ndarray] = None
     filt_designed: bool = False
     filt: Optional[FilterCoefficients] = None
-    filt_set: asyncio.Event = asyncio.Event()
+    filt_set: asyncio.Event = field(default_factory=asyncio.Event)
     samp_shape: Optional[Tuple[int, ...]] = None
     fs: Optional[float] = None  # Hz
 
 
 class Filter(ez.Unit):
     SETTINGS: FilterSettingsBase
     STATE: FilterState
```

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/messages.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/messages.py`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/sampler.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,15 +237,15 @@
 
 
 class SamplerTestSystemSettings(ez.Settings):
     sampler_settings: SamplerSettings
     trigger_settings: TriggerGeneratorSettings
 
 
-class SamplerTestSystem(ez.System):
+class SamplerTestSystem(ez.Collection):
     SETTINGS: SamplerTestSystemSettings
 
     OSC = Oscillator()
     SAMPLER = Sampler()
     TRIGGER = TriggerGenerator()
     DEBUG = DebugLog()
 
@@ -280,8 +280,8 @@
         trigger_settings=TriggerGeneratorSettings(
             period=(1.0, 2.0), prewait=0.5, publish_period=5.0
         ),
     )
 
     system = SamplerTestSystem(settings)
 
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
```

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/spectral.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/spectral.py`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/synth.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/synth.py`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/ezmsg/sigproc/window.py` & `ezmsg-sigproc-1.2.1/ezmsg/sigproc/window.py`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/PKG-INFO` & `ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg-sigproc
-Version: 1.2.0
+Version: 1.2.1
 Summary: Timeseries signal processing implementations in ezmsg
 Home-page: https://github.com/iscoe/ezmsg
 Author: Griffin Milsap
 Author-email: griffin.milsap@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-sigproc-1.2.0/ezmsg_sigproc.egg-info/SOURCES.txt` & `ezmsg-sigproc-1.2.1/ezmsg_sigproc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/setup.cfg` & `ezmsg-sigproc-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ezmsg-sigproc-1.2.0/tests/test_butterworth.py` & `ezmsg-sigproc-1.2.1/tests/test_butterworth.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 import numpy as np
 
 import ezmsg.core as ez
 from ezmsg.util.messages.axisarray import AxisArray
 from ezmsg.util.messagegate import MessageGate, MessageGateSettings
 from ezmsg.util.messagelogger import MessageLogger, MessageLoggerSettings
-from ezmsg.util.messagecodec import MessageDecoder
+from ezmsg.util.messagecodec import message_log
 from ezmsg.sigproc.synth import WhiteNoise, WhiteNoiseSettings
 from ezmsg.sigproc.butterworthfilter import ButterworthFilter, ButterworthFilterSettings
 
 from util import get_test_fn
 from ezmsg.util.terminate import TerminateOnTimeout as TerminateTest
 from ezmsg.util.terminate import TerminateOnTimeoutSettings as TerminateTestSettings
 
@@ -23,15 +23,15 @@
     noise_settings: WhiteNoiseSettings
     gate_settings: MessageGateSettings
     butter_settings: ButterworthFilterSettings
     log_settings: MessageLoggerSettings
     term_settings: TerminateTestSettings
 
 
-class ButterworthSystem(ez.System):
+class ButterworthSystem(ez.Collection):
     NOISE = WhiteNoise()
     GATE = MessageGate()
     BUTTER = ButterworthFilter()
     LOG = MessageLogger()
     TERM = TerminateTest()
 
     SETTINGS: ButterworthSystemSettings
@@ -86,20 +86,19 @@
         butter_settings=ButterworthFilterSettings(order=5, cutoff=cutoff, cuton=cuton),
         log_settings=MessageLoggerSettings(output=test_filename),
         term_settings=TerminateTestSettings(time=1.0),
     )
 
     system = ButterworthSystem(settings)
 
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     messages: List[AxisArray] = []
-    with open(test_filename, "r") as file:
-        for line in file:
-            messages.append(json.loads(line, cls=MessageDecoder))
+    for msg in message_log(test_filename):
+        messages.append(msg)
 
     os.remove(test_filename)
 
     ez.logger.info(f"Analyzing recording of { len( messages ) } messages...")
 
     data = np.concatenate([msg.data for msg in messages], axis=0)
```

### Comparing `ezmsg-sigproc-1.2.0/tests/test_downsample.py` & `ezmsg-sigproc-1.2.1/tests/test_downsample.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 import numpy as np
 
 import ezmsg.core as ez
 from ezmsg.util.messages.axisarray import AxisArray
 from ezmsg.util.messagegate import MessageGate, MessageGateSettings
 from ezmsg.util.messagelogger import MessageLogger, MessageLoggerSettings
-from ezmsg.util.messagecodec import MessageDecoder
+from ezmsg.util.messagecodec import message_log
 from ezmsg.sigproc.downsample import Downsample, DownsampleSettings
 from ezmsg.sigproc.synth import Oscillator, OscillatorSettings
 
 from util import get_test_fn
 from ezmsg.util.terminate import TerminateOnTimeout as TerminateTest
 from ezmsg.util.terminate import TerminateOnTimeoutSettings as TerminateTestSettings
 from ezmsg.util.debuglog import DebugLog
@@ -24,15 +24,15 @@
     num_msgs: int
     osc_settings: OscillatorSettings
     down_settings: DownsampleSettings
     log_settings: MessageLoggerSettings
     term_settings: TerminateTestSettings
 
 
-class DownsampleSystem(ez.System):
+class DownsampleSystem(ez.Collection):
     OSC = Oscillator()
     GATE = MessageGate()
     DOWN = Downsample()
     LOG = MessageLogger()
     TERM = TerminateTest()
 
     DEBUG = DebugLog()
@@ -86,20 +86,19 @@
         down_settings=DownsampleSettings(factor=factor),
         log_settings=MessageLoggerSettings(output=test_filename),
         term_settings=TerminateTestSettings(time=1.0),
     )
 
     system = DownsampleSystem(settings)
 
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     messages: List[AxisArray] = []
-    with open(test_filename, "r") as file:
-        for line in file:
-            messages.append(json.loads(line, cls=MessageDecoder))
+    for msg in message_log(test_filename):
+        messages.append(msg)
 
     os.remove(test_filename)
 
     ez.logger.info(f"Analyzing recording of { len( messages ) } messages...")
 
     fs: Optional[float] = None
     dims: Optional[List[str]] = None
```

### Comparing `ezmsg-sigproc-1.2.0/tests/test_window.py` & `ezmsg-sigproc-1.2.1/tests/test_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 import numpy as np
 import ezmsg.core as ez
 
 from ezmsg.util.messages.axisarray import AxisArray
 from ezmsg.util.messagegate import MessageGate, MessageGateSettings
 from ezmsg.util.messagelogger import MessageLogger, MessageLoggerSettings
-from ezmsg.util.messagecodec import MessageDecoder
+from ezmsg.util.messagecodec import message_log
 from ezmsg.sigproc.synth import Counter, CounterSettings
 from ezmsg.sigproc.window import Window, WindowSettings
 
 from util import get_test_fn
 from ezmsg.util.terminate import TerminateOnTimeout as TerminateTest
 from ezmsg.util.terminate import TerminateOnTimeoutSettings as TerminateTestSettings
 from ezmsg.util.debuglog import DebugLog
@@ -26,15 +26,15 @@
     num_msgs: int
     counter_settings: CounterSettings
     window_settings: WindowSettings
     log_settings: MessageLoggerSettings
     term_settings: TerminateTestSettings = field(default_factory=TerminateTestSettings)
 
 
-class WindowSystem(ez.System):
+class WindowSystem(ez.Collection):
     COUNTER = Counter()
     GATE = MessageGate()
     WIN = Window()
     LOG = MessageLogger()
     TERM = TerminateTest()
 
     DEBUG = DebugLog()
@@ -90,20 +90,19 @@
         window_settings=WindowSettings(window_dur=win_dur, window_shift=win_shift),
         log_settings=MessageLoggerSettings(output=test_filename),
         term_settings=TerminateTestSettings(time=1.0),  # sec
     )
 
     system = WindowSystem(settings)
 
-    ez.run_system(system)
+    ez.run(SYSTEM = system)
 
     messages: List[AxisArray] = []
-    with open(test_filename, "r") as file:
-        for line in file:
-            messages.append(json.loads(line, cls=MessageDecoder))
+    for msg in message_log(test_filename):
+        messages.append(msg)
 
     os.remove(test_filename)
 
     ez.logger.info(f"Analyzing recording of { len( messages ) } messages...")
 
     fs: Optional[float] = None
     dims: Optional[List[str]] = None
```

