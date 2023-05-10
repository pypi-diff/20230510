# Comparing `tmp/obob_mne-0.0.18.tar.gz` & `tmp/obob_mne-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obob_mne-0.0.18.tar", last modified: Tue Sep 13 08:43:29 2022, max compression
+gzip compressed data, was "obob_mne-0.0.19.tar", last modified: Wed May 10 09:08:52 2023, max compression
```

## Comparing `obob_mne-0.0.18.tar` & `obob_mne-0.0.19.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.759042 obob_mne-0.0.18/
--rw-r--r--   0 th        (1011) th        (1011)    35097 2022-06-23 07:45:12.000000 obob_mne-0.0.18/LICENSE
--rw-r--r--   0 th        (1011) th        (1011)       49 2022-06-23 07:45:12.000000 obob_mne-0.0.18/MANIFEST.in
--rw-r--r--   0 th        (1011) th        (1011)      321 2022-09-13 08:43:29.759042 obob_mne-0.0.18/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)       81 2022-06-23 07:45:12.000000 obob_mne-0.0.18/README.md
--rw-r--r--   0 th        (1011) th        (1011)        6 2022-09-13 08:43:18.000000 obob_mne-0.0.18/VERSION
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.752042 obob_mne-0.0.18/obob_mne/
--rw-r--r--   0 th        (1011) th        (1011)      870 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/__init__.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.756042 obob_mne-0.0.18/obob_mne/decoding/
--rw-r--r--   0 th        (1011) th        (1011)     1048 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/decoding/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)    22937 2022-09-13 08:42:54.000000 obob_mne-0.0.18/obob_mne/decoding/gentemporal.py
--rw-r--r--   0 th        (1011) th        (1011)     1180 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/decoding/helpers.py
--rw-r--r--   0 th        (1011) th        (1011)     9036 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/decoding/temporal.py
--rw-r--r--   0 th        (1011) th        (1011)     4065 2022-06-23 08:42:16.000000 obob_mne-0.0.18/obob_mne/epochs.py
--rw-r--r--   0 th        (1011) th        (1011)     2367 2022-06-23 08:42:16.000000 obob_mne-0.0.18/obob_mne/events.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.757042 obob_mne-0.0.18/obob_mne/mixins/
--rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/mixins/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)    13373 2022-06-23 08:42:16.000000 obob_mne-0.0.18/obob_mne/mixins/raw.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.757042 obob_mne-0.0.18/obob_mne/mri/
--rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/mri/__init__.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.758042 obob_mne-0.0.18/obob_mne/mri/cmd/
--rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/mri/cmd/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)     1444 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/mri/cmd/import_subject.py
--rw-r--r--   0 th        (1011) th        (1011)     3516 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/mri/cmd/make_freesurfer_bem.py
--rw-r--r--   0 th        (1011) th        (1011)     2960 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/mri/cmd/make_source_space.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.759042 obob_mne-0.0.18/obob_mne/mri/cmd/utils/
--rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/mri/cmd/utils/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)     1632 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/mri/cmd/utils/jobs.py
--rw-r--r--   0 th        (1011) th        (1011)      958 2022-06-23 07:45:12.000000 obob_mne-0.0.18/obob_mne/raw.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.754042 obob_mne-0.0.18/obob_mne.egg-info/
--rw-r--r--   0 th        (1011) th        (1011)      321 2022-09-13 08:43:29.000000 obob_mne-0.0.18/obob_mne.egg-info/PKG-INFO
--rw-r--r--   0 th        (1011) th        (1011)      771 2022-09-13 08:43:29.000000 obob_mne-0.0.18/obob_mne.egg-info/SOURCES.txt
--rw-r--r--   0 th        (1011) th        (1011)        1 2022-09-13 08:43:29.000000 obob_mne-0.0.18/obob_mne.egg-info/dependency_links.txt
--rw-r--r--   0 th        (1011) th        (1011)      278 2022-09-13 08:43:29.000000 obob_mne-0.0.18/obob_mne.egg-info/entry_points.txt
--rw-r--r--   0 th        (1011) th        (1011)       35 2022-09-13 08:43:29.000000 obob_mne-0.0.18/obob_mne.egg-info/requires.txt
--rw-r--r--   0 th        (1011) th        (1011)       15 2022-09-13 08:43:29.000000 obob_mne-0.0.18/obob_mne.egg-info/top_level.txt
--rw-r--r--   0 th        (1011) th        (1011)      444 2022-09-13 08:43:29.760042 obob_mne-0.0.18/setup.cfg
--rw-r--r--   0 th        (1011) th        (1011)     2138 2022-06-23 08:42:16.000000 obob_mne-0.0.18/setup.py
-drwxr-xr-x   0 th        (1011) th        (1011)        0 2022-09-13 08:43:29.759042 obob_mne-0.0.18/tests/
--rw-r--r--   0 th        (1011) th        (1011)      809 2022-06-23 07:45:12.000000 obob_mne-0.0.18/tests/__init__.py
--rw-r--r--   0 th        (1011) th        (1011)      844 2022-06-23 07:45:12.000000 obob_mne-0.0.18/tests/test_example.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.567787 obob_mne-0.0.19/
+-rw-r--r--   0 th        (1011) th        (1011)    35097 2022-06-23 07:45:12.000000 obob_mne-0.0.19/LICENSE
+-rw-r--r--   0 th        (1011) th        (1011)       49 2022-06-23 07:45:12.000000 obob_mne-0.0.19/MANIFEST.in
+-rw-r--r--   0 th        (1011) th        (1011)      302 2023-05-10 09:08:52.567787 obob_mne-0.0.19/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)       81 2022-06-23 07:45:12.000000 obob_mne-0.0.19/README.md
+-rw-r--r--   0 th        (1011) th        (1011)        6 2023-05-10 09:08:40.000000 obob_mne-0.0.19/VERSION
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.562787 obob_mne-0.0.19/obob_mne/
+-rw-r--r--   0 th        (1011) th        (1011)      870 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/__init__.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.564787 obob_mne-0.0.19/obob_mne/decoding/
+-rw-r--r--   0 th        (1011) th        (1011)     1048 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/decoding/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)    25352 2023-05-10 09:08:26.000000 obob_mne-0.0.19/obob_mne/decoding/gentemporal.py
+-rw-r--r--   0 th        (1011) th        (1011)     1180 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/decoding/helpers.py
+-rw-r--r--   0 th        (1011) th        (1011)     9036 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/decoding/temporal.py
+-rw-r--r--   0 th        (1011) th        (1011)     4065 2022-06-23 08:42:16.000000 obob_mne-0.0.19/obob_mne/epochs.py
+-rw-r--r--   0 th        (1011) th        (1011)     2367 2022-06-23 08:42:16.000000 obob_mne-0.0.19/obob_mne/events.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.564787 obob_mne-0.0.19/obob_mne/mixins/
+-rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/mixins/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)    13373 2022-06-23 08:42:16.000000 obob_mne-0.0.19/obob_mne/mixins/raw.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.565787 obob_mne-0.0.19/obob_mne/mri/
+-rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/mri/__init__.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.566787 obob_mne-0.0.19/obob_mne/mri/cmd/
+-rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/mri/cmd/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)     1444 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/mri/cmd/import_subject.py
+-rw-r--r--   0 th        (1011) th        (1011)     3516 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/mri/cmd/make_freesurfer_bem.py
+-rw-r--r--   0 th        (1011) th        (1011)     2960 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/mri/cmd/make_source_space.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.567787 obob_mne-0.0.19/obob_mne/mri/cmd/utils/
+-rw-r--r--   0 th        (1011) th        (1011)      807 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/mri/cmd/utils/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)     1632 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/mri/cmd/utils/jobs.py
+-rw-r--r--   0 th        (1011) th        (1011)      958 2022-06-23 07:45:12.000000 obob_mne-0.0.19/obob_mne/raw.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.563787 obob_mne-0.0.19/obob_mne.egg-info/
+-rw-r--r--   0 th        (1011) th        (1011)      302 2023-05-10 09:08:52.000000 obob_mne-0.0.19/obob_mne.egg-info/PKG-INFO
+-rw-r--r--   0 th        (1011) th        (1011)      771 2023-05-10 09:08:52.000000 obob_mne-0.0.19/obob_mne.egg-info/SOURCES.txt
+-rw-r--r--   0 th        (1011) th        (1011)        1 2023-05-10 09:08:52.000000 obob_mne-0.0.19/obob_mne.egg-info/dependency_links.txt
+-rw-r--r--   0 th        (1011) th        (1011)      278 2023-05-10 09:08:52.000000 obob_mne-0.0.19/obob_mne.egg-info/entry_points.txt
+-rw-r--r--   0 th        (1011) th        (1011)       35 2023-05-10 09:08:52.000000 obob_mne-0.0.19/obob_mne.egg-info/requires.txt
+-rw-r--r--   0 th        (1011) th        (1011)       15 2023-05-10 09:08:52.000000 obob_mne-0.0.19/obob_mne.egg-info/top_level.txt
+-rw-r--r--   0 th        (1011) th        (1011)      444 2023-05-10 09:08:52.571787 obob_mne-0.0.19/setup.cfg
+-rw-r--r--   0 th        (1011) th        (1011)     2138 2022-06-23 08:42:16.000000 obob_mne-0.0.19/setup.py
+drwxr-xr-x   0 th        (1011) th        (1011)        0 2023-05-10 09:08:52.567787 obob_mne-0.0.19/tests/
+-rw-r--r--   0 th        (1011) th        (1011)      809 2022-06-23 07:45:12.000000 obob_mne-0.0.19/tests/__init__.py
+-rw-r--r--   0 th        (1011) th        (1011)      844 2022-06-23 07:45:12.000000 obob_mne-0.0.19/tests/test_example.py
```

### Comparing `obob_mne-0.0.18/LICENSE` & `obob_mne-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/__init__.py` & `obob_mne-0.0.19/obob_mne/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/decoding/__init__.py` & `obob_mne-0.0.19/obob_mne/decoding/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/decoding/gentemporal.py` & `obob_mne-0.0.19/obob_mne/decoding/gentemporal.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,14 +128,17 @@
     @property
     def chance_level(self):
         """float: The chance level of the classifier."""
         return 1.0 / self._nclasses
 
     def diagonal_as_temporal(self):
         """Return the non-generalized results."""
+        if len(self._times_training) != len(self._times_testing):
+            raise RuntimeError('Cannot show diagonal for non uniform '
+                               'dimensions!')
         if self._scores_raw.ndim == 2:
             raw_scores = numpy.diagonal(self._scores_raw)
         else:
             raw_scores = numpy.diagonal(self._scores_raw, axis1=1, axis2=2)
 
         return TemporalArray(raw_scores=raw_scores,
                              weights=self.weights,
@@ -183,27 +186,28 @@
                              nave_testing=self.nave_testing,
                              c_factors_training=self._c_factors_training,
                              c_factors_testing=self._c_factors_testing
                              )
 
     def _plot_image(self, values, axes=None, show=True, cmap='Reds',
                     colorbar=True,
-                    interpolation='bessel'):
+                    interpolation='bessel', alpha=None):
         import matplotlib.pyplot as plt
 
         if not isinstance(axes, plt.Axes):
             fig, axes = plt.subplots(1, 1)
         else:
             fig = axes.get_figure()
 
         im = axes.imshow(values, interpolation=interpolation, origin='lower',
                          cmap=cmap,
-                         extent=numpy.append(self._times_training[[0, -1]],
-                                             self._times_testing[[0, -1]]),
-                         aspect='auto')
+                         extent=numpy.append(self._times_testing[[0, -1]],
+                                             self._times_training[[0, -1]]),
+                         aspect='auto',
+                         alpha=alpha)
 
         xlabel = 'Testing time (s)'
         ylabel = 'Training time (s)'
 
         if self._c_factors_testing:
             xlabel = '\n'.join([self._c_factors_testing, xlabel])
 
@@ -213,27 +217,29 @@
         axes.set_xlabel(xlabel)
         axes.set_ylabel(ylabel)
         axes.set_title('Temporal Generalization')
         axes.axvline(0, color='k')
         axes.axhline(0, color='k')
         old_xlim = axes.get_xlim()
         old_ylim = axes.get_ylim()
-        axes.plot(axes.get_xlim(), axes.get_ylim(), color='k')
+        diag = (min(self._times_testing[0], self._times_training[0]), max(self._times_testing[-1], self._times_training[-1]))
+        axes.plot(diag, diag, color='k')
         axes.set_xlim(old_xlim)
         axes.set_ylim(old_ylim)
         if colorbar:
             plt.colorbar(im, ax=axes)
 
         if show:
             plt.show()
 
         return fig
 
     def plot_scores(self, axes=None, show=True, cmap='Reds', colorbar=True,
-                    mask_below_chance=False, interpolation='bessel'):
+                    mask_below_chance=False, interpolation='bessel',
+                    insignificant_alpha=0.3):
         """Plot the scores as a Matrix.
 
         Parameters
         ----------
         axes : :class:`matplotlib.axes.Axes` or None, optional
             The axes where to draw the plot. If ``None``, a new figure is
             created.
@@ -246,19 +252,23 @@
         mask_below_chance : bool, optional
             If True, values below chance level get masked.
         interpolation : str, optional
             The interpolation method used.
         """
         scores = self.scores
 
+        alpha = numpy.ones_like(scores)
+        
         if mask_below_chance:
-            scores = numpy.ma.masked_less(scores, self.chance_level)
+            mask = scores < self.chance_level
+            alpha[mask] = insignificant_alpha
 
         return self._plot_image(values=scores, axes=axes, show=show, cmap=cmap,
-                                colorbar=colorbar, interpolation=interpolation)
+                                colorbar=colorbar, interpolation=interpolation,
+                                alpha=alpha)
 
     def drop_channels(self, chs):
         """Drop the channels from the weights.
 
         Parameters
         ----------
         chs : list of str
@@ -267,14 +277,59 @@
         good_channels_idx = mne.pick_channels(self.info['ch_names'],
                                               include=[],
                                               exclude=chs)
 
         self._info = mne.pick_info(self.info, good_channels_idx)
         self._weights = self._weights[good_channels_idx, :]
 
+    def crop(self, tmin_training=None, tmax_training=None,
+             tmin_testing=None, tmax_testing=None):
+        """Crop to times
+        
+        """
+        if tmin_training is None:
+            tmin_training = self._times_training[0]
+        if tmax_training is None:
+            tmax_training = self._times_training[-1]
+
+        if tmin_testing is None:
+            tmin_testing = self._times_testing[0]
+        if tmax_testing is None:
+            tmax_testing = self._times_testing[-1]
+
+        
+        time_idx_training = numpy.where(
+            numpy.logical_and(
+                self._times_training >= tmin_training,
+                self._times_training <= tmax_training))[0]
+        
+        time_idx_testing = numpy.where(
+            numpy.logical_and(
+                self._times_testing >= tmin_testing,
+                self._times_testing <= tmax_testing))[0]
+        
+        
+        if self._scores_raw.ndim == 2:
+            self._scores_raw = self._scores_raw[time_idx_training, :]
+            self._scores_raw = self._scores_raw[:, time_idx_testing]
+            if self._weights is not None:
+                self._weights = self._weights[time_idx_training, :]
+                self._weights = self._weights[:, time_idx_testing]
+        else:
+            self._scores_raw = self._scores_raw[:, time_idx_training, :]
+            self._scores_raw = self._scores_raw[:, :, time_idx_testing]
+            if self._weights is not None:
+                self._weights = self._weights[:, time_idx_training, :]
+                self._weights = self._weights[:, :, time_idx_testing]
+
+        self._times_testing = self._times_testing[time_idx_testing]
+        self._times_training = self._times_training[time_idx_training]
+
+        return self
+
 
 class GeneralizedTemporalFromCollection(GeneralizedTemporalArray):
     """Base class for Temporal Generalization data from multiple subjects.
 
     The individual elements must match in number of classes, times etc.
 
     Parameters
@@ -397,15 +452,15 @@
 
         self.stat_values, self.p = stat_function(scores_for_stats,
                                                  popmean=popmean, **kwargs)
         self.p = self.p / 2.0
 
     def plot_scores(self, axes=None, show=True, cmap='Reds', colorbar=True,
                     mask_below_chance=False, interpolation='bessel',
-                    mask_p=None):
+                    mask_p=None, insignificant_alpha=0.3):
         """Plot the scores as a Matrix.
 
         Parameters
         ----------
         axes : :class:`matplotlib.axes.Axes` or None, optional
             The axes where to draw the plot. If ``None``, a new figure is
             created.
@@ -420,22 +475,27 @@
         interpolation : str, optional
             The interpolation method used.
         mask_p : float or None, optional
             If set, the plot is masked for the given p-value.
         """
         scores = self.scores
 
+        alpha = numpy.ones_like(scores)
+        
         if mask_below_chance:
-            scores = numpy.ma.masked_less(scores, self.chance_level)
+            mask = scores < self.chance_level
+            alpha[mask] = insignificant_alpha
 
         if mask_p is not None:
-            scores = numpy.ma.masked_where(self.p > mask_p, scores)
+            mask = self.p > mask_p
+            alpha[mask] = insignificant_alpha
 
         return self._plot_image(values=scores, axes=axes, show=show, cmap=cmap,
-                                colorbar=colorbar, interpolation=interpolation)
+                                colorbar=colorbar, interpolation=interpolation,
+                                alpha=alpha)
 
     def get_temporal_from_training_interval(self, tmin, tmax):
         """Average the scores of a training interval.
 
         Parameters
         ----------
         tmin : int
```

### Comparing `obob_mne-0.0.18/obob_mne/decoding/helpers.py` & `obob_mne-0.0.19/obob_mne/decoding/helpers.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/decoding/temporal.py` & `obob_mne-0.0.19/obob_mne/decoding/temporal.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/epochs.py` & `obob_mne-0.0.19/obob_mne/epochs.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/events.py` & `obob_mne-0.0.19/obob_mne/events.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mixins/__init__.py` & `obob_mne-0.0.19/obob_mne/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mixins/raw.py` & `obob_mne-0.0.19/obob_mne/mixins/raw.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mri/__init__.py` & `obob_mne-0.0.19/obob_mne/mri/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mri/cmd/__init__.py` & `obob_mne-0.0.19/obob_mne/mri/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mri/cmd/import_subject.py` & `obob_mne-0.0.19/obob_mne/mri/cmd/import_subject.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mri/cmd/make_freesurfer_bem.py` & `obob_mne-0.0.19/obob_mne/mri/cmd/make_freesurfer_bem.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mri/cmd/make_source_space.py` & `obob_mne-0.0.19/obob_mne/mri/cmd/make_source_space.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mri/cmd/utils/__init__.py` & `obob_mne-0.0.19/obob_mne/mri/cmd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/mri/cmd/utils/jobs.py` & `obob_mne-0.0.19/obob_mne/mri/cmd/utils/jobs.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne/raw.py` & `obob_mne-0.0.19/obob_mne/raw.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/obob_mne.egg-info/SOURCES.txt` & `obob_mne-0.0.19/obob_mne.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/setup.py` & `obob_mne-0.0.19/setup.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/tests/__init__.py` & `obob_mne-0.0.19/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `obob_mne-0.0.18/tests/test_example.py` & `obob_mne-0.0.19/tests/test_example.py`

 * *Files identical despite different names*

