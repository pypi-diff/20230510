# Comparing `tmp/mountainsort5-0.1.5.tar.gz` & `tmp/mountainsort5-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountainsort5-0.1.5.tar", last modified: Thu Apr 13 19:18:22 2023, max compression
+gzip compressed data, was "mountainsort5-0.3.0.tar", last modified: Wed May 10 18:20:23 2023, max compression
```

## Comparing `mountainsort5-0.1.5.tar` & `mountainsort5-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.327712 mountainsort5-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-13 19:18:22.327712 mountainsort5-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.323712 mountainsort5-0.1.5/mountainsort5/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.323712 mountainsort5-0.1.5/mountainsort5/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/SnippetClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/branch_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/compute_pca_features.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/compute_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/detect_spikes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/extract_snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/get_block_recording_for_scheme3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/get_sampled_recording_for_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/get_times_labels_from_sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/core/remove_duplicate_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.323712 mountainsort5-0.1.5/mountainsort5/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/Scheme1SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/Scheme2SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/Scheme3SortingParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (123)    16907 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.323712 mountainsort5-0.1.5/mountainsort5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 19:18:22.000000 mountainsort5-0.1.5/mountainsort5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 19:18:22.327712 mountainsort5-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 19:18:22.327712 mountainsort5-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/tests/test_scheme1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/tests/test_scheme2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-13 19:17:18.000000 mountainsort5-0.1.5/tests/test_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:23.652221 mountainsort5-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-10 18:20:23.652221 mountainsort5-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:23.644221 mountainsort5-0.3.0/mountainsort5/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:23.648221 mountainsort5-0.3.0/mountainsort5/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/SnippetClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/compute_pca_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/compute_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/detect_spikes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/extract_snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/get_block_recording_for_scheme3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/get_sampled_recording_for_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/get_times_labels_from_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/isosplit6_subdivision_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/core/remove_duplicate_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:23.652221 mountainsort5-0.3.0/mountainsort5/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/schemes/Scheme1SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/schemes/Scheme2SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/schemes/Scheme3SortingParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9703 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/schemes/sorting_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16990 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/schemes/sorting_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/mountainsort5/schemes/sorting_scheme3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:23.644221 mountainsort5-0.3.0/mountainsort5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-10 18:20:23.000000 mountainsort5-0.3.0/mountainsort5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-10 18:20:23.000000 mountainsort5-0.3.0/mountainsort5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:20:23.000000 mountainsort5-0.3.0/mountainsort5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 18:20:23.000000 mountainsort5-0.3.0/mountainsort5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 18:20:23.000000 mountainsort5-0.3.0/mountainsort5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:20:23.652221 mountainsort5-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:20:23.652221 mountainsort5-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/tests/test_scheme1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/tests/test_scheme2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-10 18:18:52.000000 mountainsort5-0.3.0/tests/test_scheme3.py
```

### Comparing `mountainsort5-0.1.5/LICENSE` & `mountainsort5-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/PKG-INFO` & `mountainsort5-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mountainsort5
-Version: 0.1.5
+Version: 0.3.0
 Summary: MountainSort 5 spike sorting algorithm
-Home-page: https://github.com/magland/mountainsort5
+Home-page: https://github.com/flatironinstitute/mountainsort5
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MountainSort 5
 
 [![latest-release](https://img.shields.io/pypi/v/mountainsort5.svg)](https://pypi.org/project/mountainsort5)
-![tests](https://github.com/magland/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
-[![codecov](https://codecov.io/gh/magland/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/magland/mountainsort5)
+![tests](https://github.com/flatironinstitute/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/flatironinstitute/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/flatironinstitute/mountainsort5)
 
 This is the most recent version of the [MountainSort](https://www.sciencedirect.com/science/article/pii/S0896627317307456) spike sorting algorithm. An implementation of the previous version of this algorithm can be [found here](https://github.com/magland/mountainsort4).
 
 * Uses [Isosplit clustering](https://github.com/magland/isosplit6)
 * Runs faster than previous versions, especially for large channel counts
 * Better handles time-overlapping events and drifting waveforms
 * Runs fast on CPU
@@ -47,15 +47,15 @@
 import mountainsort5 as ms5
 
 recording = ... # load your recording using SpikeInterface
 
 # Make sure the recording is preprocessed appropriately
 # lazy preprocessing
 recording_filtered = spre.bandpass_filter(recording, freq_min=300, freq_max=6000)
-recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered)
+recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered, dtype='float32')
 
 # use scheme 1
 sorting = ms5.sorting_scheme1(
     recording=recording_preprocessed,
     sorting_parameters=ms5.Scheme1SortingParameters(...)
 )
```

### Comparing `mountainsort5-0.1.5/README.md` & `mountainsort5-0.3.0/mountainsort5.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,22 @@
+Metadata-Version: 2.1
+Name: mountainsort5
+Version: 0.3.0
+Summary: MountainSort 5 spike sorting algorithm
+Home-page: https://github.com/flatironinstitute/mountainsort5
+Author: Jeremy Magland
+Author-email: jmagland@flatironinstitute.org
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MountainSort 5
 
 [![latest-release](https://img.shields.io/pypi/v/mountainsort5.svg)](https://pypi.org/project/mountainsort5)
-![tests](https://github.com/magland/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
-[![codecov](https://codecov.io/gh/magland/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/magland/mountainsort5)
+![tests](https://github.com/flatironinstitute/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/flatironinstitute/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/flatironinstitute/mountainsort5)
 
 This is the most recent version of the [MountainSort](https://www.sciencedirect.com/science/article/pii/S0896627317307456) spike sorting algorithm. An implementation of the previous version of this algorithm can be [found here](https://github.com/magland/mountainsort4).
 
 * Uses [Isosplit clustering](https://github.com/magland/isosplit6)
 * Runs faster than previous versions, especially for large channel counts
 * Better handles time-overlapping events and drifting waveforms
 * Runs fast on CPU
@@ -37,15 +47,15 @@
 import mountainsort5 as ms5
 
 recording = ... # load your recording using SpikeInterface
 
 # Make sure the recording is preprocessed appropriately
 # lazy preprocessing
 recording_filtered = spre.bandpass_filter(recording, freq_min=300, freq_max=6000)
-recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered)
+recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered, dtype='float32')
 
 # use scheme 1
 sorting = ms5.sorting_scheme1(
     recording=recording_preprocessed,
     sorting_parameters=ms5.Scheme1SortingParameters(...)
 )
```

### Comparing `mountainsort5-0.1.5/mountainsort5/core/SnippetClassifier.py` & `mountainsort5-0.3.0/mountainsort5/core/SnippetClassifier.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5/core/detect_spikes.py` & `mountainsort5-0.3.0/mountainsort5/core/detect_spikes.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5/core/extract_snippets.py` & `mountainsort5-0.3.0/mountainsort5/core/extract_snippets.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5/core/get_block_recording_for_scheme3.py` & `mountainsort5-0.3.0/mountainsort5/core/get_block_recording_for_scheme3.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5/core/get_sampled_recording_for_training.py` & `mountainsort5-0.3.0/mountainsort5/core/get_sampled_recording_for_training.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5/core/get_times_labels_from_sorting.py` & `mountainsort5-0.3.0/mountainsort5/core/get_times_labels_from_sorting.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5/core/remove_duplicate_events.py` & `mountainsort5-0.3.0/mountainsort5/core/remove_duplicate_events.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5/schemes/Scheme1SortingParameters.py` & `mountainsort5-0.3.0/mountainsort5/schemes/Scheme1SortingParameters.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,24 +10,26 @@
     - detect_threshold: the threshold for detection of whitened data
     - detect_channel_radius: the radius (in units of channel locations) for exluding nearby channels from detection
     - detect_time_radius_msec: the radius (in msec) for excluding nearby events from detection
     - detect_sign: the sign of the threshold for detection (1, -1, or 0)
     - snippet_T1: the number of timepoints before the event to include in the snippet
     - snippet_T2: the number of timepoints after the event to include in the snippet
     - snippet_mask_radius: the radius (in units of channel locations) for making a snippet around the central channel
-    - npca_per_branch: the number of PCA components to compute for each branch of clustering
+    - npca_per_channel: the number of PCA components per channel for initial dimension reduction
+    - npca_per_subdivision: the number of PCA components to compute for each subdivision of clustering
     """
     detect_threshold: float=5.5
     detect_channel_radius: Union[float, None]=None
     detect_time_radius_msec: float=0.5
     detect_sign: int=-1
     snippet_T1: int=20
     snippet_T2: int=20
     snippet_mask_radius: Union[float, None]=None
-    npca_per_branch: int=12
+    npca_per_channel: int=3
+    npca_per_subdivision: int=10
     pairwise_merge_step: bool=False # deprecated
 
     def check_valid(self, *, M: int, N: int, sampling_frequency: float, channel_locations: npt.NDArray[np.float32]):
         """Internal function for checking validity of parameters"""
         assert channel_locations.shape[0] == M, 'Shape mismatch between traces and channel locations'
         D = channel_locations.shape[1]
         assert N >= self.snippet_T1 + self.snippet_T2
@@ -37,9 +39,10 @@
         assert D >= 1 and D <= 3
         assert sampling_frequency > 0 and sampling_frequency <= 1e7
         if self.detect_channel_radius is not None:
             assert self.detect_channel_radius > 0
         assert self.detect_time_radius_msec > 0 and self.detect_time_radius_msec <= 1e4
         assert self.detect_threshold > 0
         assert self.detect_sign in [-1, 0, 1]
-        assert self.npca_per_branch >= 1 and self.npca_per_branch <= 1e3
+        assert self.npca_per_channel >= 1 and self.npca_per_channel <= 1e3
+        assert self.npca_per_subdivision >= 1 and self.npca_per_subdivision <= 1e3
```

### Comparing `mountainsort5-0.1.5/mountainsort5/schemes/Scheme2SortingParameters.py` & `mountainsort5-0.3.0/mountainsort5/schemes/Scheme2SortingParameters.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     See Scheme1SortingParameters for more details on the parameters below.
 
     - phase1_detect_channel_radius: detect_channel_radius in phase 1
     - detect_channel_radius: detect_channel_radius in phase 2
     - phase1_detect_threshold: detect_threshold in phase 1
     - phase1_detect_time_radius_msec: detect_time_radius_msec in phase 1
     - detect_time_radius_msec: detect_time_radius_msec in phase 2
-    - phase1_npca_per_branch: npca_per_branch in phase 1
+    - phase1_npca_per_channel: npca_per_channel in phase 1
+    - phase1_npca_per_subdivision: npca_per_subdivision in phase 1
     - detect_sign
     - detect_threshold: detect_threshold in phase 2
     - snippet_T1
     - snippet_T2
     - snippet_mask_radius
     - max_num_snippets_per_training_batch: the maximum number of snippets to use for training the classifier in each batch
     - classifier_npca: the number of principal components to use for each neighborhood classifier
@@ -27,15 +28,17 @@
     - training_recording_sampling_mode: how to sample the training data. If 'initial', then the first training_duration_sec of the recording will be used. If 'uniform', then the training data will be sampled uniformly in 10-second chunks from the recording.
     """
     phase1_detect_channel_radius: Union[float, None]
     detect_channel_radius: Union[float, None]
     phase1_detect_threshold: float=5.5
     phase1_detect_time_radius_msec: float=1.5
     detect_time_radius_msec: float=0.5
-    phase1_npca_per_branch: int=12
+    phase1_npca_per_channel: int=3
+    phase1_npca_per_subdivision: int=10
+    subdivision: int=10
     phase1_pairwise_merge_step: bool=False # deprecated
     detect_sign: int=-1
     detect_threshold: float=5.5
     snippet_T1: int=20
     snippet_T2: int=20
     snippet_mask_radius: Union[float, None]=None
     max_num_snippets_per_training_batch: int=200
@@ -54,9 +57,10 @@
         assert D >= 1 and D <= 3
         assert sampling_frequency > 0 and sampling_frequency <= 1e7
         if self.phase1_detect_channel_radius is not None:
             assert self.phase1_detect_channel_radius > 0
         assert self.phase1_detect_time_radius_msec > 0 and self.phase1_detect_time_radius_msec <= 1e4
         assert self.phase1_detect_threshold > 0
         assert self.detect_sign in [-1, 0, 1]
-        assert self.phase1_npca_per_branch >= 1 and self.phase1_npca_per_branch <= 1e3
+        assert self.phase1_npca_per_channel >=1 and self.phase1_npca_per_channel <= 1e3
+        assert self.phase1_npca_per_subdivision >= 1 and self.phase1_npca_per_subdivision <= 1e3
```

### Comparing `mountainsort5-0.1.5/mountainsort5/schemes/Scheme3SortingParameters.py` & `mountainsort5-0.3.0/mountainsort5/schemes/Scheme3SortingParameters.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme1.py` & `mountainsort5-0.3.0/mountainsort5/schemes/sorting_scheme1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import numpy.typing as npt
 import math
 import spikeinterface as si
 from .Scheme1SortingParameters import Scheme1SortingParameters
 from ..core.detect_spikes import detect_spikes
 from ..core.extract_snippets import extract_snippets
-from ..core.branch_cluster import branch_cluster
+from ..core.isosplit6_subdivision_method import isosplit6_subdivision_method
 from ..core.compute_templates import compute_templates
+from ..core.compute_pca_features import compute_pca_features
 
 
 def sorting_scheme1(
     recording: si.BaseRecording, *,
     sorting_parameters: Scheme1SortingParameters
 ):
     """MountainSort 5 sorting scheme 1
@@ -79,17 +80,18 @@
         T2=sorting_parameters.snippet_T2
     )
     L = snippets.shape[0]
     T = snippets.shape[1]
     assert snippets.shape[2] == M
 
     print('Clustering snippets')
-    labels = branch_cluster(
-        X=snippets.reshape((L, T * M)),
-        npca_per_branch=sorting_parameters.npca_per_branch
+    features = compute_pca_features(snippets.reshape((L, T * M)), npca=sorting_parameters.npca_per_channel * M)
+    labels = isosplit6_subdivision_method(
+        X=features,
+        npca_per_subdivision=sorting_parameters.npca_per_subdivision
     )
     K = int(np.max(labels))
     print(f'Found {K} clusters')
 
     print('Computing templates')
     templates = compute_templates(snippets=snippets, labels=labels) # K x T x M
     peak_channel_indices = [np.argmin(np.min(templates[i], axis=0)) for i in range(K)]
@@ -99,17 +101,18 @@
 
     print('Aligning snippets')
     snippets = align_snippets(snippets, offsets, labels)
     # this is tricky - we need to subtract the offset to correspond to shifting the template
     times = offset_times(times, -offsets, labels)
 
     print('Clustering aligned snippets')
-    labels = branch_cluster(
-        X=snippets.reshape((L, T * M)),
-        npca_per_branch=sorting_parameters.npca_per_branch
+    features = compute_pca_features(snippets.reshape((L, T * M)), npca=sorting_parameters.npca_per_channel * M)
+    labels = isosplit6_subdivision_method(
+        X=features,
+        npca_per_subdivision=sorting_parameters.npca_per_subdivision
     )
     K = int(np.max(labels))
     print(f'Found {K} clusters')
 
     print('Computing templates')
     templates = compute_templates(snippets=snippets, labels=labels) # K x T x M
     peak_channel_indices = [np.argmin(np.min(templates[i], axis=0)) for i in range(K)]
```

### Comparing `mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme2.py` & `mountainsort5-0.3.0/mountainsort5/schemes/sorting_scheme2.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,16 @@
             detect_threshold=sorting_parameters.phase1_detect_threshold,
             detect_sign=sorting_parameters.detect_sign,
             detect_time_radius_msec=sorting_parameters.phase1_detect_time_radius_msec,
             detect_channel_radius=sorting_parameters.phase1_detect_channel_radius,
             snippet_mask_radius=sorting_parameters.snippet_mask_radius,
             snippet_T1=sorting_parameters.snippet_T1,
             snippet_T2=sorting_parameters.snippet_T2,
-            npca_per_branch=sorting_parameters.phase1_npca_per_branch
+            npca_per_channel=sorting_parameters.phase1_npca_per_channel,
+            npca_per_subdivision=sorting_parameters.phase1_npca_per_subdivision
         )
     )
     times, labels = get_times_labels_from_sorting(sorting1)
     K = np.max(labels) # number of clusters
     labels = labels + label_offset # used in scheme 3
 
     print('Loading training traces')
```

### Comparing `mountainsort5-0.1.5/mountainsort5/schemes/sorting_scheme3.py` & `mountainsort5-0.3.0/mountainsort5/schemes/sorting_scheme3.py`

 * *Files identical despite different names*

### Comparing `mountainsort5-0.1.5/mountainsort5.egg-info/PKG-INFO` & `mountainsort5-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,12 @@
-Metadata-Version: 2.1
-Name: mountainsort5
-Version: 0.1.5
-Summary: MountainSort 5 spike sorting algorithm
-Home-page: https://github.com/magland/mountainsort5
-Author: Jeremy Magland
-Author-email: jmagland@flatironinstitute.org
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MountainSort 5
 
 [![latest-release](https://img.shields.io/pypi/v/mountainsort5.svg)](https://pypi.org/project/mountainsort5)
-![tests](https://github.com/magland/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
-[![codecov](https://codecov.io/gh/magland/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/magland/mountainsort5)
+![tests](https://github.com/flatironinstitute/mountainsort5/actions/workflows/integration_tests.yml/badge.svg)
+[![codecov](https://codecov.io/gh/flatironinstitute/mountainsort5/branch/main/graph/badge.svg?token=RTENQMNXKQ)](https://codecov.io/gh/flatironinstitute/mountainsort5)
 
 This is the most recent version of the [MountainSort](https://www.sciencedirect.com/science/article/pii/S0896627317307456) spike sorting algorithm. An implementation of the previous version of this algorithm can be [found here](https://github.com/magland/mountainsort4).
 
 * Uses [Isosplit clustering](https://github.com/magland/isosplit6)
 * Runs faster than previous versions, especially for large channel counts
 * Better handles time-overlapping events and drifting waveforms
 * Runs fast on CPU
@@ -47,15 +37,15 @@
 import mountainsort5 as ms5
 
 recording = ... # load your recording using SpikeInterface
 
 # Make sure the recording is preprocessed appropriately
 # lazy preprocessing
 recording_filtered = spre.bandpass_filter(recording, freq_min=300, freq_max=6000)
-recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered)
+recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered, dtype='float32')
 
 # use scheme 1
 sorting = ms5.sorting_scheme1(
     recording=recording_preprocessed,
     sorting_parameters=ms5.Scheme1SortingParameters(...)
 )
```

### Comparing `mountainsort5-0.1.5/mountainsort5.egg-info/SOURCES.txt` & `mountainsort5-0.3.0/mountainsort5.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 mountainsort5.egg-info/PKG-INFO
 mountainsort5.egg-info/SOURCES.txt
 mountainsort5.egg-info/dependency_links.txt
 mountainsort5.egg-info/requires.txt
 mountainsort5.egg-info/top_level.txt
 mountainsort5/core/SnippetClassifier.py
 mountainsort5/core/__init__.py
-mountainsort5/core/branch_cluster.py
 mountainsort5/core/compute_pca_features.py
 mountainsort5/core/compute_templates.py
 mountainsort5/core/detect_spikes.py
 mountainsort5/core/extract_snippets.py
 mountainsort5/core/get_block_recording_for_scheme3.py
 mountainsort5/core/get_sampled_recording_for_training.py
 mountainsort5/core/get_times_labels_from_sorting.py
+mountainsort5/core/isosplit6_subdivision_method.py
 mountainsort5/core/remove_duplicate_events.py
 mountainsort5/schemes/Scheme1SortingParameters.py
 mountainsort5/schemes/Scheme2SortingParameters.py
 mountainsort5/schemes/Scheme3SortingParameters.py
 mountainsort5/schemes/__init__.py
 mountainsort5/schemes/sorting_scheme1.py
 mountainsort5/schemes/sorting_scheme2.py
```

### Comparing `mountainsort5-0.1.5/setup.py` & `mountainsort5-0.3.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 # read the contents of README.md
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = '0.1.5'
+__version__ = '0.3.0'
 
 setup(
     name='mountainsort5',
     version=__version__,
     author="Jeremy Magland",
     author_email="jmagland@flatironinstitute.org",
-    url="https://github.com/magland/mountainsort5",
+    url="https://github.com/flatironinstitute/mountainsort5",
     description="MountainSort 5 spike sorting algorithm",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'spikeinterface>=0.97.1',
         'isosplit6>=0.1.0',
```

### Comparing `mountainsort5-0.1.5/tests/test_core.py` & `mountainsort5-0.3.0/tests/test_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import spikeinterface.extractors as se
 from mountainsort5.core.compute_pca_features import compute_pca_features
 from mountainsort5.core.compute_templates import compute_templates
 from mountainsort5.core.detect_spikes import detect_spikes
 from mountainsort5.core.extract_snippets import extract_snippets, extract_snippets_in_channel_neighborhood
 from mountainsort5.core.get_sampled_recording_for_training import get_sampled_recording_for_training
 from mountainsort5.core.get_block_recording_for_scheme3 import get_block_recording_for_scheme3
-from mountainsort5.core.branch_cluster import branch_cluster
+from mountainsort5.core.isosplit6_subdivision_method import isosplit6_subdivision_method
 from mountainsort5.core.get_times_labels_from_sorting import get_times_labels_from_sorting
 
 
 def test_compute_pca_features():
     x = np.random.normal(size=(100, 20))
     features = compute_pca_features(x, npca=10)
     assert features.shape == (100, 10)
@@ -156,27 +156,27 @@
         end_frame=20 * recording.sampling_frequency
     )
     assert np.array_equal(
         recording.get_traces(start_frame=10 * recording.sampling_frequency, end_frame=20 * recording.sampling_frequency),
         recording2.get_traces()
     )
 
-def test_branch_cluster():
+def test_subdivision_cluster():
     N = 1000
     L = 100
     M = 4
     T1 = 20
     T2 = 20
     traces = np.random.normal(size=(N, M))
     traces[500:] += 10 # offset this so we get more than one cluster (important for coverage of cluster_snippets)
     times = np.random.randint(T1, N - T2, size=(L,))
     snippets = extract_snippets(traces, times=times, channel_locations=None, mask_radius=None, channel_indices=None, T1=T1, T2=T2)
-    labels = branch_cluster(
+    labels = isosplit6_subdivision_method(
         snippets.reshape((L, M * (T1 + T2))),
-        npca_per_branch=10
+        npca_per_subdivision=10
     )
     assert np.min(labels) == 1
     assert len(labels) == L
 
 def test_get_times_labels_from_sorting():
     recording, sorting = se.toy_example(duration=6, num_channels=4, num_units=10, sampling_frequency=30000, seed=0, num_segments=1)
     recording: si.BaseRecording = recording
```

### Comparing `mountainsort5-0.1.5/tests/test_scheme1.py` & `mountainsort5-0.3.0/tests/test_scheme1.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         seed=0
     )
 
     timer = time.time()
 
     # lazy preprocessing
     recording_filtered = spre.bandpass_filter(recording, freq_min=300, freq_max=6000)
-    recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered)
+    recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered, dtype='float32')
 
     # sorting
     print('Starting MountainSort5')
     sorting = ms5.sorting_scheme1(
         recording_preprocessed,
         sorting_parameters=ms5.Scheme1SortingParameters(
             snippet_mask_radius=50
```

### Comparing `mountainsort5-0.1.5/tests/test_scheme2.py` & `mountainsort5-0.3.0/tests/test_scheme2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         sampling_frequency=30000,
         num_segments=2,
         seed=0
     )
 
     # lazy preprocessing
     recording_filtered = spre.bandpass_filter(recording, freq_min=300, freq_max=6000)
-    recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered)
+    recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered, dtype='float32')
 
     # sorting
     print('Starting MountainSort5 (sorting1)')
     timer = time.time()
     sorting1, classifer1 = ms5.sorting_scheme2(
         recording_preprocessed,
         sorting_parameters=ms5.Scheme2SortingParameters(
```

### Comparing `mountainsort5-0.1.5/tests/test_scheme3.py` & `mountainsort5-0.3.0/tests/test_scheme3.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         seed=0
     )
 
     timer = time.time()
 
     # lazy preprocessing
     recording_filtered = spre.bandpass_filter(recording, freq_min=300, freq_max=6000)
-    recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered)
+    recording_preprocessed: si.BaseRecording = spre.whiten(recording_filtered, dtype='float32')
 
     # sorting
     print('Starting MountainSort5')
     sorting = ms5.sorting_scheme3(
         recording_preprocessed,
         sorting_parameters=ms5.Scheme3SortingParameters(
             block_sorting_parameters=ms5.Scheme2SortingParameters(
```

