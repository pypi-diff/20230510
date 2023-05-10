# Comparing `tmp/samplestamps-0.4.4.tar.gz` & `tmp/samplestamps-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samplestamps-0.4.4.tar", last modified: Tue Oct 12 12:47:08 2021, max compression
+gzip compressed data, was "samplestamps-0.5.0.tar", last modified: Wed May 10 11:48:13 2023, max compression
```

## Comparing `samplestamps-0.4.4.tar` & `samplestamps-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3358 2021-10-12 12:45:46.854751 samplestamps-0.4.4/.github/workflows/publish.yml
--rwxr-xr-x   0        0        0     1554 2021-10-12 12:45:46.854751 samplestamps-0.4.4/.gitignore
--rw-r--r--   0        0        0    10255 2021-10-12 12:45:46.854751 samplestamps-0.4.4/LICENSE
--rw-r--r--   0        0        0      566 2021-10-12 12:45:46.854751 samplestamps-0.4.4/README.md
--rwxr-xr-x   0        0        0      235 2021-10-12 12:45:46.854751 samplestamps-0.4.4/conda/samplestamps/bld.bat
--rwxr-xr-x   0        0        0      219 2021-10-12 12:45:46.854751 samplestamps-0.4.4/conda/samplestamps/build.sh
--rwxr-xr-x   0        0        0        0 2021-10-12 12:45:46.854751 samplestamps-0.4.4/conda/samplestamps/conda_build_config.yaml
--rwxr-xr-x   0        0        0      846 2021-10-12 12:45:46.854751 samplestamps-0.4.4/conda/samplestamps/meta.yaml
--rwxr-xr-x   0        0        0   339652 2021-10-12 12:45:46.858751 samplestamps-0.4.4/demo/samplestamps.ipynb
--rw-r--r--   0        0        0      496 2021-10-12 12:45:46.858751 samplestamps-0.4.4/pyproject.toml
--rwxr-xr-x   0        0        0     1313 2021-10-12 12:45:46.858751 samplestamps-0.4.4/setup.py
--rw-r--r--   0        0        0       92 2021-10-12 12:45:46.858751 samplestamps-0.4.4/src/samplestamps/__init__.py
--rwxr-xr-x   0        0        0     3737 2021-10-12 12:45:46.858751 samplestamps-0.4.4/src/samplestamps/samplestamps.py
--rw-r--r--   0        0        0     6038 2021-10-12 12:45:46.858751 samplestamps-0.4.4/src/samplestamps/utils.py
--rwxr-xr-x   0        0        0   152688 2021-10-12 12:45:46.858751 samplestamps-0.4.4/test/localhost-20180703_182840_timeStamps.h5
--rw-r--r--   0        0        0     1790 2021-10-12 12:45:46.858751 samplestamps-0.4.4/tests/test_sampstamps.py
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 samplestamps-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1537 2023-04-15 17:49:08.000000 samplestamps-0.5.0/.github/workflows/publish.yml
+-rwxr-xr-x   0        0        0     1582 2023-04-15 17:48:28.000000 samplestamps-0.5.0/.gitignore
+-rw-r--r--   0        0        0    10255 2019-07-05 19:30:52.000000 samplestamps-0.5.0/LICENSE
+-rw-r--r--   0        0        0      566 2020-03-13 20:33:06.000000 samplestamps-0.5.0/README.md
+-rw-r--r--   0        0        0      169 2023-04-15 17:47:50.000000 samplestamps-0.5.0/build_env.yml
+-rwxr-xr-x   0        0        0        0 2021-10-06 15:43:15.000000 samplestamps-0.5.0/conda/samplestamps/conda_build_config.yaml
+-rwxr-xr-x   0        0        0      913 2022-10-29 07:55:16.000000 samplestamps-0.5.0/conda/samplestamps/meta.yaml
+-rw-r--r--   0        0        0       51 2022-09-24 07:20:14.000000 samplestamps-0.5.0/condarc.yml
+-rwxr-xr-x   0        0        0   339652 2020-02-11 12:04:15.000000 samplestamps-0.5.0/demo/samplestamps.ipynb
+-rw-r--r--   0        0        0      496 2021-10-06 16:07:50.000000 samplestamps-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0     1313 2021-06-26 12:36:19.000000 samplestamps-0.5.0/setup.py
+-rw-r--r--   0        0        0       93 2023-05-10 11:46:59.666071 samplestamps-0.5.0/src/samplestamps/__init__.py
+-rwxr-xr-x   0        0        0     4176 2023-05-10 11:46:19.029050 samplestamps-0.5.0/src/samplestamps/samplestamps.py
+-rw-r--r--   0        0        0     6476 2023-05-10 11:47:28.339624 samplestamps-0.5.0/src/samplestamps/utils.py
+-rwxr-xr-x   0        0        0   152688 2019-06-03 08:00:50.000000 samplestamps-0.5.0/tests/localhost-20180703_182840_timeStamps.h5
+-rw-r--r--   0        0        0     1790 2021-10-06 15:40:36.000000 samplestamps-0.5.0/tests/test_sampstamps.py
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 samplestamps-0.5.0/PKG-INFO
```

### Comparing `samplestamps-0.4.4/.gitignore` & `samplestamps-0.5.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -125,8 +125,9 @@
 !/docs/
 !/*.toml
 !/*.gitignore
 !/.github
 !/conda
 src/*.egg-info/
 src/*.egg-info
-
+!/build_env.yml
+!/condarc.yml
```

### Comparing `samplestamps-0.4.4/LICENSE` & `samplestamps-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `samplestamps-0.4.4/README.md` & `samplestamps-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `samplestamps-0.4.4/conda/samplestamps/meta.yaml` & `samplestamps-0.5.0/conda/samplestamps/meta.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -7,28 +7,26 @@
   version: "{{ version }}"
 
 source:
   url: "https://pypi.io/packages/source/{{ name[0] }}/{{ name }}/{{ name }}-{{ version }}.tar.gz"
 
 build:
   number: 0
+  noarch: python
+  script: python -m pip install --no-deps --ignore-installed .
 
 requirements:
-  build:
-    - python
+  host:
+    - python {{ python }}
     - pip
-    - numpy
-    - scipy
-    - git
+    - flit
   run:
-    - python
-    - pip
-    - numpy
+    - python {{ python }}
+    - numpy>1.20
     - scipy
-    - git
 
 test:
   imports:
     - samplestamps
 
 about:
   home: "https://github.com/janclemenslab/samplestamps"
```

### Comparing `samplestamps-0.4.4/demo/samplestamps.ipynb` & `samplestamps-0.5.0/demo/samplestamps.ipynb`

 * *Files identical despite different names*

### Comparing `samplestamps-0.4.4/setup.py` & `samplestamps-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `samplestamps-0.4.4/src/samplestamps/samplestamps.py` & `samplestamps-0.5.0/src/samplestamps/samplestamps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Tools for converting between samples and time stamps.
 
 glossary:
     densely stamped - each sample is consecutively time stamped
     sparsely stamped - only selected samples are time stamped - need to provide sample numbers
 """
-from .utils import monotonize, interpolator, ismonotonous
-
+from . import utils
 
 class SampStamp():
     """Converts between frames and samples."""
 
     def __init__(self, sample_times, frame_times=None, sample_numbers=None, frame_numbers=None, frame_samples=None,
                  sample_times_offset=0, frame_times_offset=0,
                  auto_monotonize=True):
@@ -45,39 +44,39 @@
         # correct for offsets
         sample_times += sample_times_offset
         if frame_times is not None:
             frame_times += frame_times_offset
 
         if auto_monotonize:
             if sample_times is not None:
-                sample_times = monotonize(sample_times)
+                sample_times = utils.monotonize(sample_times)
                 sample_numbers = sample_numbers[:sample_times.shape[0]]
             if frame_times is not None:
-                frame_times = monotonize(frame_times)
+                frame_times = utils.monotonize(frame_times)
                 frame_numbers = frame_numbers[:frame_times.shape[0]]
             if frame_samples is not None:
-                frame_samples = monotonize(frame_samples)
+                frame_samples = utils.monotonize(frame_samples)
                 # frame_numbers = frame_numbers[:frame_times.shape[0]]
 
         # get all interpolators for re-use
         if sample_numbers is not None and sample_times is not None:
-            self.samples2times = interpolator(sample_numbers, sample_times)
+            self.samples2times = utils.interpolator(sample_numbers, sample_times)
         if frame_times is None and frame_samples is not None:
             frame_times = self.samples2times(frame_samples)
             # self.frame_times = self.samples2times(frame_samples)
 
         if frame_numbers is not None and frame_times is not None:
-            self.frames2times = interpolator(frame_numbers, frame_times)
+            self.frames2times = utils.interpolator(frame_numbers, frame_times)
         if frame_times is not None and sample_numbers is not None:
-            self.times2samples = interpolator(sample_times, sample_numbers)
+            self.times2samples = utils.interpolator(sample_times, sample_numbers)
         if frame_times is not None and frame_numbers is not None:
-            self.times2frames = interpolator(frame_times, frame_numbers)
+            self.times2frames = utils.interpolator(frame_times, frame_numbers)
 
         if frame_samples is not None:
-            self.samples2frames = interpolator(frame_samples, frame_numbers, fill_value='extrapolate')
+            self.samples2frames = utils.interpolator(frame_samples, frame_numbers, fill_value='extrapolate')
 
     def frame(self, sample):
         """Get frame number from sample number."""
         return self.times2frames(self.sample_time(sample))
 
     def sample(self,  frame):
         """Get sample number from frame number."""
@@ -86,7 +85,19 @@
     def frame_time(self, frame):
         """Get time of frame number."""
         return self.frames2times(frame)
 
     def sample_time(self, sample):
         """Get time of sample number."""
         return self.samples2times(sample)
+
+
+class SimpleStamp(SampStamp):
+    """If all you need is conversion between sampling rates."""
+    def __init__(self, sampling_rate: float):
+
+        self.sampling_rate = sampling_rate
+        self.samples2times = utils.SampleInterpolator(self.sampling_rate)
+        self.times2samples = utils.SampleInterpolator(1/self.sampling_rate)
+
+        self.frames2times = self.samples2times
+        self.times2frames = self.times2samples
```

### Comparing `samplestamps-0.4.4/src/samplestamps/utils.py` & `samplestamps-0.5.0/src/samplestamps/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,14 +62,27 @@
     return x[:last_idx]
 
 
 def interpolator(x, y, fill_value='extrapolate'):
     return scipy.interpolate.interp1d(x, y, fill_value=fill_value)
 
 
+class SampleInterpolator():
+    """For samples on a regular grid"""
+
+    def __init__(self, sampling_rate: float):
+        self.sampling_rate = float(sampling_rate)
+        # dummy values for compatibililty with Interpolators from scipy.interpolate
+        self.x = np.array([0.0, 1.0])
+        self.y = self.x / self.sampling_rate
+
+    def __call__(self, sample_numbers):
+        return np.asarray(sample_numbers) / self.sampling_rate
+
+
 def time_from_log(logfilename, line_number=1):
     """Parse time stamp from a specified lines in a log file.
 
     Args:
         logfilename(str)
         line_number(int): line in the log file from which parse the time stamp (defaults to 1 - will read the first line (not 0-indexed!))
     Returns:
```

### Comparing `samplestamps-0.4.4/test/localhost-20180703_182840_timeStamps.h5` & `samplestamps-0.5.0/tests/localhost-20180703_182840_timeStamps.h5`

 * *Files identical despite different names*

### Comparing `samplestamps-0.4.4/tests/test_sampstamps.py` & `samplestamps-0.5.0/tests/test_sampstamps.py`

 * *Files identical despite different names*

### Comparing `samplestamps-0.4.4/PKG-INFO` & `samplestamps-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samplestamps
-Version: 0.4.4
+Version: 0.5.0
 Summary: For converting between timestamps.
 Home-page: https://github.com/janclemenslab/samplestamps
 Author: Jan Clemens
 Author-email: clemensjan@googlemail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

