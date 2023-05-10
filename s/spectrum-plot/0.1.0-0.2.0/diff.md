# Comparing `tmp/spectrum_plot-0.1.0.tar.gz` & `tmp/spectrum_plot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_plot-0.1.0.tar", last modified: Thu Feb 10 20:55:06 2022, max compression
+gzip compressed data, was "spectrum_plot-0.2.0.tar", last modified: Wed May 10 18:44:19 2023, max compression
```

## Comparing `spectrum_plot-0.1.0.tar` & `spectrum_plot-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 reut      (1000) reut      (1000)        0 2022-02-10 20:55:06.499384 spectrum_plot-0.1.0/
--rwxrwxrwx   0 reut      (1000) reut      (1000)     1097 2022-02-06 12:13:25.000000 spectrum_plot-0.1.0/LICENSE
--rwxrwxrwx   0 reut      (1000) reut      (1000)     1077 2022-02-10 20:55:06.483388 spectrum_plot-0.1.0/PKG-INFO
--rwxrwxrwx   0 reut      (1000) reut      (1000)      507 2022-02-10 20:47:37.000000 spectrum_plot-0.1.0/README.md
--rwxrwxrwx   0 reut      (1000) reut      (1000)       38 2022-02-10 20:55:06.499384 spectrum_plot-0.1.0/setup.cfg
--rwxrwxrwx   0 reut      (1000) reut      (1000)      994 2022-02-10 20:51:46.000000 spectrum_plot-0.1.0/setup.py
-drwxrwxrwx   0 reut      (1000) reut      (1000)        0 2022-02-10 20:55:06.331175 spectrum_plot-0.1.0/src/
-drwxrwxrwx   0 reut      (1000) reut      (1000)        0 2022-02-10 20:55:06.410405 spectrum_plot-0.1.0/src/spectrum_plot/
--rwxrwxrwx   0 reut      (1000) reut      (1000)      272 2022-02-10 11:11:13.000000 spectrum_plot-0.1.0/src/spectrum_plot/__init__.py
--rwxrwxrwx   0 reut      (1000) reut      (1000)     3347 2022-02-10 11:34:05.000000 spectrum_plot-0.1.0/src/spectrum_plot/plotting.py
-drwxrwxrwx   0 reut      (1000) reut      (1000)        0 2022-02-10 20:55:06.467381 spectrum_plot-0.1.0/src/spectrum_plot.egg-info/
--rwxrwxrwx   0 reut      (1000) reut      (1000)     1077 2022-02-10 20:55:04.000000 spectrum_plot-0.1.0/src/spectrum_plot.egg-info/PKG-INFO
--rwxrwxrwx   0 reut      (1000) reut      (1000)      290 2022-02-10 20:55:04.000000 spectrum_plot-0.1.0/src/spectrum_plot.egg-info/SOURCES.txt
--rwxrwxrwx   0 reut      (1000) reut      (1000)        1 2022-02-10 20:55:04.000000 spectrum_plot-0.1.0/src/spectrum_plot.egg-info/dependency_links.txt
--rwxrwxrwx   0 reut      (1000) reut      (1000)       31 2022-02-10 20:55:04.000000 spectrum_plot-0.1.0/src/spectrum_plot.egg-info/requires.txt
--rwxrwxrwx   0 reut      (1000) reut      (1000)       14 2022-02-10 20:55:04.000000 spectrum_plot-0.1.0/src/spectrum_plot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 18:44:19.475895 spectrum_plot-0.2.0/
+-rw-rw-rw-   0        0        0     1097 2022-02-06 12:13:25.000000 spectrum_plot-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1318 2023-05-10 18:44:19.474515 spectrum_plot-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2023-05-10 18:41:02.000000 spectrum_plot-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 18:44:19.475895 spectrum_plot-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      994 2023-05-10 18:43:08.000000 spectrum_plot-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:44:19.422034 spectrum_plot-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-10 18:44:19.438531 spectrum_plot-0.2.0/src/spectrum_plot/
+-rw-rw-rw-   0        0        0      272 2022-02-10 11:11:13.000000 spectrum_plot-0.2.0/src/spectrum_plot/__init__.py
+-rw-rw-rw-   0        0        0     4135 2022-02-14 19:05:38.000000 spectrum_plot-0.2.0/src/spectrum_plot/plotting.py
+drwxrwxrwx   0        0        0        0 2023-05-10 18:44:19.466515 spectrum_plot-0.2.0/src/spectrum_plot.egg-info/
+-rw-rw-rw-   0        0        0     1318 2023-05-10 18:44:19.000000 spectrum_plot-0.2.0/src/spectrum_plot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      290 2023-05-10 18:44:19.000000 spectrum_plot-0.2.0/src/spectrum_plot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 18:44:19.000000 spectrum_plot-0.2.0/src/spectrum_plot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-10 18:44:19.000000 spectrum_plot-0.2.0/src/spectrum_plot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-10 18:44:19.000000 spectrum_plot-0.2.0/src/spectrum_plot.egg-info/top_level.txt
```

### Comparing `spectrum_plot-0.1.0/LICENSE` & `spectrum_plot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_plot-0.1.0/PKG-INFO` & `spectrum_plot-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: spectrum_plot
-Version: 0.1.0
-Summary: Interactive spectrum plot. Update FFT plot on every new sampled data
-Home-page: https://github.com/lisrael1/spectrum_plot
-Author: Lior Israeli
-Author-email: israelilior@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/lisrael1/spectrum_plot/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## spectrum plot
-
-### plotting FFT of 1D data, with live plot update
-
-usage example:
-```
-    import numpy as np
-    from spectrum_plot import create_fft_plot
-    
-    
-    plot = create_fft_plot()
-    n = 200
-    seconds = 0.1
-    t = np.linspace(0, seconds, n)
-    nyquist = n / seconds / 2
-    for freq in np.linspace(100, nyquist, 100):
-        sine = np.sin(2 * np.pi * t * freq)
-        plot.update_raw_data(sine, seconds=seconds)
-```
-![](src/spectrum_plot_examples/animated_fft.gif)
-
+Metadata-Version: 2.1
+Name: spectrum_plot
+Version: 0.2.0
+Summary: Interactive spectrum plot. Update FFT plot on every new sampled data
+Home-page: https://github.com/lisrael1/spectrum_plot
+Author: Lior Israeli
+Author-email: israelilior@gmail.com
+Project-URL: Bug Tracker, https://github.com/lisrael1/spectrum_plot/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## spectrum plot
+
+### plotting FFT of 1D data, with live plot update
+
+usage example:
+```python
+import numpy as np
+from spectrum_plot import create_fft_plot
+
+
+plot = create_fft_plot()
+n = 200
+seconds = 0.1
+t = np.linspace(0, seconds, n)
+nyquist = n / seconds / 2
+for freq in np.linspace(100, nyquist, 100):
+    sine = np.sin(2 * np.pi * t * freq)
+    plot.update_raw_data(sine, seconds=seconds)
+```
+![](https://github.com/lisrael1/spectrum_plot/blob/main/src/spectrum_plot_examples/animated_fft.gif?raw=True)
+
+In the examples folder, you can locate a code that includes the addition of music notes at the graph.
+![](https://github.com/lisrael1/spectrum_plot/blob/main/src/spectrum_plot_examples/spectrom_with_notes.png?raw=True)
```

### Comparing `spectrum_plot-0.1.0/setup.py` & `spectrum_plot-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spectrum_plot",
-    version="0.1.0",
+    version="0.2.0",
     author="Lior Israeli",
     author_email="israelilior@gmail.com",
     description="Interactive spectrum plot. Update FFT plot on every new sampled data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lisrael1/spectrum_plot",
     project_urls={
```

### Comparing `spectrum_plot-0.1.0/src/spectrum_plot/plotting.py` & `spectrum_plot-0.2.0/src/spectrum_plot/plotting.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,20 +23,21 @@
         self.fft = pd.Series
         self.raw_data = list()
         self.save_path = save_path
         self.nyquist = None
         self.seconds = None
         self.n = None
         self.image_index = 0
-        self.max_xy_value = [0, 0]
+        self.max_fft_xy_value = [0, 0]
+        self.max_raw_xy_value = [0, 0]
 
         self.add_musical_notes = add_musical_notes
 
         self.no_axis = False
-        fig, self.ax = plt.subplots(1, 1, figsize=figsize)
+        fig, [self.ax_raw, self.ax_fft] = plt.subplots(2, 1, figsize=figsize)
         plt.ion()
         plt.show()
 
     def update_raw_data(self, raw_data, seconds):
         self.raw_data = raw_data
         self.n = len(raw_data)
         self.seconds = seconds
@@ -49,42 +50,60 @@
         self._update_image()
 
     def _update_image(self):
         self._clear_image()
         if self.add_musical_notes:
             self._add_notes()
         self._plot_fft()
-
-    def _clear_image(self):
-        self.ax.clear()
-        self.ax.grid(True)
-        self.ax.set_xlabel('Freq Hz')
-        self.ax.set_ylabel('Sine Amplitude')
-        if self.no_axis:
-            self.ax.set(xticks=[], yticks=[])
-            self.ax.axis('off')
-
-    def _plot_fft(self):
-        if self.fft.index[-1] > self.max_xy_value[0]:
-            self.max_xy_value[0] = self.fft.index[-1]
-        if self.fft.values.max() > self.max_xy_value[1]:
-            self.max_xy_value[1] = self.fft.values.max()
-        self.ax.set_xlim(0, self.max_xy_value[0])
-        self.ax.set_ylim(0, self.max_xy_value[1])
-        self.ax.plot(self.fft.index, self.fft.values)
+        self._plot_raw()
         plt.draw()
         plt.pause(0.001)
         if self.save_path is not None:
             plt.savefig(f'{self.save_path}/fft_{self.image_index:0>5}.jpg')
             self.image_index += 1
 
+    def _clear_image(self):
+        self.ax_fft.clear()
+        self.ax_fft.grid(True)
+        self.ax_fft.set_xlabel('Freq Hz')
+        self.ax_fft.set_ylabel('Sine Amplitude')
+        if self.no_axis:
+            self.ax_fft.set(xticks=[], yticks=[])
+            self.ax_fft.axis('off')
+
+        self.ax_raw.clear()
+        self.ax_raw.grid(True)
+        self.ax_raw.set_xlabel('time seconds')
+        self.ax_raw.set_ylabel('value')
+
+    def _plot_raw(self):
+        if self.seconds > self.max_raw_xy_value[0]:
+            self.max_raw_xy_value[0] = self.seconds
+        if max(self.raw_data) > self.max_raw_xy_value[1]:
+            self.max_raw_xy_value[1] = max(self.raw_data)
+        self.ax_raw.set_xlim(0, self.max_raw_xy_value[0])
+        self.ax_raw.set_ylim(-self.max_raw_xy_value[1], self.max_raw_xy_value[1])
+        self.ax_raw.plot(np.linspace(0, self.seconds, self.n), self.raw_data)
+
+
+    def _plot_fft(self):
+        if self.fft.index[-1] > self.max_fft_xy_value[0]:
+            self.max_fft_xy_value[0] = self.fft.index[-1]
+        if self.fft.values.max() > self.max_fft_xy_value[1]:
+            self.max_fft_xy_value[1] = self.fft.values.max()
+        self.ax_fft.set_xlim(0, self.max_fft_xy_value[0])
+        self.ax_fft.set_ylim(0, self.max_fft_xy_value[1])
+        self.ax_fft.plot(self.fft.index, self.fft.values)
+
+
+
     def _add_notes(self):
         max_note_index = from_freq(self.nyquist)
         if max_note_index.offset_from_note > 0:
             max_note_index = max_note_index.note_index - 1
         else:
             max_note_index = max_note_index.note_index
         for note_index in range(1, max_note_index):
             note = from_note_index(note_index)
-            self.ax.axvline(note.freq, color='red')
-            self.ax.text(note.freq, 0, note.note, color='red', verticalalignment='top')
+            self.ax_fft.axvline(note.freq, color='red')
+            self.ax_fft.text(note.freq, 0, note.note, color='red', verticalalignment='top')
```

### Comparing `spectrum_plot-0.1.0/src/spectrum_plot.egg-info/PKG-INFO` & `spectrum_plot-0.2.0/src/spectrum_plot.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: spectrum-plot
-Version: 0.1.0
-Summary: Interactive spectrum plot. Update FFT plot on every new sampled data
-Home-page: https://github.com/lisrael1/spectrum_plot
-Author: Lior Israeli
-Author-email: israelilior@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/lisrael1/spectrum_plot/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## spectrum plot
-
-### plotting FFT of 1D data, with live plot update
-
-usage example:
-```
-    import numpy as np
-    from spectrum_plot import create_fft_plot
-    
-    
-    plot = create_fft_plot()
-    n = 200
-    seconds = 0.1
-    t = np.linspace(0, seconds, n)
-    nyquist = n / seconds / 2
-    for freq in np.linspace(100, nyquist, 100):
-        sine = np.sin(2 * np.pi * t * freq)
-        plot.update_raw_data(sine, seconds=seconds)
-```
-![](src/spectrum_plot_examples/animated_fft.gif)
-
+Metadata-Version: 2.1
+Name: spectrum-plot
+Version: 0.2.0
+Summary: Interactive spectrum plot. Update FFT plot on every new sampled data
+Home-page: https://github.com/lisrael1/spectrum_plot
+Author: Lior Israeli
+Author-email: israelilior@gmail.com
+Project-URL: Bug Tracker, https://github.com/lisrael1/spectrum_plot/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## spectrum plot
+
+### plotting FFT of 1D data, with live plot update
+
+usage example:
+```python
+import numpy as np
+from spectrum_plot import create_fft_plot
+
+
+plot = create_fft_plot()
+n = 200
+seconds = 0.1
+t = np.linspace(0, seconds, n)
+nyquist = n / seconds / 2
+for freq in np.linspace(100, nyquist, 100):
+    sine = np.sin(2 * np.pi * t * freq)
+    plot.update_raw_data(sine, seconds=seconds)
+```
+![](https://github.com/lisrael1/spectrum_plot/blob/main/src/spectrum_plot_examples/animated_fft.gif?raw=True)
+
+In the examples folder, you can locate a code that includes the addition of music notes at the graph.
+![](https://github.com/lisrael1/spectrum_plot/blob/main/src/spectrum_plot_examples/spectrom_with_notes.png?raw=True)
```

