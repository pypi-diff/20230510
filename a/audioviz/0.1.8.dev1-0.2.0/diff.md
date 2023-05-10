# Comparing `tmp/audioviz-0.1.8.dev1.tar.gz` & `tmp/audioviz-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioviz-0.1.8.dev1.tar", last modified: Mon May  8 15:30:25 2023, max compression
+gzip compressed data, was "audioviz-0.2.0.tar", last modified: Wed May 10 10:19:20 2023, max compression
```

## Comparing `audioviz-0.1.8.dev1.tar` & `audioviz-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1938 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.1.8.dev1/README.md
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/audioviz/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.1.8.dev1/audioviz/BeatAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    10474 2023-05-05 03:22:56.000000 audioviz-0.1.8.dev1/audioviz/ChordAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.1.8.dev1/audioviz/GeneralAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2165 2023-05-08 15:29:02.000000 audioviz-0.1.8.dev1/audioviz/Panel.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.1.8.dev1/audioviz/PitchAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.1.8.dev1/audioviz/StructureAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.1.8.dev1/audioviz/TimbreAnalysis.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.1.8.dev1/audioviz/__init__.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.1.8.dev1/audioviz/colabInterface.py
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.1.8.dev1/audioviz/utils.py
-drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/audioviz.egg-info/
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1938 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/PKG-INFO
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/SOURCES.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/dependency_links.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.1.8.dev1/audioviz.egg-info/not-zip-safe
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       62 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/requires.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-08 15:30:25.000000 audioviz-0.1.8.dev1/audioviz.egg-info/top_level.txt
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-08 15:30:25.067362 audioviz-0.1.8.dev1/setup.cfg
--rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1329 2023-05-08 15:29:07.000000 audioviz-0.1.8.dev1/setup.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-10 10:19:20.492996 audioviz-0.2.0/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1933 2023-05-10 10:19:20.492996 audioviz-0.2.0/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1208 2023-05-07 03:19:43.000000 audioviz-0.2.0/README.md
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-10 10:19:20.492996 audioviz-0.2.0/audioviz/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8548 2023-04-27 03:14:29.000000 audioviz-0.2.0/audioviz/BeatAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     8706 2023-05-10 10:18:06.000000 audioviz-0.2.0/audioviz/ChordAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2679 2023-04-30 07:22:36.000000 audioviz-0.2.0/audioviz/GeneralAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     2165 2023-05-09 06:50:18.000000 audioviz-0.2.0/audioviz/Panel.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     9984 2023-04-23 03:57:05.000000 audioviz-0.2.0/audioviz/PitchAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)    14126 2023-04-23 04:28:52.000000 audioviz-0.2.0/audioviz/StructureAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     6523 2023-04-23 03:57:05.000000 audioviz-0.2.0/audioviz/TimbreAnalysis.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      304 2023-05-07 07:11:37.000000 audioviz-0.2.0/audioviz/__init__.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1591 2023-04-27 03:14:12.000000 audioviz-0.2.0/audioviz/colabInterface.py
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1094 2023-05-07 03:14:17.000000 audioviz-0.2.0/audioviz/utils.py
+drwxrwxr-x   0 yulanchu  (1009) yulanchu  (1012)        0 2023-05-10 10:19:20.492996 audioviz-0.2.0/audioviz.egg-info/
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1933 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/PKG-INFO
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)      464 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/SOURCES.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/dependency_links.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        1 2023-04-27 03:19:27.000000 audioviz-0.2.0/audioviz.egg-info/not-zip-safe
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       62 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/requires.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)        9 2023-05-10 10:19:20.000000 audioviz-0.2.0/audioviz.egg-info/top_level.txt
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)       79 2023-05-10 10:19:20.492996 audioviz-0.2.0/setup.cfg
+-rw-rw-r--   0 yulanchu  (1009) yulanchu  (1012)     1324 2023-05-10 10:16:12.000000 audioviz-0.2.0/setup.py
```

### Comparing `audioviz-0.1.8.dev1/PKG-INFO` & `audioviz-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.8.dev1
+Version: 0.2.0
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.1.8.dev1/README.md` & `audioviz-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev1/audioviz/BeatAnalysis.py` & `audioviz-0.2.0/audioviz/BeatAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev1/audioviz/ChordAnalysis.py` & `audioviz-0.2.0/audioviz/ChordAnalysis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,19 @@
 import os
 import numpy as np
 import numpy.typing as npt
 from matplotlib import pyplot as plt
 
-import madmom
-from madmom.audio.chroma import DeepChromaProcessor
-from madmom.features.chords import DeepChromaChordRecognitionProcessor
 import librosa
 import libfmp.b
 import libfmp.c3
 import libfmp.c4
 
 from .colabInterface import *
 
-def simple_chord(filename: str) -> None:
-    
-    dcp = DeepChromaProcessor()
-    decode = DeepChromaChordRecognitionProcessor()
-    chroma = dcp(filename)
-    chrod_rec_res = decode(chroma)
-    
-    chord_seq = [c[2] for c in chrod_rec_res]
-    time_slice = [np.round(c[0], 1) for c in chrod_rec_res]
-    end_time = np.round(chrod_rec_res[-1][1], 1)
-    duration = np.arange(0, end_time, 0.1)
-    color_encode_list = list(set(chord_seq))
-    
-    chord_hm = np.ones((len(color_encode_list), len(duration)))
-    for i in range(1, len(time_slice)):
-        chord_hm[color_encode_list.index(chord_seq[i-1])][int(time_slice[i-1]*10):int(time_slice[i]*10)] = 0
-        
-    plt.figure(figsize=(30, 12))
-    plt.imshow(chord_hm, interpolation='none', cmap='spring', aspect='auto')
-    plt.xticks(np.arange(0, len(duration), 300), duration[::300])
-    plt.xlabel('Time (seconds)')
-    plt.yticks(np.arange(0, len(color_encode_list)), color_encode_list)
-    plt.ylabel('Chord')
-    plt.title('Chord recognition')
-
 def compute_chromagram_from_filename(fn_wav, Fs=22050, N=4096, H=2048, gamma=None, version='STFT', norm='2'):
     """Compute chromagram for WAV file specified by filename
 
     Notebook: C5/C5S2_ChordRec_Templates.ipynb
 
     Args:
         fn_wav (str): Filenname of WAV
@@ -152,29 +124,14 @@
     chord_max_index = np.argmax(chord_sim, axis=0)
     chord_max = np.zeros(chord_sim.shape).astype(np.int32)
     for n in range(chord_sim.shape[1]):
         chord_max[chord_max_index[n], n] = 1
 
     return chord_sim, chord_max
 
-def chord_decoder(wave_filename: str) -> npt.ArrayLike :
-
-    dcp = DeepChromaProcessor()
-    decode = DeepChromaChordRecognitionProcessor()
-
-    chroma = dcp(wave_filename)
-    chordDecoded = np.array(decode(chroma))
-
-    # csv formatter for rounding issues (too many 0s in )
-    for i in chordDecoded :
-        i[0] = np.round(i[0], 1)
-        i[1] = np.round(i[1], 1)
-
-    return chordDecoded
-
 def plot_chord_recognition(wave_filename: str, anno_csv: str) -> None:
 
     '''
     To plot the chord recognition results of given input
 
     wave_filename: the exact .wav filename to analyze
     anno_csv: the segment annotation .csv 
@@ -205,19 +162,14 @@
     ax[1, 0].grid()
 
     libfmp.b.plot_segments(ann, ax=ax[2, 0], time_max=x_dur, time_label='Time (seconds)',
                        colors=color_ann,  alpha=0.3)
     ax[2, 1].axis('off')
     plt.tight_layout()
 
-    # To store the result which obtained by module madmom
-    chordDetection = chord_decoder(wave_filename)
-    header_row = np.array(['Start', 'End', 'Chord'])
-    save_and_downloader('Chord.csv', header_row, chordDetection)
-
 
 def plot_binary_template_chord_recognition(wave_filename: str, anno_csv: str) -> None:
 
     '''
     To plot the binary chord recognition results of given input
 
     wave_filename: the exact .wav filename to analyze
```

### Comparing `audioviz-0.1.8.dev1/audioviz/GeneralAnalysis.py` & `audioviz-0.2.0/audioviz/GeneralAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev1/audioviz/Panel.py` & `audioviz-0.2.0/audioviz/Panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 import librosa
 import matplotlib.pyplot as plt
 
 from .ChordAnalysis import *
 
-class Dashboard():
+class Dashboard:
     
     def __init__(self, fn) -> None:
         
         self.fn = fn
         self._y, self._sr = librosa.load(fn)
         
     def simple_chord_helper(self):
 
         X, Fs_X, x, Fs, x_dur = compute_chromagram_from_filename(self.fn)
-        _, chord_max = chord_recognition_template(X, norm_sim='max', nonchord=True)
+        _, chord_max = chord_recognition_template(X, norm_sim='max', nonchord=False)
         
         return chord_max, x_dur
     
     def simple_pitch_helper(self):
         
         f0, _, _ = librosa.pyin(self._y,
                                 fmin=librosa.note_to_hz('C2'),
@@ -41,15 +41,15 @@
         ax0.set_title('Waveform')
         
         # A simple version of chord recognition
         chord_map, dur = self.simple_chord_helper()
         ax1 = fig.add_subplot(3, 1, 2)
         ax1.imshow(chord_map, interpolation='none', cmap='gray_r', aspect='auto', origin='lower')
         times = np.round(np.linspace(0, dur, chord_map.shape[1]), 1)
-        chord_labels = get_chord_labels(nonchord=True)
+        chord_labels = get_chord_labels(nonchord=False)
         ax1.set_xticks(np.arange(0, len(times), 323), times[::323])
         ax1.xaxis.set_ticklabels([])
         ax1.set_yticks(np.arange(0, len(chord_labels)), chord_labels)
         ax1.set_ylabel('Chord')
         ax1.set_title('Chord Recognition')
         
         # Pitch
```

### Comparing `audioviz-0.1.8.dev1/audioviz/PitchAnalysis.py` & `audioviz-0.2.0/audioviz/PitchAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev1/audioviz/StructureAnalysis.py` & `audioviz-0.2.0/audioviz/StructureAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev1/audioviz/TimbreAnalysis.py` & `audioviz-0.2.0/audioviz/TimbreAnalysis.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev1/audioviz/colabInterface.py` & `audioviz-0.2.0/audioviz/colabInterface.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev1/audioviz/utils.py` & `audioviz-0.2.0/audioviz/utils.py`

 * *Files identical despite different names*

### Comparing `audioviz-0.1.8.dev1/audioviz.egg-info/PKG-INFO` & `audioviz-0.2.0/audioviz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audioviz
-Version: 0.1.8.dev1
+Version: 0.2.0
 Summary: An user-friendly music information retrieval tools interfacing with Google Colab
 Home-page: https://github.com/TrangDuLam/audioviz
 Author: ayTrang
 Author-email: andrew.chuang@gapp.nthu.edu.tw
 License: MIT
 Keywords: Music Information Retrieval,Academia Sinica,NTHU
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `audioviz-0.1.8.dev1/setup.py` & `audioviz-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='audioviz',
     packages=['audioviz'],
-    version='0.1.8.dev1',
+    version='0.2.0',
     
     description='An user-friendly music information retrieval tools interfacing with Google Colab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     
     url='https://github.com/TrangDuLam/audioviz',
     author='ayTrang',
```

