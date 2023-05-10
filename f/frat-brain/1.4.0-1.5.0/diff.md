# Comparing `tmp/frat_brain-1.4.0.tar.gz` & `tmp/frat_brain-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frat_brain-1.4.0.tar", max compression
+gzip compressed data, was "frat_brain-1.5.0.tar", max compression
```

## Comparing `frat_brain-1.4.0.tar` & `frat_brain-1.5.0.tar`

### file list

```diff
@@ -1,42 +1,54 @@
--rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.4.0/LICENSE
--rw-r--r--   0        0        0     3046 2023-04-05 12:46:27.664420 frat_brain-1.4.0/README.md
--rw-r--r--   0        0        0    53941 2023-04-24 16:58:06.275544 frat_brain-1.4.0/fRAT/__main__.py
--rw-r--r--   0        0        0       22 2023-04-26 15:19:49.684640 frat_brain-1.4.0/fRAT/_version.py
--rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.4.0/fRAT/configuration_profiles/latest_settings.toml
--rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.050383 frat_brain-1.4.0/fRAT/configuration_profiles/maps/default_config.toml
--rw-r--r--   0        0        0     4291 2023-04-24 16:58:42.676825 frat_brain-1.4.0/fRAT/configuration_profiles/maps/statmap_config.toml
--rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.060703 frat_brain-1.4.0/fRAT/configuration_profiles/maps/test_config.toml
--rw-r--r--   0        0        0    17981 2023-03-30 13:46:50.969594 frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/default_config.toml
--rw-r--r--   0        0        0    17981 2023-04-24 16:59:58.274205 frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
--rw-r--r--   0        0        0    17395 2023-03-30 13:46:51.070056 frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/test_config.toml
--rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.4.0/fRAT/images/fRAT.gif
--rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.4.0/fRAT/nogui.py
--rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.4.0/fRAT/utils/__init__.py
--rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.4.0/fRAT/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.4.0/fRAT/utils/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.4.0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.4.0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
--rw-r--r--   0        0        0    17636 2023-04-05 12:13:52.837379 frat_brain-1.4.0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.4.0/fRAT/utils/__pycache__/figures.cpython-310.pyc
--rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.4.0/fRAT/utils/__pycache__/html_report.cpython-310.pyc
--rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.4.0/fRAT/utils/__pycache__/printResults.cpython-310.pyc
--rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.4.0/fRAT/utils/__pycache__/statistics.cpython-310.pyc
--rw-r--r--   0        0        0    11331 2023-03-14 17:05:50.271422 frat_brain-1.4.0/fRAT/utils/__pycache__/statmap.cpython-310.pyc
--rw-r--r--   0        0        0     5375 2023-03-06 14:02:43.929731 frat_brain-1.4.0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    14975 2023-04-20 11:52:26.913182 frat_brain-1.4.0/fRAT/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.4.0/fRAT/utils/analysis.py
--rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.4.0/fRAT/utils/bootstrap.css
--rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.4.0/fRAT/utils/dash_report.py
--rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.4.0/fRAT/utils/directory_comparison.py
--rw-r--r--   0        0        0    34582 2023-04-03 14:11:00.889152 frat_brain-1.4.0/fRAT/utils/fRAT_config_setup.py
--rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.4.0/fRAT/utils/figures.py
--rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.4.0/fRAT/utils/html_report.py
--rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.4.0/fRAT/utils/printResults.py
--rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.4.0/fRAT/utils/script.js
--rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.4.0/fRAT/utils/statistics.py
--rw-r--r--   0        0        0    16388 2023-03-14 17:05:44.468988 frat_brain-1.4.0/fRAT/utils/statmap.py
--rw-r--r--   0        0        0     8967 2023-01-31 14:53:42.200233 frat_brain-1.4.0/fRAT/utils/statmap_config_setup.py
--rw-r--r--   0        0        0    18883 2023-04-20 10:26:54.263057 frat_brain-1.4.0/fRAT/utils/utils.py
--rw-r--r--   0        0        0     2390 2023-04-26 15:20:04.978955 frat_brain-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 frat_brain-1.4.0/setup.py
--rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 frat_brain-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3046 2023-04-05 12:46:27.664420 frat_brain-1.5.0/README.md
+-rw-r--r--   0        0        0     8196 2023-05-04 14:03:22.213584 frat_brain-1.5.0/fRAT/.DS_Store
+-rw-r--r--   0        0        0      228 2023-05-10 16:07:10.854878 frat_brain-1.5.0/fRAT/HOUSE/__init__.py
+-rw-r--r--   0        0        0      539 2023-05-05 16:06:02.329184 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     6154 2023-05-10 13:02:37.995811 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/add_motion.cpython-310.pyc
+-rw-r--r--   0        0        0     1732 2023-05-09 12:00:42.782332 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/add_noise.cpython-310.pyc
+-rw-r--r--   0        0        0     3402 2023-05-10 13:15:37.908106 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/handler.cpython-310.pyc
+-rw-r--r--   0        0        0     2339 2023-05-10 14:23:49.376966 frat_brain-1.5.0/fRAT/HOUSE/__pycache__/separate_noise_volumes.cpython-310.pyc
+-rw-r--r--   0        0        0     6580 2023-05-10 16:07:10.855691 frat_brain-1.5.0/fRAT/HOUSE/add_motion.py
+-rw-r--r--   0        0        0     1836 2023-05-10 16:07:10.856488 frat_brain-1.5.0/fRAT/HOUSE/add_noise.py
+-rw-r--r--   0        0        0     4510 2023-05-10 16:07:10.857305 frat_brain-1.5.0/fRAT/HOUSE/handler.py
+-rw-r--r--   0        0        0     2047 2023-05-10 16:07:10.858140 frat_brain-1.5.0/fRAT/HOUSE/separate_noise_volumes.py
+-rw-r--r--   0        0        0    53981 2023-05-10 16:07:10.859431 frat_brain-1.5.0/fRAT/__main__.py
+-rw-r--r--   0        0        0       22 2023-05-10 16:14:39.878750 frat_brain-1.5.0/fRAT/_version.py
+-rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.5.0/fRAT/configuration_profiles/latest_settings.toml
+-rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.860695 frat_brain-1.5.0/fRAT/configuration_profiles/maps/default_config.toml
+-rw-r--r--   0        0        0     4338 2023-05-10 16:07:10.861735 frat_brain-1.5.0/fRAT/configuration_profiles/maps/statmap_config.toml
+-rw-r--r--   0        0        0     3905 2023-05-10 16:07:10.862965 frat_brain-1.5.0/fRAT/configuration_profiles/maps/test_config.toml
+-rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.864159 frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/default_config.toml
+-rw-r--r--   0        0        0    17991 2023-05-10 16:07:10.865669 frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
+-rw-r--r--   0        0        0    17405 2023-05-10 16:07:10.866968 frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/test_config.toml
+-rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.5.0/fRAT/images/fRAT.gif
+-rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.5.0/fRAT/nogui.py
+-rw-r--r--   0        0        0     6148 2023-05-04 14:03:22.211954 frat_brain-1.5.0/fRAT/utils/.DS_Store
+-rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.5.0/fRAT/utils/__init__.py
+-rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.5.0/fRAT/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.5.0/fRAT/utils/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.5.0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.5.0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
+-rw-r--r--   0        0        0    17651 2023-05-10 14:13:55.023764 frat_brain-1.5.0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    22288 2023-04-24 17:13:29.813025 frat_brain-1.5.0/fRAT/utils/__pycache__/figures.cpython-310.pyc
+-rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.5.0/fRAT/utils/__pycache__/html_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.5.0/fRAT/utils/__pycache__/printResults.cpython-310.pyc
+-rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.5.0/fRAT/utils/__pycache__/statistics.cpython-310.pyc
+-rw-r--r--   0        0        0     9295 2023-05-10 15:56:17.112312 frat_brain-1.5.0/fRAT/utils/__pycache__/statmap.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-05-09 15:27:08.538396 frat_brain-1.5.0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    15234 2023-05-04 16:27:06.681168 frat_brain-1.5.0/fRAT/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.5.0/fRAT/utils/analysis.py
+-rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.5.0/fRAT/utils/bootstrap.css
+-rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.5.0/fRAT/utils/dash_report.py
+-rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.5.0/fRAT/utils/directory_comparison.py
+-rw-r--r--   0        0        0    34597 2023-05-10 16:07:10.868291 frat_brain-1.5.0/fRAT/utils/fRAT_config_setup.py
+-rw-r--r--   0        0        0    36719 2023-04-24 17:04:40.596180 frat_brain-1.5.0/fRAT/utils/figures.py
+-rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.5.0/fRAT/utils/html_report.py
+-rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.5.0/fRAT/utils/printResults.py
+-rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.5.0/fRAT/utils/script.js
+-rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.5.0/fRAT/utils/statistics.py
+-rw-r--r--   0        0        0    13101 2023-05-10 16:07:10.869916 frat_brain-1.5.0/fRAT/utils/statmap.py
+-rw-r--r--   0        0        0     9345 2023-05-10 16:07:10.871233 frat_brain-1.5.0/fRAT/utils/statmap_config_setup.py
+-rw-r--r--   0        0        0    19156 2023-05-10 16:07:10.917697 frat_brain-1.5.0/fRAT/utils/utils.py
+-rw-r--r--   0        0        0     2390 2023-05-10 16:14:56.329049 frat_brain-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5992 1970-01-01 00:00:00.000000 frat_brain-1.5.0/setup.py
+-rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 frat_brain-1.5.0/PKG-INFO
```

### Comparing `frat_brain-1.4.0/LICENSE` & `frat_brain-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/README.md` & `frat_brain-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/__main__.py` & `frat_brain-1.5.0/fRAT/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     def statmap_run_frame_create(self, window):
         self.statmap_run_frame = tk.LabelFrame(window)
         self.frames.append(self.statmap_run_frame)
         self.statmap_run_frame.place(relx=0.5, rely=0, height=140, relwidth=0.467)
         self.statmap_run_frame.configure(text='Run', font=self.heading_font)
         self.format_frame(self.statmap_run_frame, borderwidth=1)
 
-        statmap_options = ('Image SNR', 'Temporal SNR', 'Add Gaussian noise')
+        statmap_options = ('Image SNR', 'Temporal SNR', 'Add Gaussian noise', 'Add motion', 'Separate noise volumes')
         state = tk.StringVar()
         state.set(statmap_options[1])
         self.statmap_option = tk.OptionMenu(self.statmap_run_frame, state, *statmap_options)
         self.statmap_option.place(relx=0.08, rely=0.27, width=200, bordermode='ignore')
         self.statmap_option.configure(bg=self.background)
         self.statmap_option.val = state
```

### Comparing `frat_brain-1.4.0/fRAT/configuration_profiles/maps/default_config.toml` & `frat_brain-1.5.0/fRAT/configuration_profiles/maps/default_config.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,13 +20,12 @@
 spatial_smoothing = false                                                         # true or false. Uses SUSAN to spatial smooth. Recommended: true
 smoothing_fwhm = 8.0                                                              # fwhm of smoothing, in mm, gets converted using sqrt(8*log(2)). Recommended: 8.0
 smoothing_brightness_threshold = 2000.0                                           # Should be greater than noise level and less than contrast of edges to be preserved. Recommended: 2000.0
 
 ## Image SNR calculation
 magnitude_correction = true                                                       # true or false. Correction factor of 0.7 applied when running iSNR calculations, to correct for Rayleigh distributed noise when using magnitude vs complex images.  Reference: Constantinides, C. D., Atalar, E., & McVeigh, E. R. (1997). Signal-to-Noise Measurements in Magnitude Images from NMR Phased Arrays.
 noise_volume = true                                                               # true or false. Select true if a noise volume has been collected as part of the fMRI time series. NOTE: If true, the noise volume in the time series will be separated from the functional volumes and will be placed into the folder "func_noiseVolumeRemoved". If "noise volume" is true and "noise value" is not none, the noise volume will be used in image SNR calculation rather than the user defined noise value.
-noise_volume_location = 'End'                                                     # 'max' to select number of cores available on the system, alternatively an int to manually select number of cores to use. Recommended: 'max' Options: ['Beginning', 'End'].
 iSNR_std_use_only_nonzero_voxels = true                                           # true or false.
 
 ## Add Gaussian noise
 noise_multipliers = [1]                                                           # Provide a comma-separated list of multipliers for the standard deviation of the gaussian noise to plot e.g. '1, 5'. NOTE: a separate file will be produced for each multiplier
```

### Comparing `frat_brain-1.4.0/fRAT/configuration_profiles/maps/statmap_config.toml` & `frat_brain-1.5.0/fRAT/configuration_profiles/maps/statmap_config.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 ## Spatial smoothing
 spatial_smoothing = false                                                         # true or false. Uses SUSAN to spatial smooth. Recommended: true
 smoothing_fwhm = 8.0                                                              # fwhm of smoothing, in mm, gets converted using sqrt(8*log(2)). Recommended: 8.0
 smoothing_brightness_threshold = 2000.0                                           # Should be greater than noise level and less than contrast of edges to be preserved. Recommended: 2000.0
 
 ## Image SNR calculation
 magnitude_correction = true                                                       # true or false. Correction factor of 0.7 applied when running iSNR calculations, to correct for Rayleigh distributed noise when using magnitude vs complex images.  Reference: Constantinides, C. D., Atalar, E., & McVeigh, E. R. (1997). Signal-to-Noise Measurements in Magnitude Images from NMR Phased Arrays.
-noise_volume = false                                                              # true or false. Select true if a noise volume has been collected as part of the fMRI time series. NOTE: If true, the noise volume in the time series will be separated from the functional volumes and will be placed into the folder "func_noiseVolumeRemoved". If "noise volume" is true and "noise value" is not none, the noise volume will be used in image SNR calculation rather than the user defined noise value.
-noise_volume_location = 'End'                                                     # 'max' to select number of cores available on the system, alternatively an int to manually select number of cores to use. Recommended: 'max' Options: ['Beginning', 'End'].
+noise_volume = true                                                               # true or false. Select true if a noise volume has been collected as part of the fMRI time series. NOTE: If true, the noise volume in the time series will be separated from the functional volumes and will be placed into the folder "func_noiseVolumeRemoved". If "noise volume" is true and "noise value" is not none, the noise volume will be used in image SNR calculation rather than the user defined noise value.
 iSNR_std_use_only_nonzero_voxels = true                                           # true or false.
 
 ## Add Gaussian noise
-noise_multipliers = 1                                                             # Provide a comma-separated list of multipliers for the standard deviation of the gaussian noise to plot e.g. '1, 5'. A separate file will be produced for each multiplier. NOTE: Noise has a gaussian distribution, with a mean of 0 and a standard deviation of the noise level of each participant * multiplier.
+noise_multipliers = [1, 2, 5]                                                     # Provide a comma-separated list of multipliers, e.g. '1, 5'. A separate file will be produced for each multiplier. NOTE: Added has a gaussian distribution, with a mean of 0 and a standard deviation of the noise level of each participant * multiplier.
+motion_multipliers = [1, 2, 5]                                                    # Provide a comma-separated list of multipliers, e.g. '1, 5'. A separate file will be produced for each multiplier. NOTE: Added motion has a gaussian distribution, with a mean of 0 and a standard deviation of the average rotation/translation of each participant * multiplier.
```

### Comparing `frat_brain-1.4.0/fRAT/configuration_profiles/maps/test_config.toml` & `frat_brain-1.5.0/fRAT/configuration_profiles/maps/test_config.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,13 +20,12 @@
 spatial_smoothing = false                                                         # true or false. Uses SUSAN to spatial smooth. Recommended: true
 smoothing_fwhm = 8.0                                                              # fwhm of smoothing, in mm, gets converted using sqrt(8*log(2)). Recommended: 8.0
 smoothing_brightness_threshold = 2000.0                                           # Should be greater than noise level and less than contrast of edges to be preserved. Recommended: 2000.0
 
 ## Image SNR calculation
 magnitude_correction = true                                                       # true or false. Correction factor of 0.7 applied when running iSNR calculations, to correct for Rayleigh distributed noise when using magnitude vs complex images.  Reference: Constantinides, C. D., Atalar, E., & McVeigh, E. R. (1997). Signal-to-Noise Measurements in Magnitude Images from NMR Phased Arrays.
 noise_volume = true                                                               # true or false. Select true if a noise volume has been collected as part of the fMRI time series. NOTE: If true, the noise volume in the time series will be separated from the functional volumes and will be placed into the folder "func_noiseVolumeRemoved". If "noise volume" is true and "noise value" is not none, the noise volume will be used in image SNR calculation rather than the user defined noise value.
-noise_volume_location = 'End'                                                     # 'max' to select number of cores available on the system, alternatively an int to manually select number of cores to use. Recommended: 'max' Options: ['Beginning', 'End'].
 iSNR_std_use_only_nonzero_voxels = true                                           # true or false.
 
 ## Add Gaussian noise
 noise_multipliers = [1]                                                           # Provide a comma-separated list of multipliers for the standard deviation of the gaussian noise to plot e.g. '1, 5'. NOTE: a separate file will be produced for each multiplier
```

### Comparing `frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/default_config.toml` & `frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/default_config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Installation testing
 delete_test_folder = 'Always'                                                     # Option to choose whether the folder generated while running tests is deleted upon completion. Options: ['Always', 'If completed without error', 'Never'].
 verbose_errors = false                                                            # true or false. Print all missing files and differences found during testing to the terminal.
 
 # Analysis
 atlas_number = 'HarvardOxford-cort'                                               #  Options: ['Cerebellum-MNIflirt', 'Cerebellum-MNIfnirt', 'HarvardOxford-cort', 'HarvardOxford-sub', 'JHU-ICBM-labels', 'JHU-ICBM-tracts', 'juelich', 'MNI', 'SMATT-labels', 'STN', 'striatum-structural', 'Talairach-labels', 'Thalamus'].
-input_folder_name = 'func_cleaned'                                                # Folder found in each subjects directory containing the files to be analysed. func_cleaned is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
+input_folder_name = 'func_preprocessed'                                                # Folder found in each subjects directory containing the files to be analysed. func_preprocessed is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
 output_folder = 'DEFAULT'                                                         # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
 dof = 12                                                                          # Degrees of freedom for FLIRT (only used for the fMRI to anatomical alignment when using Correlation Ratio cost function). Recommended: 12
 anat_align_cost_function = 'BBR'                                                  # BBR or Correlation Ratio. Recommended: BBR. Using BBR (Boundary-Based Registration) requires an FSL FAST segmentation (this will be automatically created if necessary if the Run FSL FAST option is set to "Run if files not found") and a wholehead non-brain extracted anatomical placed in the anat folder. Options: ['BBR', 'Correlation Ratio'].
 grey_matter_segment = true                                                        # true or false. Recommended: true if using a cortical atlas. Note: FSL FAST segmentation files should be placed in the sub-{id}/fslfast/ directory. Only the FSL FAST file appended with pve_1 needs to be in this directory, however if all files output by FAST are placed in this directory, then fRAT will find the necessary file.
 run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found".  These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
 fslfast_min_prob = 0.1                                                            # Recommended: 0.1
 stat_map_folder = ''                                                              # Folder name which contains the statistical map files. Example: temporalSNR_report
```

### Comparing `frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml` & `frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Installation testing
 delete_test_folder = 'If completed without error'                                 # Option to choose whether the folder generated while running tests is deleted upon completion. This only applies when running the full comparison. Options: ['Always', 'If completed without error', 'Never'].
 verbose_errors = true                                                             # true or false. Print all missing files and differences found during testing to the terminal.
 
 # Analysis
 atlas_number = 'HarvardOxford-cort'                                               #  Options: ['Cerebellum-MNIflirt', 'Cerebellum-MNIfnirt', 'HarvardOxford-cort', 'HarvardOxford-sub', 'JHU-ICBM-labels', 'JHU-ICBM-tracts', 'juelich', 'MNI', 'SMATT-labels', 'STN', 'striatum-structural', 'Talairach-labels', 'Thalamus'].
-input_folder_name = 'func_cleaned'                                                # Folder found in each subjects directory containing the files to be analysed. func_cleaned is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
+input_folder_name = 'func_preprocessed'                                                # Folder found in each subjects directory containing the files to be analysed. func_preprocessed is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
 output_folder = 'DEFAULT'                                                         # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
 dof = 12                                                                          # Degrees of freedom for FLIRT (only used for the fMRI to anatomical alignment when using Correlation Ratio cost function). Recommended: 12
 anat_align_cost_function = 'BBR'                                                  # BBR or Correlation Ratio. Recommended: BBR. Using BBR (Boundary-Based Registration) requires an FSL FAST segmentation (this will be automatically created if necessary if the Run FSL FAST option is set to "Run if files not found") and a wholehead non-brain extracted anatomical placed in the anat folder. Options: ['BBR', 'Correlation Ratio'].
 grey_matter_segment = true                                                        # true or false. Recommended: true if using a cortical atlas. Note: FSL FAST segmentation files should be placed in the sub-{id}/fslfast/ directory. Only the FSL FAST file appended with pve_1 needs to be in this directory, however if all files output by FAST are placed in this directory, then fRAT will find the necessary file.
 run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found". These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
 fslfast_min_prob = 0.1                                                            # Recommended: 0.1
 stat_map_folder = ''                                                              # Folder name which contains the statistical map files. Example: temporalSNR_report
```

### Comparing `frat_brain-1.4.0/fRAT/configuration_profiles/roi_analysis/test_config.toml` & `frat_brain-1.5.0/fRAT/configuration_profiles/roi_analysis/test_config.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Installation testing
 delete_test_folder = 'Always'                                                     # Option to choose whether the folder generated while running tests is deleted upon completion. Options: ['Always', 'If completed without error', 'Never'].
 verbose_errors = false                                                            # true or false. Print all missing files and differences found during testing to the terminal.
 
 # Analysis
 atlas_number = 'HarvardOxford-cort'                                               #  Options: ['Cerebellum-MNIflirt', 'Cerebellum-MNIfnirt', 'HarvardOxford-cort', 'HarvardOxford-sub', 'JHU-ICBM-labels', 'JHU-ICBM-tracts', 'juelich', 'MNI', 'SMATT-labels', 'STN', 'striatum-structural', 'Talairach-labels', 'Thalamus'].
-input_folder_name = 'func_cleaned'                                                # Folder found in each subjects directory containing the files to be analysed. func_cleaned is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
+input_folder_name = 'func_preprocessed'                                                # Folder found in each subjects directory containing the files to be analysed. func_preprocessed is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
 output_folder = 'DEFAULT'                                                         # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
 dof = 12                                                                          # Degrees of freedom for FLIRT (only used for the fMRI to anatomical alignment when using Correlation Ratio cost function). Recommended: 12
 anat_align_cost_function = 'BBR'                                                  # BBR or Correlation Ratio. Recommended: BBR. Using BBR (Boundary-Based Registration) requires an FSL FAST segmentation (this will be automatically created if necessary if the Run FSL FAST option is set to "Run if files not found") and a wholehead non-brain extracted anatomical placed in the anat folder. Options: ['BBR', 'Correlation Ratio'].
 grey_matter_segment = true                                                        # true or false. Recommended: true if using a cortical atlas. Note: FSL FAST segmentation files should be placed in the sub-{id}/fslfast/ directory. Only the FSL FAST file appended with pve_1 needs to be in this directory, however if all files output by FAST are placed in this directory, then fRAT will find the necessary file.
 run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found".  These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
 fslfast_min_prob = 0.1                                                            # Recommended: 0.1
 stat_map_folder = ''                                                              # Folder name which contains the statistical map files. Example: temporalSNR_report
```

### Comparing `frat_brain-1.4.0/fRAT/images/fRAT.gif` & `frat_brain-1.5.0/fRAT/images/fRAT.gif`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/nogui.py` & `frat_brain-1.5.0/fRAT/nogui.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/analysis.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/analysis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/dash_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr  3 14:11:00 2023 UTC, .py size: 34582 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 74de 2a64 1687 0000  o.......t.*d....
+00000000: 6f0d 0d0a 0000 0000 a0a6 5b64 2587 0000  o.........[d%...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0014 0000 0040 0000 0073 8e07 0000 6400  .....@...s....d.
 00000030: 5a00 6700 6401 a201 5a01 0900 6900 6402  Z.g.d...Z...i.d.
 00000040: 6403 6404 6405 6406 6407 6408 9c05 9301  d.d.d.d.d.d.....
 00000050: 6409 6403 6404 6405 640a 640b 6408 9c05  d.d.d.d.d.d.d...
 00000060: 9301 640c 6403 6404 6405 640a 640d 6408  ..d.d.d.d.d.d.d.
 00000070: 9c05 9301 640e 6403 6404 640a 640f 6410  ....d.d.d.d.d.d.
@@ -302,802 +302,803 @@
 000012d0: 497a 0c53 4d41 5454 2d6c 6162 656c 73da  Iz.SMATT-labels.
 000012e0: 0353 544e 7a13 7374 7269 6174 756d 2d73  .STNz.striatum-s
 000012f0: 7472 7563 7475 7261 6c7a 1054 616c 6169  tructuralz.Talai
 00001300: 7261 6368 2d6c 6162 656c 73da 0854 6861  rach-labels..Tha
 00001310: 6c61 6d75 7329 0672 0b00 0000 720c 0000  lamus).r....r...
 00001320: 0072 2100 0000 720f 0000 0072 2000 0000  .r!...r....r ...
 00001330: 720e 0000 00da 1169 6e70 7574 5f66 6f6c  r......input_fol
-00001340: 6465 725f 6e61 6d65 5a0c 6675 6e63 5f63  der_nameZ.func_c
-00001350: 6c65 616e 6564 6125 0200 0046 6f6c 6465  leaneda%...Folde
-00001360: 7220 666f 756e 6420 696e 2065 6163 6820  r found in each 
-00001370: 7375 626a 6563 7473 2064 6972 6563 746f  subjects directo
-00001380: 7279 2063 6f6e 7461 696e 696e 6720 7468  ry containing th
-00001390: 6520 6669 6c65 7320 746f 2062 6520 616e  e files to be an
-000013a0: 616c 7973 6564 2e20 6675 6e63 5f63 6c65  alysed. func_cle
-000013b0: 616e 6564 2069 7320 7468 6520 6465 6661  aned is the defa
-000013c0: 756c 7420 6f70 7469 6f6e 2061 7320 7468  ult option as th
-000013d0: 6973 2066 6f6c 6465 7220 7769 6c6c 2061  is folder will a
-000013e0: 7574 6f6d 6174 6963 616c 6c79 2062 6520  utomatically be 
-000013f0: 6372 6561 7465 6420 7768 656e 206d 616b  created when mak
-00001400: 696e 6720 7374 6174 6d61 7073 2e20 4966  ing statmaps. If
-00001410: 2074 6865 2022 4e6f 6973 6520 766f 6c75   the "Noise volu
-00001420: 6d65 2069 6e63 6c75 6465 6420 696e 2074  me included in t
-00001430: 696d 6520 7365 7269 6573 2220 6f70 7469  ime series" opti
-00001440: 6f6e 2077 6173 2073 6574 2074 6f20 7472  on was set to tr
-00001450: 7565 2c20 6f72 206d 6f74 696f 6e20 6f75  ue, or motion ou
-00001460: 746c 6965 7220 7265 6d6f 7661 6c20 7761  tlier removal wa
-00001470: 7320 7573 6564 2077 6865 6e20 6372 6561  s used when crea
-00001480: 7469 6e67 2074 6865 2073 7461 746d 6170  ting the statmap
-00001490: 732c 2074 6869 7320 666f 6c64 6572 2077  s, this folder w
-000014a0: 696c 6c20 636f 6e74 6169 6e20 636c 6561  ill contain clea
-000014b0: 6e65 6420 7665 7273 696f 6e73 206f 6620  ned versions of 
-000014c0: 7468 6520 6f72 6967 696e 616c 2066 756e  the original fun
-000014d0: 6320 6669 6c65 732e 2048 6f77 6576 6572  c files. However
-000014e0: 2069 6620 7468 6573 6520 6f70 7469 6f6e   if these option
-000014f0: 7320 7765 7265 206e 6f74 2075 7365 6420  s were not used 
-00001500: 7768 656e 2063 7265 6174 696e 6720 7468  when creating th
-00001510: 6520 7374 6174 6d61 7073 2c20 7468 6520  e statmaps, the 
-00001520: 666f 6c64 6572 2077 696c 6c20 7374 696c  folder will stil
-00001530: 6c20 6265 2070 7265 7365 6e74 2c20 686f  l be present, ho
-00001540: 7765 7665 7220 7468 6520 6669 6c65 7320  wever the files 
-00001550: 7769 6c6c 2062 6520 6964 656e 7469 6361  will be identica
-00001560: 6c20 746f 2074 686f 7365 2069 6e20 7468  l to those in th
-00001570: 6520 2266 756e 6322 2066 6f6c 6465 722e  e "func" folder.
-00001580: da0d 6f75 7470 7574 5f66 6f6c 6465 72da  ..output_folder.
-00001590: 0744 4546 4155 4c54 7a10 4f75 7470 7574  .DEFAULTz.Output
-000015a0: 2064 6972 6563 746f 7279 7aae 4469 7265   directoryz.Dire
-000015b0: 6374 6f72 7920 746f 2073 6176 6520 6f75  ctory to save ou
-000015c0: 7470 7574 2e20 4966 2073 6574 2074 6f20  tput. If set to 
-000015d0: 4445 4641 554c 542c 206f 7574 7075 7420  DEFAULT, output 
-000015e0: 6469 7265 6374 6f72 7920 7769 6c6c 2062  directory will b
-000015f0: 6520 7365 7420 746f 2074 6865 2063 6f72  e set to the cor
-00001600: 7469 6361 6c20 6174 6c61 7320 7573 6564  tical atlas used
-00001610: 2061 7070 656e 6465 6420 7769 7468 2022   appended with "
-00001620: 5f52 4f49 5f72 6570 6f72 7422 2e20 0a45  _ROI_report". .E
-00001630: 7861 6d70 6c65 3a20 4861 7276 6172 644f  xample: HarvardO
-00001640: 7866 6f72 642d 436f 7274 6963 616c 5f52  xford-Cortical_R
-00001650: 4f49 5f72 6570 6f72 742f da03 646f 66e9  OI_report/..dof.
-00001660: 0c00 0000 5a03 444f 467a 8944 6567 7265  ....Z.DOFz.Degre
-00001670: 6573 206f 6620 6672 6565 646f 6d20 666f  es of freedom fo
-00001680: 7220 464c 4952 5420 286f 6e6c 7920 7573  r FLIRT (only us
-00001690: 6564 2066 6f72 2074 6865 2066 4d52 4920  ed for the fMRI 
-000016a0: 746f 2061 6e61 746f 6d69 6361 6c20 616c  to anatomical al
-000016b0: 6967 6e6d 656e 7420 7768 656e 2075 7369  ignment when usi
-000016c0: 6e67 2043 6f72 7265 6c61 7469 6f6e 2052  ng Correlation R
-000016d0: 6174 696f 2063 6f73 7420 6675 6e63 7469  atio cost functi
-000016e0: 6f6e 292e 2052 6563 6f6d 6d65 6e64 6564  on). Recommended
-000016f0: 3a20 3132 2904 720b 0000 0072 0c00 0000  : 12).r....r....
-00001700: 720f 0000 0072 0e00 0000 da18 616e 6174  r....r......anat
-00001710: 5f61 6c69 676e 5f63 6f73 745f 6675 6e63  _align_cost_func
-00001720: 7469 6f6e 7a20 664d 5249 2074 6f20 616e  tionz fMRI to an
-00001730: 6174 6f6d 6963 616c 2063 6f73 7420 6675  atomical cost fu
-00001740: 6e63 7469 6f6e da03 4242 527a 1143 6f72  nction..BBRz.Cor
-00001750: 7265 6c61 7469 6f6e 2052 6174 696f 612f  relation Ratioa/
-00001760: 0100 0042 4252 206f 7220 436f 7272 656c  ...BBR or Correl
-00001770: 6174 696f 6e20 5261 7469 6f2e 2052 6563  ation Ratio. Rec
-00001780: 6f6d 6d65 6e64 6564 3a20 4242 522e 0a55  ommended: BBR..U
-00001790: 7369 6e67 2042 4252 2028 426f 756e 6461  sing BBR (Bounda
-000017a0: 7279 2d42 6173 6564 2052 6567 6973 7472  ry-Based Registr
-000017b0: 6174 696f 6e29 2072 6571 7569 7265 7320  ation) requires 
-000017c0: 616e 2046 534c 2046 4153 5420 7365 676d  an FSL FAST segm
-000017d0: 656e 7461 7469 6f6e 2028 7468 6973 2077  entation (this w
-000017e0: 696c 6c20 6265 2061 7574 6f6d 6174 6963  ill be automatic
-000017f0: 616c 6c79 2063 7265 6174 6564 2069 6620  ally created if 
-00001800: 6e65 6365 7373 6172 7920 6966 2074 6865  necessary if the
-00001810: 2052 756e 2046 534c 2046 4153 5420 6f70   Run FSL FAST op
-00001820: 7469 6f6e 2069 7320 7365 7420 746f 2022  tion is set to "
-00001830: 5275 6e20 6966 2066 696c 6573 206e 6f74  Run if files not
-00001840: 2066 6f75 6e64 2229 2061 6e64 2061 2077   found") and a w
-00001850: 686f 6c65 6865 6164 206e 6f6e 2d62 7261  holehead non-bra
-00001860: 696e 2065 7874 7261 6374 6564 2061 6e61  in extracted ana
-00001870: 746f 6d69 6361 6c20 706c 6163 6564 2069  tomical placed i
-00001880: 6e20 7468 6520 616e 6174 2066 6f6c 6465  n the anat folde
-00001890: 722e 2906 720b 0000 0072 0f00 0000 720c  r.).r....r....r.
-000018a0: 0000 0072 2000 0000 7221 0000 0072 0e00  ...r ...r!...r..
-000018b0: 0000 da13 6772 6579 5f6d 6174 7465 725f  ....grey_matter_
-000018c0: 7365 676d 656e 747a 2455 7365 2046 4153  segmentz$Use FAS
-000018d0: 5420 746f 206f 6e6c 7920 696e 636c 7564  T to only includ
-000018e0: 6520 6772 6579 206d 6174 7465 7261 4601  e grey matteraF.
-000018f0: 0000 7472 7565 206f 7220 6661 6c73 652e  ..true or false.
-00001900: 2052 6563 6f6d 6d65 6e64 6564 3a20 7472   Recommended: tr
-00001910: 7565 2069 6620 7573 696e 6720 6120 636f  ue if using a co
-00001920: 7274 6963 616c 2061 746c 6173 2e0a 4e6f  rtical atlas..No
-00001930: 7465 3a20 4653 4c20 4641 5354 2073 6567  te: FSL FAST seg
-00001940: 6d65 6e74 6174 696f 6e20 6669 6c65 7320  mentation files 
-00001950: 7368 6f75 6c64 2062 6520 706c 6163 6564  should be placed
-00001960: 2069 6e20 7468 6520 7375 622d 7b69 647d   in the sub-{id}
-00001970: 2f66 736c 6661 7374 2f20 6469 7265 6374  /fslfast/ direct
-00001980: 6f72 792e 204f 6e6c 7920 7468 6520 4653  ory. Only the FS
-00001990: 4c20 4641 5354 2066 696c 6520 6170 7065  L FAST file appe
-000019a0: 6e64 6564 2077 6974 6820 7076 655f 3120  nded with pve_1 
-000019b0: 6e65 6564 7320 746f 2062 6520 696e 2074  needs to be in t
-000019c0: 6869 7320 6469 7265 6374 6f72 792c 2068  his directory, h
-000019d0: 6f77 6576 6572 2069 6620 616c 6c20 6669  owever if all fi
-000019e0: 6c65 7320 6f75 7470 7574 2062 7920 4641  les output by FA
-000019f0: 5354 2061 7265 2070 6c61 6365 6420 696e  ST are placed in
-00001a00: 2074 6869 7320 6469 7265 6374 6f72 792c   this directory,
-00001a10: 2074 6865 6e20 6652 4154 2077 696c 6c20   then fRAT will 
-00001a20: 6669 6e64 2074 6865 206e 6563 6573 7361  find the necessa
-00001a30: 7279 2066 696c 652e da0c 7275 6e5f 6673  ry file...run_fs
-00001a40: 6c5f 6661 7374 7a16 5275 6e20 6966 2066  l_fastz.Run if f
-00001a50: 696c 6573 206e 6f74 2066 6f75 6e64 7a09  iles not foundz.
-00001a60: 4e65 7665 7220 7275 6e7a 8e52 6563 6f6d  Never runz.Recom
-00001a70: 6d65 6e64 6564 3a20 2252 756e 2069 6620  mended: "Run if 
-00001a80: 6669 6c65 7320 6e6f 7420 666f 756e 6422  files not found"
-00001a90: 2e0a 5468 6573 6520 6669 6c65 7320 7769  ..These files wi
-00001aa0: 6c6c 206f 6e6c 7920 6265 2073 6561 7263  ll only be searc
-00001ab0: 6865 6420 666f 7220 2861 6e64 2074 6875  hed for (and thu
-00001ac0: 7320 6372 6561 7465 6429 2069 6620 2255  s created) if "U
-00001ad0: 7365 2046 534c 2046 4153 5420 7365 676d  se FSL FAST segm
-00001ae0: 656e 7461 7469 6f6e 2220 6973 2073 6574  entation" is set
-00001af0: 2074 6f20 7472 7565 2e7a 0c52 756e 2046   to true.z.Run F
-00001b00: 534c 2046 4153 5429 0672 0b00 0000 7220  SL FAST).r....r 
-00001b10: 0000 0072 0c00 0000 720e 0000 0072 0f00  ...r....r....r..
-00001b20: 0000 7221 0000 00da 1066 736c 6661 7374  ..r!.....fslfast
-00001b30: 5f6d 696e 5f70 726f 62da 0553 6361 6c65  _min_prob..Scale
-00001b40: 679a 9999 9999 99b9 3fe9 0000 0000 721e  g.......?.....r.
-00001b50: 0000 0067 9a99 9999 9999 a93f 7a1c 4653  ...g.......?z.FS
-00001b60: 4c20 4641 5354 206d 696e 696d 756d 2070  L FAST minimum p
-00001b70: 726f 6261 6269 6c69 7479 7a10 5265 636f  robabilityz.Reco
-00001b80: 6d6d 656e 6465 643a 2030 2e31 2907 720b  mmended: 0.1).r.
-00001b90: 0000 0072 0c00 0000 da04 4672 6f6d da02  ...r......From..
-00001ba0: 546f da0a 5265 736f 6c75 7469 6f6e 720f  To..Resolutionr.
-00001bb0: 0000 0072 0e00 0000 da0f 7374 6174 5f6d  ...r......stat_m
-00001bc0: 6170 5f66 6f6c 6465 727a 1653 7461 7469  ap_folderz.Stati
-00001bd0: 7374 6963 616c 206d 6170 2066 6f6c 6465  stical map folde
-00001be0: 727a 5146 6f6c 6465 7220 6e61 6d65 2077  rzQFolder name w
-00001bf0: 6869 6368 2063 6f6e 7461 696e 7320 7468  hich contains th
-00001c00: 6520 7374 6174 6973 7469 6361 6c20 6d61  e statistical ma
-00001c10: 7020 6669 6c65 732e 2045 7861 6d70 6c65  p files. Example
-00001c20: 3a20 7465 6d70 6f72 616c 534e 525f 7265  : temporalSNR_re
-00001c30: 706f 7274 2906 720b 0000 0072 0c00 0000  port).r....r....
-00001c40: 7221 0000 0072 0d00 0000 720f 0000 0072  r!...r....r....r
-00001c50: 0e00 0000 da0f 7374 6174 5f6d 6170 5f73  ......stat_map_s
-00001c60: 7566 6669 787a 0c5f 7453 4e52 2e6e 6969  uffixz._tSNR.nii
-00001c70: 2e67 7a7a 1653 7461 7469 7374 6963 616c  .gzz.Statistical
-00001c80: 206d 6170 2073 7566 6669 787a 5d46 696c   map suffixz]Fil
-00001c90: 6520 6e61 6d65 2073 7566 6669 7820 6f66  e name suffix of
-00001ca0: 2074 6865 2073 7461 7469 7374 6963 616c   the statistical
-00001cb0: 206d 6170 2066 696c 6573 2e20 496e 636c   map files. Incl
-00001cc0: 7564 6520 7468 6520 6669 6c65 2065 7874  ude the file ext
-00001cd0: 656e 7369 6f6e 2e20 4578 616d 706c 653a  ension. Example:
-00001ce0: 205f 7453 4e52 2e69 6d67 da11 636f 6e66   _tSNR.img..conf
-00001cf0: 5f6c 6576 656c 5f6e 756d 6265 72fa 0939  _level_number..9
-00001d00: 3525 2c20 312e 3936 2906 7a09 3830 252c  5%, 1.96).z.80%,
-00001d10: 2031 2e32 387a 0938 3525 2c20 312e 3434   1.28z.85%, 1.44
-00001d20: 7a09 3930 252c 2031 2e36 3472 4d00 0000  z.90%, 1.64rM...
-00001d30: 7a09 3938 252c 2032 2e33 337a 0939 3925  z.98%, 2.33z.99%
-00001d40: 2c20 322e 3538 7a10 436f 6e66 6964 656e  , 2.58z.Confiden
-00001d50: 6365 206c 6576 656c 7aa5 5365 7420 7468  ce levelz.Set th
-00001d60: 6520 636f 6e66 6964 656e 6365 206c 6576  e confidence lev
-00001d70: 656c 2066 6f72 2063 6f6e 6669 6465 6e63  el for confidenc
-00001d80: 6520 696e 7465 7276 616c 2063 616c 6375  e interval calcu
-00001d90: 6c61 7469 6f6e 732e 0a4e 756d 6265 7273  lations..Numbers
-00001da0: 2072 6570 7265 7365 6e74 2074 6865 2063   represent the c
-00001db0: 6f6e 6669 6465 6e63 6520 6c65 7665 6c20  onfidence level 
-00001dc0: 616e 6420 7468 6520 636f 7272 6573 706f  and the correspo
-00001dd0: 6e64 696e 6720 6372 6974 6963 616c 207a  nding critical z
-00001de0: 2076 616c 7565 2e0a 5265 636f 6d6d 656e   value..Recommen
-00001df0: 6465 643a 2039 3525 2c20 312e 3936 2e29  ded: 95%, 1.96.)
-00001e00: 0672 0b00 0000 720c 0000 0072 2000 0000  .r....r....r ...
-00001e10: 7221 0000 0072 0f00 0000 720e 0000 00da  r!...r....r.....
-00001e20: 0d62 696e 6172 795f 7061 7261 6d73 da07  .binary_params..
-00001e30: 4479 6e61 6d69 637a 1a50 6172 7369 6e67  Dynamicz.Parsing
-00001e40: 5b22 7061 7261 6d65 7465 725f 6469 6374  ["parameter_dict
-00001e50: 3122 5dda 0b43 6865 636b 6275 7474 6f6e  1"]..Checkbutton
-00001e60: 7a11 4269 6e61 7279 2070 6172 616d 6574  z.Binary paramet
-00001e70: 6572 73da 046c 6973 747a 3341 6464 2070  ers..listz3Add p
-00001e80: 6172 616d 6574 6572 7320 6865 7265 2077  arameters here w
-00001e90: 6869 6368 2077 696c 6c20 6569 7468 6572  hich will either
-00001ea0: 2062 6520 6f6e 206f 7220 6f66 662e 2907   be on or off.).
-00001eb0: 720b 0000 0072 0c00 0000 7220 0000 00da  r....r....r ....
-00001ec0: 0773 7562 7479 7065 720f 0000 0072 2100  .subtyper....r!.
-00001ed0: 0000 720e 0000 007a 114f 7574 6c69 6572  ..r....z.Outlier
-00001ee0: 2064 6574 6563 7469 6f6e da0c 6e6f 6973   detection..nois
-00001ef0: 655f 6375 746f 6666 6180 0100 0074 7275  e_cutoffa....tru
-00001f00: 6520 6f72 2066 616c 7365 2e20 4361 6c63  e or false. Calc
-00001f10: 756c 6174 6520 6120 6d69 6e69 6d75 6d20  ulate a minimum 
-00001f20: 6375 746f 6666 2076 616c 7565 2074 6f20  cutoff value to 
-00001f30: 6265 2069 6e63 6c75 6465 6420 696e 2061  be included in a
-00001f40: 6e20 524f 492c 6261 7365 6420 6f6e 2076  n ROI,based on v
-00001f50: 6f78 656c 7320 6e6f 7420 6173 7369 676e  oxels not assign
-00001f60: 6564 2061 6e20 524f 4920 6f72 2074 6861  ed an ROI or tha
-00001f70: 7420 6861 7665 2062 6565 6e20 6578 636c  t have been excl
-00001f80: 7564 6564 2066 726f 6d20 616e 616c 7973  uded from analys
-00001f90: 6973 2e20 566f 7865 6c73 2077 6974 6820  is. Voxels with 
-00001fa0: 7661 6c75 6573 206f 6620 3020 6172 6520  values of 0 are 
-00001fb0: 6e6f 7420 696e 636c 7564 6564 2077 6865  not included whe
-00001fc0: 6e20 6361 6c63 756c 6174 696e 6720 7468  n calculating th
-00001fd0: 6520 6e6f 6973 6520 6375 746f 6666 2e20  e noise cutoff. 
-00001fe0: 0a55 7365 6675 6c20 666f 7220 7374 6174  .Useful for stat
-00001ff0: 6973 7469 6361 6c20 6d61 7073 2077 6865  istical maps whe
-00002000: 7265 2065 7874 7261 6372 616e 6961 6c20  re extracranial 
-00002010: 766f 7865 6c73 2061 7265 206c 696b 656c  voxels are likel
-00002020: 7920 746f 2068 6176 6520 6d75 6368 206c  y to have much l
-00002030: 6f77 6572 2076 616c 7565 7320 7468 616e  ower values than
-00002040: 2074 686f 7365 2069 6e73 6964 6520 7468   those inside th
-00002050: 6520 6272 6169 6e20 7375 6368 2061 7320  e brain such as 
-00002060: 7453 4e52 206d 6170 732e 2052 6563 6f6d  tSNR maps. Recom
-00002070: 6d65 6e64 6564 3a20 7472 7565 2eda 1a67  mended: true...g
-00002080: 6175 7373 6961 6e5f 6f75 746c 6965 725f  aussian_outlier_
-00002090: 6465 7465 6374 696f 6e7a 2147 6175 7373  detectionz!Gauss
-000020a0: 6961 6e20 6f75 746c 6965 7220 2847 6175  ian outlier (Gau
-000020b0: 4f29 2064 6574 6563 7469 6f6e 7a6b 7472  O) detectionzktr
-000020c0: 7565 206f 7220 6661 6c73 652e 2046 6974  ue or false. Fit
-000020d0: 2061 2067 6175 7373 6961 6e20 746f 2074   a gaussian to t
-000020e0: 6865 2064 6174 6120 746f 2064 6574 6572  he data to deter
-000020f0: 6d69 6e65 206f 7574 6c69 6572 7320 7573  mine outliers us
-00002100: 696e 6720 456c 6c69 7074 6963 2045 6e76  ing Elliptic Env
-00002110: 656c 6f70 652e 2052 6563 6f6d 6d65 6e64  elope. Recommend
-00002120: 6564 3a20 7472 7565 2eda 1e67 6175 7373  ed: true...gauss
-00002130: 6961 6e5f 6f75 746c 6965 725f 636f 6e74  ian_outlier_cont
-00002140: 616d 696e 6174 696f 6e67 7b14 ae47 e17a  aminationg{..G.z
-00002150: 843f 7a1d 4761 754f 2063 6f6e 7461 6d69  .?z.GauO contami
-00002160: 6e61 7469 6f6e 2070 6572 6365 6e74 6167  nation percentag
-00002170: 657a 3850 6572 6365 6e74 206f 6620 6578  ez8Percent of ex
-00002180: 7065 6374 6564 206f 7574 6c69 6572 7320  pected outliers 
-00002190: 696e 2064 6174 6173 6574 0a52 6563 6f6d  in dataset.Recom
-000021a0: 6d65 6e64 6564 3a20 302e 31da 1967 6175  mended: 0.1..gau
-000021b0: 7373 6961 6e5f 6f75 746c 6965 725f 6c6f  ssian_outlier_lo
-000021c0: 6361 7469 6f6e fa0e 6265 6c6f 7720 6761  cation..below ga
-000021d0: 7573 7369 616e 2903 7257 0000 007a 0e61  ussian).rW...z.a
-000021e0: 626f 7665 2067 6175 7373 6961 6eda 0462  bove gaussian..b
-000021f0: 6f74 687a 0d47 6175 4f20 6c6f 6361 7469  othz.GauO locati
-00002200: 6f6e 7aa4 4461 7461 2074 6f20 7265 6d6f  onz.Data to remo
-00002210: 7665 2028 6966 2067 6175 7373 6961 6e20  ve (if gaussian 
-00002220: 6f75 746c 6965 7220 6465 7465 6374 696f  outlier detectio
-00002230: 6e20 6973 2074 7275 6529 2e0a 466f 7220  n is true)..For 
-00002240: 6578 616d 706c 653a 2069 6620 7365 7420  example: if set 
-00002250: 746f 2062 656c 6f77 2067 6175 7373 6961  to below gaussia
-00002260: 6e2c 2064 6174 6120 6265 6c6f 7720 7468  n, data below th
-00002270: 6520 6761 7573 7369 616e 2077 696c 6c20  e gaussian will 
-00002280: 6265 2072 656d 6f76 6564 2e0a 5265 636f  be removed..Reco
-00002290: 6d6d 656e 6465 643a 2062 656c 6f77 2067  mmended: below g
-000022a0: 6175 7373 6961 6e2e 5a1e 6372 6561 7465  aussian.Z.create
-000022b0: 5f73 7461 7469 7374 6963 735f 6f70 7469  _statistics_opti
-000022c0: 6f6e 735f 6669 6c65 da16 6372 6561 7465  ons_file..create
-000022d0: 5f73 7461 7469 7374 6963 735f 6669 6c65  _statistics_file
-000022e0: 7a1c 4372 6561 7465 2073 7461 7469 7374  z.Create statist
-000022f0: 6963 734f 7074 696f 6e73 2e63 7376 7a97  icsOptions.csvz.
-00002300: 4372 6561 7465 2066 696c 6520 696e 2062  Create file in b
-00002310: 6173 6520 666f 6c64 6572 2074 6f20 6368  ase folder to ch
-00002320: 6f6f 7365 2073 7461 7469 7374 6963 7320  oose statistics 
-00002330: 6f70 7469 6f6e 732e 2053 7563 6820 6173  options. Such as
-00002340: 2077 6869 6368 2070 6172 616d 6574 6572   which parameter
-00002350: 7320 746f 2065 7863 6c75 6465 2066 726f  s to exclude fro
-00002360: 6d20 616e 616c 7973 6973 2061 6e64 2077  m analysis and w
-00002370: 6861 7420 6d61 696e 2065 6666 6563 7420  hat main effect 
-00002380: 636f 6e74 7261 7374 7320 746f 2063 616c  contrasts to cal
-00002390: 6375 6c61 7465 2e29 0572 0b00 0000 722e  culate.).r....r.
-000023a0: 0000 0072 3000 0000 722f 0000 0072 0e00  ...r0...r/...r..
-000023b0: 0000 da2c 6175 746f 6d61 7469 6361 6c6c  ...,automaticall
-000023c0: 795f 6372 6561 7465 5f73 7461 7469 7374  y_create_statist
-000023d0: 6963 735f 6f70 7469 6f6e 735f 6669 6c65  ics_options_file
-000023e0: 6103 0100 0074 7275 6520 6f72 2066 616c  a....true or fal
-000023f0: 7365 2e0a 5573 7561 6c6c 7920 7374 6174  se..Usually stat
-00002400: 6973 7469 6373 4f70 7469 6f6e 732e 6373  isticsOptions.cs
-00002410: 7620 6973 2061 7574 6f6d 6174 6963 616c  v is automatical
-00002420: 6c79 2063 7265 6174 6564 2077 6865 6e20  ly created when 
-00002430: 6372 6561 7469 6e67 2070 6172 616d 5661  creating paramVa
-00002440: 6c75 6573 2e63 7376 2e20 4465 7365 6c65  lues.csv. Desele
-00002450: 6374 2074 6869 7320 6f70 7469 6f6e 2069  ct this option i
-00002460: 6620 796f 7520 776f 6e27 7420 6265 2072  f you won't be r
-00002470: 756e 6e69 6e67 2074 6865 2073 7461 7469  unning the stati
-00002480: 7374 6963 7320 7374 6570 2e20 5468 6520  stics step. The 
-00002490: 6372 6561 7465 2073 7461 7469 7374 6963  create statistic
-000024a0: 734f 7074 696f 6e73 2e63 7376 2062 7574  sOptions.csv but
-000024b0: 746f 6e20 6162 6f76 6520 6361 6e20 616c  ton above can al
-000024c0: 736f 2062 6520 7573 6564 2074 6f20 6d61  so be used to ma
-000024d0: 6e75 616c 6c79 2063 7265 6174 6520 7468  nually create th
-000024e0: 6973 2066 696c 652e 5a19 7374 6174 6973  is file.Z.statis
-000024f0: 7469 6373 5f73 7562 666f 6c64 6572 5f6e  tics_subfolder_n
-00002500: 616d 65da 0573 7461 7473 7a25 4469 7265  ame..statsz%Dire
-00002510: 6374 6f72 7920 6e61 6d65 2066 6f72 2073  ctory name for s
-00002520: 7461 7469 7374 6963 7320 666f 6c64 6572  tatistics folder
-00002530: 2e5a 0c70 7269 6e74 5f72 6573 756c 747a  .Z.print_resultz
-00002540: 1950 7269 6e74 2072 6573 756c 7473 2074  .Print results t
-00002550: 6f20 7465 726d 696e 616c 7a58 7472 7565  o terminalzXtrue
-00002560: 206f 7220 6661 6c73 652e 2050 7269 6e74   or false. Print
-00002570: 7320 7265 7375 6c74 7320 746f 2074 6572  s results to ter
-00002580: 6d69 6e61 6c20 6966 2074 7275 6520 696e  minal if true in
-00002590: 2061 6464 6974 696f 6e20 746f 2073 6176   addition to sav
-000025a0: 696e 6720 7265 7375 6c74 7320 746f 2066  ing results to f
-000025b0: 696c 652e 5a0e 6d69 6e69 6d75 6d5f 766f  ile.Z.minimum_vo
-000025c0: 7865 6c73 6990 0100 0061 9401 0000 466f  xelsi....a....Fo
-000025d0: 7220 626f 6f74 7374 7261 7070 6564 2063  r bootstrapped c
-000025e0: 6861 6e67 6520 7665 7273 7573 2062 6173  hange versus bas
-000025f0: 656c 696e 652c 2066 6f72 2065 6163 6820  eline, for each 
-00002600: 524f 492c 2074 6865 2061 7665 7261 6765  ROI, the average
-00002610: 206e 756d 6265 7220 6f66 2076 6f78 656c   number of voxel
-00002620: 7320 7065 7220 7365 7373 696f 6e20 666f  s per session fo
-00002630: 7220 616e 2052 4f49 206d 7573 7420 6265  r an ROI must be
-00002640: 2061 626f 7665 2074 6869 7320 7661 6c75   above this valu
-00002650: 6520 746f 2062 6520 696e 636c 7564 6564  e to be included
-00002660: 2069 6e20 7468 6520 616e 616c 7973 6973   in the analysis
-00002670: 2e46 6f72 2072 756e 6e69 6e67 2074 6865  .For running the
-00002680: 206c 696e 6561 7220 6d69 7865 6420 6d6f   linear mixed mo
-00002690: 6465 6c2c 2066 6f72 2065 6163 6820 524f  del, for each RO
-000026a0: 492c 2061 6e79 2073 6573 7369 6f6e 7320  I, any sessions 
-000026b0: 7769 7468 2061 2076 6f78 656c 2063 6f75  with a voxel cou
-000026c0: 6e74 2062 656c 6f77 2074 6869 7320 7661  nt below this va
-000026d0: 6c75 6520 7769 6c6c 2062 6520 7265 6d6f  lue will be remo
-000026e0: 7665 642e 0a48 6967 686c 7920 7265 636f  ved..Highly reco
-000026f0: 6d6d 656e 6465 6420 746f 2073 6574 2061  mmended to set a
-00002700: 2076 616c 7565 2068 6572 652c 2061 7320   value here, as 
-00002710: 524f 4973 2077 6974 6820 6120 736d 616c  ROIs with a smal
-00002720: 6c20 6e75 6d62 6572 206f 6620 766f 7865  l number of voxe
-00002730: 6c73 206d 6179 2073 7567 6765 7374 2070  ls may suggest p
-00002740: 6f6f 7220 6669 7474 696e 672e 0a52 6563  oor fitting..Rec
-00002750: 6f6d 6d65 6e64 6564 2076 616c 7565 2034  ommended value 4
-00002760: 3030 5a11 626f 6f74 7374 7261 705f 7361  00Z.bootstrap_sa
-00002770: 6d70 6c65 7369 e803 0000 7a69 5265 636f  mplesi....ziReco
-00002780: 6d6d 656e 6465 6420 7661 6c75 6520 3130  mmended value 10
-00002790: 3030 2e20 0a4e 6f74 653a 2042 6f6f 7473  00. .Note: Boots
-000027a0: 7472 6170 7069 6e67 2069 7320 6f6e 6c79  trapping is only
-000027b0: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
-000027c0: 7465 2070 6572 6365 6e74 6167 6520 6368  te percentage ch
-000027d0: 616e 6765 2076 6572 7375 7320 6261 7365  ange versus base
-000027e0: 6c69 6e65 2e5a 1d62 6f6f 7473 7472 6170  line.Z.bootstrap
-000027f0: 5f63 6f6e 6669 6465 6e63 655f 696e 7465  _confidence_inte
-00002800: 7276 616c e95f 0000 007a 6752 6563 6f6d  rval._...zgRecom
-00002810: 6d65 6e64 6564 2076 616c 7565 3a20 3935  mended value: 95
-00002820: 200a 4e6f 7465 3a20 426f 6f74 7374 7261   .Note: Bootstra
-00002830: 7070 696e 6720 6973 206f 6e6c 7920 7573  pping is only us
-00002840: 6564 2074 6f20 6361 6c63 756c 6174 6520  ed to calculate 
-00002850: 7065 7263 656e 7461 6765 2063 6861 6e67  percentage chang
-00002860: 6520 7665 7273 7573 2062 6173 656c 696e  e versus baselin
-00002870: 652e 5a13 7265 6769 6f6e 616c 5f73 7461  e.Z.regional_sta
-00002880: 7473 5f72 6f69 73da 0361 6c6c 7a20 524f  ts_rois..allz RO
-00002890: 4973 2074 6f20 6361 6c63 756c 6174 6520  Is to calculate 
-000028a0: 7374 6174 6973 7469 6373 2066 6f72 7a8c  statistics forz.
-000028b0: 5072 6f76 6964 6520 6120 636f 6d6d 612d  Provide a comma-
-000028c0: 7365 7061 7261 7465 6420 6c69 7374 206f  separated list o
-000028d0: 6620 7265 6769 6f6e 732c 2065 2e67 2e20  f regions, e.g. 
-000028e0: 2733 2c20 3527 2c20 7468 6520 7374 7269  '3, 5', the stri
-000028f0: 6e67 2027 616c 6c27 2066 6f72 2061 6c6c  ng 'all' for all
-00002900: 2072 6f69 7320 6f72 2074 6865 2073 7472   rois or the str
-00002910: 696e 6720 2752 756e 7469 6d65 2720 746f  ing 'Runtime' to
-00002920: 2070 726f 7669 6465 2072 6567 696f 6e73   provide regions
-00002930: 2061 7420 7275 6e74 696d 652e da13 696e   at runtime...in
-00002940: 636c 7564 655f 6173 5f76 6172 6961 626c  clude_as_variabl
-00002950: 657a 1549 4e43 4c55 4445 2041 4c4c 2056  ez.INCLUDE ALL V
-00002960: 4152 4941 424c 4553 7ae9 5365 6c65 6374  ARIABLESz.Select
-00002970: 2077 6869 6368 2076 6172 6961 626c 6573   which variables
-00002980: 2074 6f20 696e 636c 7564 6520 696e 2073   to include in s
-00002990: 7461 7469 7374 6963 616c 2061 6e61 6c79  tatistical analy
-000029a0: 7369 732e 0a55 7365 6420 746f 2064 6574  sis..Used to det
-000029b0: 6572 6d69 6e65 2077 6869 6368 2076 6172  ermine which var
-000029c0: 6961 626c 6573 2074 6f20 7573 6520 6173  iables to use as
-000029d0: 2066 6978 6564 2065 6666 6563 7473 2069   fixed effects i
-000029e0: 6e20 6c69 6e65 6172 206d 6978 6564 206d  n linear mixed m
-000029f0: 6f64 656c 7320 616e 6420 7768 6963 6820  odels and which 
-00002a00: 7661 7269 6162 6c65 7320 746f 2074 616b  variables to tak
-00002a10: 6520 696e 746f 2061 6363 6f75 6e74 2077  e into account w
-00002a20: 6865 6e20 6261 6c61 6e63 696e 6720 6461  hen balancing da
-00002a30: 7461 2066 6f72 2074 6865 206d 6169 6e20  ta for the main 
-00002a40: 6566 6665 6374 2074 2074 6573 7420 6461  effect t test da
-00002a50: 7461 2e29 0772 0b00 0000 720c 0000 0072  ta.).r....r....r
-00002a60: 0d00 0000 7220 0000 0072 5200 0000 7221  ....r ...rR...r!
-00002a70: 0000 0072 0e00 0000 5a12 6272 6169 6e5f  ...r....Z.brain_
-00002a80: 6d61 705f 705f 7468 7265 7368 7a1b 436f  map_p_threshz.Co
-00002a90: 6566 6669 6369 656e 7420 6d61 7020 702d  efficient map p-
-00002aa0: 7468 7265 7368 6f6c 647a ba50 2d76 616c  thresholdz.P-val
-00002ab0: 7565 2074 6872 6573 686f 6c64 2074 6f20  ue threshold to 
-00002ac0: 7573 6520 7768 656e 2063 7265 6174 696e  use when creatin
-00002ad0: 6720 6272 6169 6e20 636f 6566 6669 6369  g brain coeffici
-00002ae0: 656e 7420 6d61 7073 2e20 416e 7920 6669  ent maps. Any fi
-00002af0: 7865 6420 6566 6665 6374 2074 6861 7420  xed effect that 
-00002b00: 646f 6573 6e27 7420 6861 7665 2061 2070  doesn't have a p
-00002b10: 2d76 616c 7565 2065 7175 616c 2074 6f20  -value equal to 
-00002b20: 6f72 206c 6573 7320 7468 616e 2074 6869  or less than thi
-00002b30: 7320 7661 6c75 6520 7769 6c6c 206e 6f74  s value will not
-00002b40: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
-00002b50: 7468 6520 636f 6566 6669 6369 656e 7420  the coefficient 
-00002b60: 6d61 702e 0a29 0572 0b00 0000 720c 0000  map..).r....r...
-00002b70: 0072 0f00 0000 720e 0000 0072 0d00 0000  .r....r....r....
-00002b80: 7a07 542d 7465 7374 735a 0b72 756e 5f74  z.T-testsZ.run_t
-00002b90: 5f74 6573 7473 7a0f 7472 7565 206f 7220  _testsz.true or 
-00002ba0: 6661 6c73 652e 0a29 0472 0b00 0000 720d  false..).r....r.
-00002bb0: 0000 0072 0c00 0000 720e 0000 00da 0749  ...r....r......I
-00002bc0: 565f 7479 7065 7a20 4649 4c4c 2049 5620  V_typez FILL IV 
-00002bd0: 5459 5045 2041 5320 4245 5457 4545 4e2d  TYPE AS BETWEEN-
-00002be0: 5355 424a 4543 5453 da0b 4f70 7469 6f6e  SUBJECTS..Option
-00002bf0: 4d65 6e75 327a 0f57 6974 6869 6e2d 7375  Menu2z.Within-su
-00002c00: 626a 6563 7473 7a10 4265 7477 6565 6e2d  bjectsz.Between-
-00002c10: 7375 626a 6563 7473 7a07 4956 2074 7970  subjectsz.IV typ
-00002c20: 657a 5854 7970 6520 6f66 2076 6172 6961  ezXType of varia
-00002c30: 626c 6520 636f 6c6c 6563 7465 642e 2055  ble collected. U
-00002c40: 7365 6420 746f 2063 686f 6f73 6520 7768  sed to choose wh
-00002c50: 6963 6820 742d 7465 7374 2074 6f20 7573  ich t-test to us
-00002c60: 6520 666f 7220 7061 6972 7769 7365 2063  e for pairwise c
-00002c70: 6f6d 7061 7269 736f 6e73 2e29 0a72 0b00  omparisons.).r..
-00002c80: 0000 720c 0000 0072 2000 0000 7252 0000  ..r....r ...rR..
-00002c90: 0072 2100 0000 da08 4f70 7469 6f6e 7332  .r!.....Options2
-00002ca0: 720f 0000 0072 0d00 0000 da0d 4465 6661  r....r......Defa
-00002cb0: 756c 744e 756d 6265 7272 0e00 0000 7a13  ultNumberr....z.
-00002cc0: 4c69 6e65 6172 206d 6978 6564 206d 6f64  Linear mixed mod
-00002cd0: 656c 735a 1772 756e 5f6c 696e 6561 725f  elsZ.run_linear_
-00002ce0: 6d69 7865 645f 6d6f 6465 6c73 5a15 6361  mixed_modelsZ.ca
-00002cf0: 7465 676f 7269 6361 6c5f 7661 7269 6162  tegorical_variab
-00002d00: 6c65 737a 4253 656c 6563 7420 7768 6963  leszBSelect whic
-00002d10: 6820 7661 7269 6162 6c65 7320 2869 6620  h variables (if 
-00002d20: 616e 7929 2061 7265 2063 6174 6567 6f72  any) are categor
-00002d30: 6963 616c 2e20 5573 6564 2066 6f72 2074  ical. Used for t
-00002d40: 6865 204c 4d4d 2e29 0672 0b00 0000 720c  he LMM.).r....r.
-00002d50: 0000 0072 2000 0000 7252 0000 0072 2100  ...r ...rR...r!.
-00002d60: 0000 720e 0000 005a 0c6d 6169 6e5f 6566  ..r....Z.main_ef
-00002d70: 6665 6374 737a 1443 6f6d 7075 7465 206d  fectsz.Compute m
-00002d80: 6169 6e20 6566 6665 6374 737a 5374 7275  ain effectszStru
-00002d90: 6520 6f72 2066 616c 7365 2e0a 4e6f 7465  e or false..Note
-00002da0: 3a20 5468 6973 206f 7074 696f 6e20 6973  : This option is
-00002db0: 2069 6e64 6570 656e 6465 6e74 2066 726f   independent fro
-00002dc0: 6d20 7468 6520 6f74 6865 7220 6566 6665  m the other effe
-00002dd0: 6374 2063 616c 6375 6c61 7469 6f6e 732e  ct calculations.
-00002de0: 7a24 436f 6d70 7574 6520 6d61 696e 2061  z$Compute main a
-00002df0: 6e64 2069 6e74 6572 6163 7469 6f6e 2065  nd interaction e
-00002e00: 6666 6563 7473 7a1b 436f 6d70 7574 6520  ffectsz.Compute 
-00002e10: 696e 7465 7261 6374 696f 6e20 6566 6665  interaction effe
-00002e20: 6374 737a 284d 6178 696d 756d 2070 6572  ctsz(Maximum per
-00002e30: 6365 6e74 206f 6620 7365 7373 696f 6e73  cent of sessions
-00002e40: 2062 656c 6f77 2074 6872 6573 6861 4901   below threshaI.
-00002e50: 0000 5265 636f 6d6d 656e 6465 6420 7661  ..Recommended va
-00002e60: 6c75 6520 302e 200a 466f 7220 6120 6769  lue 0. .For a gi
-00002e70: 7665 6e20 524f 492c 2074 6869 7320 7661  ven ROI, this va
-00002e80: 6c75 6520 7365 7473 2074 6865 206d 6178  lue sets the max
-00002e90: 696d 756d 2070 6572 6365 6e74 206f 6620  imum percent of 
-00002ea0: 7365 7373 696f 6e73 2074 6861 7420 6361  sessions that ca
-00002eb0: 6e20 6265 2065 7863 6c75 6465 6420 2864  n be excluded (d
-00002ec0: 7565 2074 6f20 6861 7669 6e67 2069 6e73  ue to having ins
-00002ed0: 7566 6669 6369 656e 7420 766f 7865 6c20  ufficient voxel 
-00002ee0: 636f 756e 7429 2062 6566 6f72 6520 7468  count) before th
-00002ef0: 6520 524f 4920 6973 206e 6f74 2069 6e63  e ROI is not inc
-00002f00: 6c75 6465 6420 696e 2072 3220 7673 2076  luded in r2 vs v
-00002f10: 6f78 656c 2063 6f75 6e74 2073 7461 7469  oxel count stati
-00002f20: 7374 6963 732e 0a57 6974 6820 7468 6520  stics..With the 
-00002f30: 6465 6661 756c 7420 7661 6c75 6520 6f66  default value of
-00002f40: 2031 3030 2825 2920 616e 2052 4f49 2077   100(%) an ROI w
-00002f50: 696c 6c20 6e6f 7420 6265 2069 6e63 6c75  ill not be inclu
-00002f60: 6465 6420 696e 2074 6869 7320 6361 6c63  ded in this calc
-00002f70: 756c 6174 696f 6e20 6966 2061 6e79 2073  ulation if any s
-00002f80: 6573 7369 6f6e 7320 6861 7665 2062 6565  essions have bee
-00002f90: 6e20 6578 636c 7564 6564 2e29 045a 1c6d  n excluded.).Z.m
-00002fa0: 6169 6e5f 616e 645f 696e 7465 7261 6374  ain_and_interact
-00002fb0: 696f 6e5f 6566 6665 6374 735a 1369 6e74  ion_effectsZ.int
-00002fc0: 6572 6163 7469 6f6e 5f65 6666 6563 7473  eraction_effects
-00002fd0: 7a15 5232 2076 7320 766f 7865 6c20 636f  z.R2 vs voxel co
-00002fe0: 756e 7420 4c4d 4d5a 106d 6178 5f62 656c  unt LMMZ.max_bel
-00002ff0: 6f77 5f74 6872 6573 687a 094d 422c 2053  ow_threshz.MB, S
-00003000: 454e 5345 7a13 4372 6974 6963 616c 2070  ENSEz.Critical p
-00003010: 6172 616d 6574 6572 7361 5d02 0000 436f  arametersa]...Co
-00003020: 6d6d 612d 7365 7061 7261 7465 6420 6c69  mma-separated li
-00003030: 7374 206f 6620 696e 6465 7065 6e64 656e  st of independen
-00003040: 7420 7661 7269 6162 6c65 732e 0a54 6865  t variables..The
-00003050: 2063 7269 7469 6361 6c20 7061 7261 6d65   critical parame
-00003060: 7465 7220 7365 7474 696e 6773 2061 7265  ter settings are
-00003070: 2075 7365 6420 746f 2073 7570 706c 7920   used to supply 
-00003080: 7468 6520 6e61 6d65 7320 616e 6420 6669  the names and fi
-00003090: 6c65 206e 616d 6520 6162 6272 6576 6961  le name abbrevia
-000030a0: 7469 6f6e 7320 6f66 2074 6865 2069 6e64  tions of the ind
-000030b0: 6570 656e 6465 6e74 2076 6172 6961 626c  ependent variabl
-000030c0: 6573 2c20 7468 6572 6566 6f72 6520 6066  es, therefore `f
-000030d0: 5241 5460 2073 7570 706f 7274 7320 7468  RAT` supports th
-000030e0: 6520 7573 6520 6f66 2061 6e79 2070 6172  e use of any par
-000030f0: 616d 6574 6572 7320 2861 6e64 2061 6e79  ameters (and any
-00003100: 206e 756d 6265 7220 6f66 2074 6865 6d29   number of them)
-00003110: 2e0a 4173 2074 6865 7365 2063 7269 7469  ..As these criti
-00003120: 6361 6c20 7061 7261 6d65 7465 7273 2077  cal parameters w
-00003130: 696c 6c20 616c 736f 2062 6520 7573 6564  ill also be used
-00003140: 2077 6865 6e20 6c61 6265 6c6c 696e 6720   when labelling 
-00003150: 7468 6520 726f 7773 2061 6e64 2063 6f6c  the rows and col
-00003160: 756d 6e73 206f 6620 626f 7468 2074 6865  umns of both the
-00003170: 2076 696f 6c69 6e20 706c 6f74 7320 616e   violin plots an
-00003180: 6420 6869 7374 6f67 7261 6d73 2c20 7468  d histograms, th
-00003190: 6579 2073 686f 756c 6420 6265 2077 7269  ey should be wri
-000031a0: 7474 656e 2061 7320 796f 7520 7761 6e74  tten as you want
-000031b0: 2074 6865 6d20 746f 2061 7070 6561 7220   them to appear 
-000031c0: 696e 2074 6865 7365 2066 6967 7572 6573  in these figures
-000031d0: 2e0a 4e6f 7465 3a20 4c65 6176 6520 626c  ..Note: Leave bl
-000031e0: 616e 6b20 6966 2079 6f75 2064 6f20 6e6f  ank if you do no
-000031f0: 7420 7761 6e74 2074 6f20 636f 6d70 6172  t want to compar
-00003200: 6520 6265 7477 6565 6e20 6469 6666 6572  e between differ
-00003210: 656e 7420 636f 6e64 6974 696f 6e73 2c20  ent conditions, 
-00003220: 666f 7220 6578 616d 706c 652c 2069 6620  for example, if 
-00003230: 796f 7520 7769 7368 2074 6f20 7365 6520  you wish to see 
-00003240: 7468 6520 6f76 6572 616c 6c20 7453 4e52  the overall tSNR
-00003250: 2066 6f72 2065 6163 6820 7265 6769 6f6e   for each region
-00003260: 2061 6372 6f73 7320 7468 6520 656e 7469   across the enti
-00003270: 7265 2064 6174 6173 6574 2e29 0672 0b00  re dataset.).r..
-00003280: 0000 720d 0000 0072 0c00 0000 7221 0000  ..r....r....r!..
-00003290: 0072 0f00 0000 720e 0000 007a 056d 622c  .r....r....z.mb,
-000032a0: 2073 7a1f 4372 6974 6963 616c 2070 6172   sz.Critical par
-000032b0: 616d 6574 6572 2061 6262 7265 7669 6174  ameter abbreviat
-000032c0: 696f 6e61 5001 0000 436f 6d6d 612d 7365  ionaP...Comma-se
-000032d0: 7061 7261 7465 6420 6c69 7374 206f 6620  parated list of 
-000032e0: 7465 726d 7320 746f 2070 6172 7365 2074  terms to parse t
-000032f0: 6865 2066 696c 6520 6e61 6d65 2066 6f72  he file name for
-00003300: 2e20 4561 6368 2065 6e74 7279 2063 6f72  . Each entry cor
-00003310: 7265 7370 6f6e 6473 2074 6f20 6120 6372  responds to a cr
-00003320: 6974 6963 616c 2070 6172 616d 6574 6572  itical parameter
-00003330: 2061 626f 7665 2e20 0a4f 7074 696f 6e61   above. .Optiona
-00003340: 6c20 6966 2075 7369 6e67 2074 6162 6c65  l if using table
-00003350: 2070 6172 616d 6574 6572 2076 6572 6966   parameter verif
-00003360: 6963 6174 696f 6e2c 2068 6f77 6576 6572  ication, however
-00003370: 2069 6620 7468 6520 6669 6c65 206e 616d   if the file nam
-00003380: 6520 636f 6e74 6169 6e73 2074 6869 7320  e contains this 
-00003390: 696e 666f 726d 6174 696f 6e20 6974 2063  information it c
-000033a0: 616e 2075 7365 2074 6869 7320 696e 666f  an use this info
-000033b0: 726d 6174 696f 6e20 746f 2061 7574 6f2d  rmation to auto-
-000033c0: 6465 7465 6374 2074 6865 2063 7269 7469  detect the criti
-000033d0: 6361 6c20 7061 7261 6d65 7465 7273 2075  cal parameters u
-000033e0: 7365 6420 666f 7220 6561 6368 2066 4d52  sed for each fMR
-000033f0: 4920 766f 6c75 6d65 2e0a 4e6f 7465 3a20  I volume..Note: 
-00003400: 5468 6973 2066 6965 6c64 2063 616e 2062  This field can b
-00003410: 6520 626c 616e 6b2e 7a42 7472 7565 206f  e blank.zBtrue o
-00003420: 7220 6661 6c73 652e 204d 616b 6520 666f  r false. Make fo
-00003430: 6c64 6572 2073 7472 7563 7475 7265 2077  lder structure w
-00003440: 6865 6e20 6372 6561 7469 6e67 2070 6172  hen creating par
-00003450: 616d 5661 6c75 6573 2e63 7376 da04 6675  amValues.csv..fu
-00003460: 6e63 7aa9 466f 6c64 6572 2074 6f20 6669  ncz.Folder to fi
-00003470: 6e64 2066 696c 6573 2074 6f20 6164 6420  nd files to add 
-00003480: 746f 2070 6172 616d 5661 6c75 6573 2e63  to paramValues.c
-00003490: 7376 2e20 4966 2075 7369 6e67 2022 4d61  sv. If using "Ma
-000034a0: 6b65 2066 6f6c 6465 7220 7374 7275 6374  ke folder struct
-000034b0: 7572 6522 206f 7074 696f 6e2c 2074 6869  ure" option, thi
-000034c0: 7320 7769 6c6c 2062 6520 7468 6520 6469  s will be the di
-000034d0: 7265 6374 6f72 7920 7468 6520 6669 6c65  rectory the file
-000034e0: 7320 696e 2074 6865 2070 6172 7469 6369  s in the partici
-000034f0: 7061 6e74 2066 6f6c 6465 7220 7769 6c6c  pant folder will
-00003500: 2062 6520 6d6f 7665 6420 746f 2e29 04da   be moved to.)..
-00003510: 0f70 6172 616d 6574 6572 5f64 6963 7431  .parameter_dict1
-00003520: da0f 7061 7261 6d65 7465 725f 6469 6374  ..parameter_dict
-00003530: 32da 156d 616b 655f 666f 6c64 6572 5f73  2..make_folder_s
-00003540: 7472 7563 7475 7265 da0e 7061 7273 696e  tructure..parsin
-00003550: 675f 666f 6c64 6572 7a15 4765 6e65 7261  g_folderz.Genera
-00003560: 6c20 706c 6f74 2073 6574 7469 6e67 735a  l plot settingsZ
-00003570: 0870 6c6f 745f 6470 6969 5802 0000 7a0a  .plot_dpiiX...z.
-00003580: 4669 6775 7265 2044 5049 7a15 5265 636f  Figure DPIz.Reco
-00003590: 6d6d 656e 6465 6420 7661 6c75 6520 3630  mmended value 60
-000035a0: 305a 0e70 6c6f 745f 666f 6e74 5f73 697a  0Z.plot_font_siz
-000035b0: 65e9 2800 0000 7a10 4669 6775 7265 2066  e.(...z.Figure f
-000035c0: 6f6e 7420 7369 7a65 7a14 5265 636f 6d6d  ont sizez.Recomm
-000035d0: 656e 6465 6420 7661 6c75 6520 3330 5a0a  ended value 30Z.
-000035e0: 706c 6f74 5f73 6361 6c65 e90a 0000 007a  plot_scale.....z
-000035f0: 0c46 6967 7572 6520 7363 616c 657a 1452  .Figure scalez.R
-00003600: 6563 6f6d 6d65 6e64 6564 2076 616c 7565  ecommended value
-00003610: 2031 305a 106d 616b 655f 7669 6f6c 696e   10Z.make_violin
-00003620: 5f70 6c6f 747a 114d 616b 6520 7669 6f6c  _plotz.Make viol
-00003630: 696e 2070 6c6f 7473 5a10 6d61 6b65 5f62  in plotsZ.make_b
-00003640: 7261 696e 5f74 6162 6c65 7a19 4d61 6b65  rain_tablez.Make
-00003650: 2062 7261 696e 2076 6973 7561 6c69 7361   brain visualisa
-00003660: 7469 6f6e 735a 136d 616b 655f 6f6e 655f  tionsZ.make_one_
-00003670: 7265 6769 6f6e 5f66 6967 7a17 4d61 6b65  region_figz.Make
-00003680: 2072 6567 696f 6e61 6c20 6261 7263 6861   regional barcha
-00003690: 7274 735a 0e6d 616b 655f 6869 7374 6f67  rtsZ.make_histog
-000036a0: 7261 6d7a 184d 616b 6520 7265 6769 6f6e  ramz.Make region
-000036b0: 616c 2068 6973 746f 6772 616d 735a 2063  al histogramsZ c
-000036c0: 6f6c 6f72 626c 696e 645f 6672 6965 6e64  olorblind_friend
-000036d0: 6c79 5f70 6c6f 745f 636f 6c6f 7572 737a  ly_plot_coloursz
-000036e0: 2223 6666 6564 6130 2c20 2366 6562 3234  "#ffeda0, #feb24
-000036f0: 632c 2023 6663 3465 3261 2c20 2362 6430  c, #fc4e2a, #bd0
-00003700: 3032 367a 3048 6578 2076 616c 7565 7320  026z0Hex values 
-00003710: 6f66 2063 6f6c 6f75 7262 6c69 6e64 2066  of colourblind f
-00003720: 7269 656e 646c 7920 636f 6c6f 7572 2073  riendly colour s
-00003730: 6361 6c65 2e5a 1172 6567 696f 6e61 6c5f  cale.Z.regional_
-00003740: 6669 675f 726f 6973 7a0c 524f 4973 2074  fig_roisz.ROIs t
-00003750: 6f20 706c 6f74 7a93 5072 6f76 6964 6520  o plotz.Provide 
-00003760: 6120 636f 6d6d 612d 7365 7061 7261 7465  a comma-separate
-00003770: 6420 6c69 7374 206f 6620 7265 6769 6f6e  d list of region
-00003780: 7320 746f 2070 6c6f 7420 652e 672e 2027  s to plot e.g. '
-00003790: 332c 2035 272c 2074 6865 2073 7472 696e  3, 5', the strin
-000037a0: 6720 2761 6c6c 2720 666f 7220 616c 6c20  g 'all' for all 
-000037b0: 726f 6973 206f 7220 7468 6520 7374 7269  rois or the stri
-000037c0: 6e67 2027 5275 6e74 696d 6527 2074 6f20  ng 'Runtime' to 
-000037d0: 7072 6f76 6964 6520 7265 6769 6f6e 7320  provide regions 
-000037e0: 6174 2072 756e 7469 6d65 2e7a 0b42 7261  at runtime.z.Bra
-000037f0: 696e 2074 6162 6c65 5a12 6272 6169 6e5f  in tableZ.brain_
-00003800: 7469 6768 745f 6c61 796f 7574 7a50 7472  tight_layoutzPtr
-00003810: 7565 206f 7220 6661 6c73 652e 2055 7365  ue or false. Use
-00003820: 2061 2074 6967 6874 206c 6179 6f75 7420   a tight layout 
-00003830: 7768 656e 206c 6179 696e 6720 6f75 7420  when laying out 
-00003840: 7468 6520 6669 6775 7265 2e20 5265 636f  the figure. Reco
-00003850: 6d6d 656e 6465 643a 2066 616c 7365 5a13  mmended: falseZ.
-00003860: 6272 6169 6e5f 6669 675f 7661 6c75 655f  brain_fig_value_
-00003870: 6d69 6e7a 1d4d 696e 696d 756d 206d 6564  minz.Minimum med
-00003880: 6961 6e20 616e 6420 6d65 616e 2076 616c  ian and mean val
-00003890: 7565 7ab6 5072 6f76 6964 6573 2074 6865  uez.Provides the
-000038a0: 206d 696e 696d 756d 2076 616c 7565 206f   minimum value o
-000038b0: 6620 7468 6520 636f 6c6f 7572 6261 7220  f the colourbar 
-000038c0: 7768 656e 2063 7265 6174 696e 6720 6d65  when creating me
-000038d0: 616e 2061 6e64 206d 6564 6961 6e20 696d  an and median im
-000038e0: 6167 6573 2e20 466f 7220 6578 616d 706c  ages. For exampl
-000038f0: 652c 2073 6574 206d 696e 696d 756d 2074  e, set minimum t
-00003900: 6f20 3530 2074 6f20 6d61 6b65 2061 7265  o 50 to make are
-00003910: 6173 2077 6974 6820 7661 6c75 6573 2062  as with values b
-00003920: 656c 6f77 2035 3020 6170 7065 6172 2062  elow 50 appear b
-00003930: 6c61 636b 2e0a 5265 636f 6d6d 656e 6465  lack..Recommende
-00003940: 6420 7661 6c75 653a 2030 5a13 6272 6169  d value: 0Z.brai
-00003950: 6e5f 6669 675f 7661 6c75 655f 6d61 784e  n_fig_value_maxN
-00003960: 7a1d 4d61 7869 6d75 6d20 6d65 6469 616e  z.Maximum median
-00003970: 2061 6e64 206d 6561 6e20 7661 6c75 6561   and mean valuea
-00003980: 0701 0000 5072 6f76 6964 6573 2074 6865  ....Provides the
-00003990: 206d 6178 696d 756d 2076 616c 7565 206f   maximum value o
-000039a0: 6620 7468 6520 636f 6c6f 7572 6261 7220  f the colourbar 
-000039b0: 7768 656e 2063 7265 6174 696e 6720 6d65  when creating me
-000039c0: 616e 2061 6e64 206d 6564 6961 6e20 696d  an and median im
-000039d0: 6167 6573 2e20 466f 7220 6578 616d 706c  ages. For exampl
-000039e0: 652c 2073 6574 206d 6178 696d 756d 2074  e, set maximum t
-000039f0: 6f20 3530 2074 6f20 6d61 6b65 2061 7265  o 50 to make are
-00003a00: 6173 2077 6974 6820 7661 6c75 6573 2061  as with values a
-00003a10: 626f 7665 2035 3020 6170 7065 6172 2061  bove 50 appear a
-00003a20: 7320 7468 6520 6272 6967 6865 7374 2063  s the brighest c
-00003a30: 6f6c 6f75 7220 6f6e 2074 6865 2063 6f6c  olour on the col
-00003a40: 6f75 7262 6172 2e0a 5265 636f 6d6d 656e  ourbar..Recommen
-00003a50: 6465 6420 7661 6c75 653a 204e 6f6e 652e  ded value: None.
-00003a60: 204e 6f74 653a 2077 696c 6c20 6465 6661   Note: will defa
-00003a70: 756c 7420 746f 2031 3030 2066 6f72 2073  ult to 100 for s
-00003a80: 6361 6c65 6420 6d61 7073 2e5a 0d62 7261  caled maps.Z.bra
-00003a90: 696e 5f78 5f63 6f6f 7264 e9ff ffff ff7a  in_x_coord.....z
-00003aa0: 6656 6f78 656c 206c 6f63 6174 696f 6e20  fVoxel location 
-00003ab0: 746f 2073 6c69 6365 2074 6865 2069 6d61  to slice the ima
-00003ac0: 6765 7320 6174 2069 6e20 7468 6520 7820  ges at in the x 
-00003ad0: 6178 6973 2e20 5265 636f 6d6d 656e 6465  axis. Recommende
-00003ae0: 6420 7365 7474 696e 6773 2066 6f72 2062  d settings for b
-00003af0: 6f74 6820 7661 7269 6162 6c65 733a 2039  oth variables: 9
-00003b00: 3120 6f72 2035 385a 0d62 7261 696e 5f7a  1 or 58Z.brain_z
-00003b10: 5f63 6f6f 7264 e913 0000 007a 6656 6f78  _coord.....zfVox
-00003b20: 656c 206c 6f63 6174 696f 6e20 746f 2073  el location to s
-00003b30: 6c69 6365 2074 6865 2069 6d61 6765 7320  lice the images 
-00003b40: 6174 2069 6e20 7468 6520 7a20 6178 6973  at in the z axis
-00003b50: 2e20 5265 636f 6d6d 656e 6465 6420 7365  . Recommended se
-00003b60: 7474 696e 6773 2066 6f72 2062 6f74 6820  ttings for both 
-00003b70: 7661 7269 6162 6c65 733a 2039 3120 6f72  variables: 91 or
-00003b80: 2035 38da 1662 7261 696e 5f74 6162 6c65   58..brain_table
-00003b90: 5f63 6f6c 5f6c 6162 656c 737a 1743 4841  _col_labelsz.CHA
-00003ba0: 4e47 4520 544f 2044 4553 4952 4544 204c  NGE TO DESIRED L
-00003bb0: 4142 454c 7a0d 436f 6c75 6d6e 206c 6162  ABELz.Column lab
-00003bc0: 656c 737a 124c 6162 656c 2066 6f72 2063  elsz.Label for c
-00003bd0: 6f6c 756d 6e73 2e29 0672 0b00 0000 720c  olumns.).r....r.
-00003be0: 0000 0072 2100 0000 720f 0000 0072 6200  ...r!...r....rb.
-00003bf0: 0000 720e 0000 00da 1662 7261 696e 5f74  ..r......brain_t
-00003c00: 6162 6c65 5f72 6f77 5f6c 6162 656c 737a  able_row_labelsz
-00003c10: 0a52 6f77 206c 6162 656c 737a 0f4c 6162  .Row labelsz.Lab
-00003c20: 656c 2066 6f72 2072 6f77 732e da10 6272  el for rows...br
-00003c30: 6169 6e5f 7461 626c 655f 636f 6c73 2907  ain_table_cols).
-00003c40: 720b 0000 0072 0c00 0000 7220 0000 0072  r....r....r ...r
-00003c50: 5200 0000 7221 0000 0072 6200 0000 720e  R...r!...rb...r.
-00003c60: 0000 00da 1062 7261 696e 5f74 6162 6c65  .....brain_table
-00003c70: 5f72 6f77 737a 0b56 696f 6c69 6e20 706c  _rowsz.Violin pl
-00003c80: 6f74 5a0d 7461 626c 655f 785f 6c61 6265  otZ.table_x_labe
-00003c90: 6c7a 0974 534e 5220 6d65 616e 5a0d 7461  lz.tSNR meanZ.ta
-00003ca0: 626c 655f 795f 6c61 6265 6c5a 0352 4f49  ble_y_labelZ.ROI
-00003cb0: 5a10 7669 6f6c 696e 5f73 686f 775f 6461  Z.violin_show_da
-00003cc0: 7461 7a10 5368 6f77 2064 6174 6120 706f  taz.Show data po
-00003cd0: 696e 7473 5a0d 7669 6f6c 696e 5f6a 6974  intsZ.violin_jit
-00003ce0: 7465 727a 124a 6974 7465 7220 6461 7461  terz.Jitter data
-00003cf0: 2070 6f69 6e74 735a 0d76 696f 6c69 6e5f   pointsZ.violin_
-00003d00: 636f 6c6f 7572 7a07 2366 6334 6532 617a  colourz.#fc4e2az
-00003d10: 2c50 6c6f 7474 696e 675b 2263 6f6c 6f72  ,Plotting["color
-00003d20: 626c 696e 645f 6672 6965 6e64 6c79 5f70  blind_friendly_p
-00003d30: 6c6f 745f 636f 6c6f 7572 7322 5d7a 5d48  lot_colours"]z]H
-00003d40: 6578 2076 616c 7565 206f 6620 636f 6c6f  ex value of colo
-00003d50: 7572 2062 6c69 6e64 2066 7269 656e 646c  ur blind friendl
-00003d60: 7920 636f 6c6f 7572 2e20 5661 6c75 6520  y colour. Value 
-00003d70: 7461 6b65 6e20 6672 6f6d 2063 6f6c 6f72  taken from color
-00003d80: 626c 696e 6420 6672 6965 6e64 6c79 2070  blind friendly p
-00003d90: 6c6f 7420 636f 6c6f 7572 732e 5a0e 626f  lot colours.Z.bo
-00003da0: 7870 6c6f 745f 636f 6c6f 7572 7a07 2366  xplot_colourz.#f
-00003db0: 6562 3234 63da 0a74 6162 6c65 5f63 6f6c  eb24c..table_col
-00003dc0: 73da 0a74 6162 6c65 5f72 6f77 737a 1252  s..table_rowsz.R
-00003dd0: 6567 696f 6e61 6c20 6261 7220 6368 6172  egional bar char
-00003de0: 745a 1673 696e 676c 655f 726f 695f 6669  tZ.single_roi_fi
-00003df0: 675f 6c61 6265 6c5f 787a 104d 756c 7469  g_label_xz.Multi
-00003e00: 6261 6e64 2066 6163 746f 725a 1673 696e  band factorZ.sin
-00003e10: 676c 655f 726f 695f 6669 675f 6c61 6265  gle_roi_fig_labe
-00003e20: 6c5f 797a 1e74 656d 706f 7261 6c20 5369  l_yz.temporal Si
-00003e30: 676e 616c 2074 6f20 4e6f 6973 6520 5261  gnal to Noise Ra
-00003e40: 7469 6f5a 1973 696e 676c 655f 726f 695f  tioZ.single_roi_
-00003e50: 6669 675f 6c61 6265 6c5f 6669 6c6c 7a0c  fig_label_fillz.
-00003e60: 5345 4e53 4520 6661 6374 6f72 da15 7369  SENSE factor..si
-00003e70: 6e67 6c65 5f72 6f69 5f66 6967 5f78 5f61  ngle_roi_fig_x_a
-00003e80: 7869 7372 1d00 0000 7a09 4269 6e20 7769  xisr....z.Bin wi
-00003e90: 6474 687a 0c78 2d61 7869 7320 6c61 6265  dthz.x-axis labe
-00003ea0: 6cda 0946 7265 7175 656e 6379 7a0c 792d  l..Frequencyz.y-
-00003eb0: 6178 6973 206c 6162 656c 6700 0000 0000  axis labelg.....
-00003ec0: 00f8 3f7a 1353 7461 7469 7374 6963 206c  ..?z.Statistic l
-00003ed0: 696e 6520 7369 7a65 7a09 5368 6f77 206d  ine sizez.Show m
-00003ee0: 6561 6e7a 0b53 686f 7720 6d65 6469 616e  eanz.Show median
-00003ef0: 7a0b 5368 6f77 206c 6567 656e 647a 0c78  z.Show legendz.x
-00003f00: 2d61 7869 7320 6661 6365 7429 0872 0b00  -axis facet).r..
-00003f10: 0000 720c 0000 0072 0f00 0000 7220 0000  ..r....r....r ..
-00003f20: 0072 5200 0000 7221 0000 0072 6200 0000  .rR...r!...rb...
-00003f30: 720e 0000 007a 0c79 2d61 7869 7320 6661  r....z.y-axis fa
-00003f40: 6365 747a 0a42 696e 2063 6f6c 6f75 7229  cetz.Bin colour)
-00003f50: 0772 0b00 0000 720c 0000 0072 0f00 0000  .r....r....r....
-00003f60: 7220 0000 0072 5200 0000 7221 0000 0072  r ...rR...r!...r
-00003f70: 0e00 0000 290c da15 7369 6e67 6c65 5f72  ....)...single_r
-00003f80: 6f69 5f66 6967 5f63 6f6c 6f75 727a 1252  oi_fig_colourz.R
-00003f90: 6567 696f 6e61 6c20 6869 7374 6f67 7261  egional histogra
-00003fa0: 6d5a 1268 6973 746f 6772 616d 5f62 696e  mZ.histogram_bin
-00003fb0: 7769 6474 685a 1568 6973 746f 6772 616d  widthZ.histogram
-00003fc0: 5f66 6967 5f6c 6162 656c 5f78 5a15 6869  _fig_label_xZ.hi
-00003fd0: 7374 6f67 7261 6d5f 6669 675f 6c61 6265  stogram_fig_labe
-00003fe0: 6c5f 795a 1868 6973 746f 6772 616d 5f73  l_yZ.histogram_s
-00003ff0: 7461 745f 6c69 6e65 5f73 697a 655a 1368  tat_line_sizeZ.h
-00004000: 6973 746f 6772 616d 5f73 686f 775f 6d65  istogram_show_me
-00004010: 616e 5a15 6869 7374 6f67 7261 6d5f 7368  anZ.histogram_sh
-00004020: 6f77 5f6d 6564 6961 6e5a 1568 6973 746f  ow_medianZ.histo
-00004030: 6772 616d 5f73 686f 775f 6c65 6765 6e64  gram_show_legend
-00004040: da15 6869 7374 6f67 7261 6d5f 6669 675f  ..histogram_fig_
-00004050: 785f 6661 6365 74da 1568 6973 746f 6772  x_facet..histogr
-00004060: 616d 5f66 6967 5f79 5f66 6163 6574 5a14  am_fig_y_facetZ.
-00004070: 6869 7374 6f67 7261 6d5f 6669 675f 636f  histogram_fig_co
-00004080: 6c6f 7572 2907 da07 5f5f 646f 635f 5fda  lour)...__doc__.
-00004090: 0570 6167 6573 7202 0000 0072 0300 0000  .pagesr....r....
-000040a0: 7204 0000 0072 0500 0000 7206 0000 00a9  r....r....r.....
-000040b0: 0072 7900 0000 7279 0000 00fa 5c2f 5573  .ry...ry....\/Us
-000040c0: 6572 732f 6c70 7865 6831 302f 446f 6375  ers/lpxeh10/Docu
-000040d0: 6d65 6e74 732f 5265 706f 7369 746f 7269  ments/Repositori
-000040e0: 6573 2f66 4d52 495f 524f 495f 616e 616c  es/fMRI_ROI_anal
-000040f0: 7973 6973 5f74 6f6f 6c2f 6652 4154 2f75  ysis_tool/fRAT/u
-00004100: 7469 6c73 2f66 5241 545f 636f 6e66 6967  tils/fRAT_config
-00004110: 5f73 6574 7570 2e70 79da 083c 6d6f 6475  _setup.py..<modu
-00004120: 6c65 3e01 0000 0073 b803 0000 0400 0801  le>....s........
-00004130: 0202 0201 0601 0201 0201 0201 04fd 02ff  ................
-00004140: 0606 0201 0401 04fe 02fa 060a 0201 0401  ................
-00004150: 04fe 02f6 060e 0401 04ff 02f2 0611 0401  ................
-00004160: 04ff 02ef 0614 0201 04ff 02ec 0c17 0201  ................
-00004170: 0201 04fe 02e9 081b 0201 0201 04fe 02e5  ................
-00004180: 081f 0201 0201 04fe 02e1 0423 0201 0601  ...........#....
-00004190: 0201 0201 04fc 02dd 082d 0201 04ff 02d3  .........-......
-000041a0: 0e32 0401 04ff 02ce 0835 02cb 0a37 0201  .2.......5...7..
-000041b0: 04ff 02c9 043a 0201 0601 0201 0201 04fc  .....:..........
-000041c0: 02c6 0641 0201 04ff 04bf 0246 0201 0a01  ...A.......F....
-000041d0: 0601 020f 04f0 02ff 0813 0201 04ff 02ed  ................
-000041e0: 0a1d 0201 04ff 02e3 0822 0201 04ff 02de  ........."......
-000041f0: 0426 0201 0201 0601 0201 0201 04fb 02da  .&..............
-00004200: 0432 0401 0201 04fe 02ce 043a 0601 0201  .2.........:....
-00004210: 0201 0202 0201 04fa 02c6 0c42 0401 04ff  ...........B....
-00004220: 02be 0845 0201 0201 0201 04fd 02bb 084b  ...E...........K
-00004230: 0201 0201 0201 04fd 02b5 0654 0601 0401  ...........T....
-00004240: 0201 04fd 02ac 0a5b 0401 0401 04fe 02a5  .......[........
-00004250: 085f 02a1 0661 0201 04ff 029f 0668 0201  ._...a.......h..
-00004260: 0201 04fe 0298 0c6d 0201 0201 04fe 0293  .......m........
-00004270: 0672 0601 0401 0201 04fd 048e 027a 0201  .r...........z..
-00004280: 0801 0201 0201 04fe 02ff 0407 0201 0201  ................
-00004290: 04fe 02f9 040f 0201 0201 0201 04fd 02f1  ................
-000042a0: 0614 0201 0201 04fe 02ec 0419 0201 0201  ................
-000042b0: 04fe 02e7 0624 0201 04ff 02dc 0629 0201  .....$.......)..
-000042c0: 04ff 02d7 082e 0201 0201 04fe 02d2 0633  ...............3
-000042d0: 0201 0201 0201 0201 0201 04fb 02cd 063d  ...............=
-000042e0: 0201 0201 0203 04fb 02c3 0844 02bc 0646  ...........D...F
-000042f0: 0201 0201 04fe 02ba 064a 0201 0a01 0601  .........J......
-00004300: 0201 04fc 02b6 085a 02a6 065c 0201 0201  .......Z...\....
-00004310: 04fe 02a4 0a60 0201 0201 0201 04fd 02a0  .....`..........
-00004320: 0465 0201 0201 0201 04fd 029b 026b 0201  .e...........k..
-00004330: 0201 0201 04fd 0206 0201 0201 0201 04fd  ................
-00004340: 0606 0602 0201 04ff 0887 007f 0203 0202  ................
-00004350: 0201 0601 0201 04fd 020e 0201 0401 0201  ................
-00004360: 0201 04fc 040b 0201 04ff 0603 0201 04ff  ................
-00004370: 06e3 0223 0201 0801 02ff 0803 0201 04ff  ...#............
-00004380: 02fd 0806 0201 04ff 02fa 0809 0201 04ff  ................
-00004390: 02f7 080c 0201 04ff 02f4 080f 0201 04ff  ................
-000043a0: 02f1 0812 0201 04ff 02ee 0815 0201 04ff  ................
-000043b0: 02eb 0618 0201 0201 04fe 02e8 0a1c 0201  ................
-000043c0: 04ff 02e4 0820 02e0 0622 0201 04ff 02de  ..... ..."......
-000043d0: 0825 0201 04ff 02db 082b 0201 04ff 02d5  .%.......+......
-000043e0: 0631 0201 04ff 02cf 0a35 0401 04ff 02cb  .1.......5......
-000043f0: 0c39 0401 0601 06fe 04c7 0c3d 0401 0601  .9.........=....
-00004400: 06fe 02c3 0a41 0401 0401 06fe 02bf 0a45  .....A.........E
-00004410: 0401 0401 06fe 02bb 0a49 02b7 0c4b 0201  .........I...K..
-00004420: 04ff 02b5 0c4e 0201 04ff 02b2 0c51 0201  .....N.......Q..
-00004430: 04ff 02af 0c54 0201 04ff 02ac 0a57 0401  .....T.......W..
-00004440: 0401 0401 04fd 02a9 0a5c 0401 0401 0401  .........\......
-00004450: 04fd 02a4 0a61 0601 0201 06fe 029f 0a65  .....a.........e
-00004460: 0601 0201 06fe 029b 0a69 0297 0c6b 0201  .........i...k..
-00004470: 04ff 0295 0c6e 0201 04ff 0292 0c71 0201  .....n.......q..
-00004480: 04ff 028f 0a74 0601 0201 06fe 048c 0678  .....t.........x
-00004490: 0601 0201 06fe 0604 1002 0602 0601 0201  ................
-000044a0: 04fe 0604 0601 0201 04fe 0a04 0201 04ff  ................
-000044b0: 0803 0201 04ff 0803 0201 04ff 0803 0201  ................
-000044c0: 04ff 0803 0201 0601 0201 06fd 0805 0201  ................
-000044d0: 0401 0401 06fd 0a05 0401 0401 0401 06fd  ................
-000044e0: 0081 0ee1                                ....
+00001340: 6465 725f 6e61 6d65 5a11 6675 6e63 5f70  der_nameZ.func_p
+00001350: 7265 7072 6f63 6573 7365 6461 2f02 0000  reprocesseda/...
+00001360: 466f 6c64 6572 2066 6f75 6e64 2069 6e20  Folder found in 
+00001370: 6561 6368 2073 7562 6a65 6374 7320 6469  each subjects di
+00001380: 7265 6374 6f72 7920 636f 6e74 6169 6e69  rectory containi
+00001390: 6e67 2074 6865 2066 696c 6573 2074 6f20  ng the files to 
+000013a0: 6265 2061 6e61 6c79 7365 642e 2066 756e  be analysed. fun
+000013b0: 635f 7072 6570 726f 6365 7373 6564 2069  c_preprocessed i
+000013c0: 7320 7468 6520 6465 6661 756c 7420 6f70  s the default op
+000013d0: 7469 6f6e 2061 7320 7468 6973 2066 6f6c  tion as this fol
+000013e0: 6465 7220 7769 6c6c 2061 7574 6f6d 6174  der will automat
+000013f0: 6963 616c 6c79 2062 6520 6372 6561 7465  ically be create
+00001400: 6420 7768 656e 206d 616b 696e 6720 7374  d when making st
+00001410: 6174 6d61 7073 2e20 4966 2074 6865 2022  atmaps. If the "
+00001420: 4e6f 6973 6520 766f 6c75 6d65 2069 6e63  Noise volume inc
+00001430: 6c75 6465 6420 696e 2074 696d 6520 7365  luded in time se
+00001440: 7269 6573 2220 6f70 7469 6f6e 2077 6173  ries" option was
+00001450: 2073 6574 2074 6f20 7472 7565 2c20 6f72   set to true, or
+00001460: 206d 6f74 696f 6e20 6f75 746c 6965 7220   motion outlier 
+00001470: 7265 6d6f 7661 6c20 7761 7320 7573 6564  removal was used
+00001480: 2077 6865 6e20 6372 6561 7469 6e67 2074   when creating t
+00001490: 6865 2073 7461 746d 6170 732c 2074 6869  he statmaps, thi
+000014a0: 7320 666f 6c64 6572 2077 696c 6c20 636f  s folder will co
+000014b0: 6e74 6169 6e20 7072 6570 726f 6365 7373  ntain preprocess
+000014c0: 6564 2076 6572 7369 6f6e 7320 6f66 2074  ed versions of t
+000014d0: 6865 206f 7269 6769 6e61 6c20 6675 6e63  he original func
+000014e0: 2066 696c 6573 2e20 486f 7765 7665 7220   files. However 
+000014f0: 6966 2074 6865 7365 206f 7074 696f 6e73  if these options
+00001500: 2077 6572 6520 6e6f 7420 7573 6564 2077   were not used w
+00001510: 6865 6e20 6372 6561 7469 6e67 2074 6865  hen creating the
+00001520: 2073 7461 746d 6170 732c 2074 6865 2066   statmaps, the f
+00001530: 6f6c 6465 7220 7769 6c6c 2073 7469 6c6c  older will still
+00001540: 2062 6520 7072 6573 656e 742c 2068 6f77   be present, how
+00001550: 6576 6572 2074 6865 2066 696c 6573 2077  ever the files w
+00001560: 696c 6c20 6265 2069 6465 6e74 6963 616c  ill be identical
+00001570: 2074 6f20 7468 6f73 6520 696e 2074 6865   to those in the
+00001580: 2022 6675 6e63 2220 666f 6c64 6572 2eda   "func" folder..
+00001590: 0d6f 7574 7075 745f 666f 6c64 6572 da07  .output_folder..
+000015a0: 4445 4641 554c 547a 104f 7574 7075 7420  DEFAULTz.Output 
+000015b0: 6469 7265 6374 6f72 797a ae44 6972 6563  directoryz.Direc
+000015c0: 746f 7279 2074 6f20 7361 7665 206f 7574  tory to save out
+000015d0: 7075 742e 2049 6620 7365 7420 746f 2044  put. If set to D
+000015e0: 4546 4155 4c54 2c20 6f75 7470 7574 2064  EFAULT, output d
+000015f0: 6972 6563 746f 7279 2077 696c 6c20 6265  irectory will be
+00001600: 2073 6574 2074 6f20 7468 6520 636f 7274   set to the cort
+00001610: 6963 616c 2061 746c 6173 2075 7365 6420  ical atlas used 
+00001620: 6170 7065 6e64 6564 2077 6974 6820 225f  appended with "_
+00001630: 524f 495f 7265 706f 7274 222e 200a 4578  ROI_report". .Ex
+00001640: 616d 706c 653a 2048 6172 7661 7264 4f78  ample: HarvardOx
+00001650: 666f 7264 2d43 6f72 7469 6361 6c5f 524f  ford-Cortical_RO
+00001660: 495f 7265 706f 7274 2fda 0364 6f66 e90c  I_report/..dof..
+00001670: 0000 005a 0344 4f46 7a89 4465 6772 6565  ...Z.DOFz.Degree
+00001680: 7320 6f66 2066 7265 6564 6f6d 2066 6f72  s of freedom for
+00001690: 2046 4c49 5254 2028 6f6e 6c79 2075 7365   FLIRT (only use
+000016a0: 6420 666f 7220 7468 6520 664d 5249 2074  d for the fMRI t
+000016b0: 6f20 616e 6174 6f6d 6963 616c 2061 6c69  o anatomical ali
+000016c0: 676e 6d65 6e74 2077 6865 6e20 7573 696e  gnment when usin
+000016d0: 6720 436f 7272 656c 6174 696f 6e20 5261  g Correlation Ra
+000016e0: 7469 6f20 636f 7374 2066 756e 6374 696f  tio cost functio
+000016f0: 6e29 2e20 5265 636f 6d6d 656e 6465 643a  n). Recommended:
+00001700: 2031 3229 0472 0b00 0000 720c 0000 0072   12).r....r....r
+00001710: 0f00 0000 720e 0000 00da 1861 6e61 745f  ....r......anat_
+00001720: 616c 6967 6e5f 636f 7374 5f66 756e 6374  align_cost_funct
+00001730: 696f 6e7a 2066 4d52 4920 746f 2061 6e61  ionz fMRI to ana
+00001740: 746f 6d69 6361 6c20 636f 7374 2066 756e  tomical cost fun
+00001750: 6374 696f 6eda 0342 4252 7a11 436f 7272  ction..BBRz.Corr
+00001760: 656c 6174 696f 6e20 5261 7469 6f61 2f01  elation Ratioa/.
+00001770: 0000 4242 5220 6f72 2043 6f72 7265 6c61  ..BBR or Correla
+00001780: 7469 6f6e 2052 6174 696f 2e20 5265 636f  tion Ratio. Reco
+00001790: 6d6d 656e 6465 643a 2042 4252 2e0a 5573  mmended: BBR..Us
+000017a0: 696e 6720 4242 5220 2842 6f75 6e64 6172  ing BBR (Boundar
+000017b0: 792d 4261 7365 6420 5265 6769 7374 7261  y-Based Registra
+000017c0: 7469 6f6e 2920 7265 7175 6972 6573 2061  tion) requires a
+000017d0: 6e20 4653 4c20 4641 5354 2073 6567 6d65  n FSL FAST segme
+000017e0: 6e74 6174 696f 6e20 2874 6869 7320 7769  ntation (this wi
+000017f0: 6c6c 2062 6520 6175 746f 6d61 7469 6361  ll be automatica
+00001800: 6c6c 7920 6372 6561 7465 6420 6966 206e  lly created if n
+00001810: 6563 6573 7361 7279 2069 6620 7468 6520  ecessary if the 
+00001820: 5275 6e20 4653 4c20 4641 5354 206f 7074  Run FSL FAST opt
+00001830: 696f 6e20 6973 2073 6574 2074 6f20 2252  ion is set to "R
+00001840: 756e 2069 6620 6669 6c65 7320 6e6f 7420  un if files not 
+00001850: 666f 756e 6422 2920 616e 6420 6120 7768  found") and a wh
+00001860: 6f6c 6568 6561 6420 6e6f 6e2d 6272 6169  olehead non-brai
+00001870: 6e20 6578 7472 6163 7465 6420 616e 6174  n extracted anat
+00001880: 6f6d 6963 616c 2070 6c61 6365 6420 696e  omical placed in
+00001890: 2074 6865 2061 6e61 7420 666f 6c64 6572   the anat folder
+000018a0: 2e29 0672 0b00 0000 720f 0000 0072 0c00  .).r....r....r..
+000018b0: 0000 7220 0000 0072 2100 0000 720e 0000  ..r ...r!...r...
+000018c0: 00da 1367 7265 795f 6d61 7474 6572 5f73  ...grey_matter_s
+000018d0: 6567 6d65 6e74 7a24 5573 6520 4641 5354  egmentz$Use FAST
+000018e0: 2074 6f20 6f6e 6c79 2069 6e63 6c75 6465   to only include
+000018f0: 2067 7265 7920 6d61 7474 6572 6146 0100   grey matteraF..
+00001900: 0074 7275 6520 6f72 2066 616c 7365 2e20  .true or false. 
+00001910: 5265 636f 6d6d 656e 6465 643a 2074 7275  Recommended: tru
+00001920: 6520 6966 2075 7369 6e67 2061 2063 6f72  e if using a cor
+00001930: 7469 6361 6c20 6174 6c61 732e 0a4e 6f74  tical atlas..Not
+00001940: 653a 2046 534c 2046 4153 5420 7365 676d  e: FSL FAST segm
+00001950: 656e 7461 7469 6f6e 2066 696c 6573 2073  entation files s
+00001960: 686f 756c 6420 6265 2070 6c61 6365 6420  hould be placed 
+00001970: 696e 2074 6865 2073 7562 2d7b 6964 7d2f  in the sub-{id}/
+00001980: 6673 6c66 6173 742f 2064 6972 6563 746f  fslfast/ directo
+00001990: 7279 2e20 4f6e 6c79 2074 6865 2046 534c  ry. Only the FSL
+000019a0: 2046 4153 5420 6669 6c65 2061 7070 656e   FAST file appen
+000019b0: 6465 6420 7769 7468 2070 7665 5f31 206e  ded with pve_1 n
+000019c0: 6565 6473 2074 6f20 6265 2069 6e20 7468  eeds to be in th
+000019d0: 6973 2064 6972 6563 746f 7279 2c20 686f  is directory, ho
+000019e0: 7765 7665 7220 6966 2061 6c6c 2066 696c  wever if all fil
+000019f0: 6573 206f 7574 7075 7420 6279 2046 4153  es output by FAS
+00001a00: 5420 6172 6520 706c 6163 6564 2069 6e20  T are placed in 
+00001a10: 7468 6973 2064 6972 6563 746f 7279 2c20  this directory, 
+00001a20: 7468 656e 2066 5241 5420 7769 6c6c 2066  then fRAT will f
+00001a30: 696e 6420 7468 6520 6e65 6365 7373 6172  ind the necessar
+00001a40: 7920 6669 6c65 2eda 0c72 756e 5f66 736c  y file...run_fsl
+00001a50: 5f66 6173 747a 1652 756e 2069 6620 6669  _fastz.Run if fi
+00001a60: 6c65 7320 6e6f 7420 666f 756e 647a 094e  les not foundz.N
+00001a70: 6576 6572 2072 756e 7a8e 5265 636f 6d6d  ever runz.Recomm
+00001a80: 656e 6465 643a 2022 5275 6e20 6966 2066  ended: "Run if f
+00001a90: 696c 6573 206e 6f74 2066 6f75 6e64 222e  iles not found".
+00001aa0: 0a54 6865 7365 2066 696c 6573 2077 696c  .These files wil
+00001ab0: 6c20 6f6e 6c79 2062 6520 7365 6172 6368  l only be search
+00001ac0: 6564 2066 6f72 2028 616e 6420 7468 7573  ed for (and thus
+00001ad0: 2063 7265 6174 6564 2920 6966 2022 5573   created) if "Us
+00001ae0: 6520 4653 4c20 4641 5354 2073 6567 6d65  e FSL FAST segme
+00001af0: 6e74 6174 696f 6e22 2069 7320 7365 7420  ntation" is set 
+00001b00: 746f 2074 7275 652e 7a0c 5275 6e20 4653  to true.z.Run FS
+00001b10: 4c20 4641 5354 2906 720b 0000 0072 2000  L FAST).r....r .
+00001b20: 0000 720c 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00001b30: 0072 2100 0000 da10 6673 6c66 6173 745f  .r!.....fslfast_
+00001b40: 6d69 6e5f 7072 6f62 da05 5363 616c 6567  min_prob..Scaleg
+00001b50: 9a99 9999 9999 b93f e900 0000 0072 1e00  .......?.....r..
+00001b60: 0000 679a 9999 9999 99a9 3f7a 1c46 534c  ..g.......?z.FSL
+00001b70: 2046 4153 5420 6d69 6e69 6d75 6d20 7072   FAST minimum pr
+00001b80: 6f62 6162 696c 6974 797a 1052 6563 6f6d  obabilityz.Recom
+00001b90: 6d65 6e64 6564 3a20 302e 3129 0772 0b00  mended: 0.1).r..
+00001ba0: 0000 720c 0000 00da 0446 726f 6dda 0254  ..r......From..T
+00001bb0: 6fda 0a52 6573 6f6c 7574 696f 6e72 0f00  o..Resolutionr..
+00001bc0: 0000 720e 0000 00da 0f73 7461 745f 6d61  ..r......stat_ma
+00001bd0: 705f 666f 6c64 6572 7a16 5374 6174 6973  p_folderz.Statis
+00001be0: 7469 6361 6c20 6d61 7020 666f 6c64 6572  tical map folder
+00001bf0: 7a51 466f 6c64 6572 206e 616d 6520 7768  zQFolder name wh
+00001c00: 6963 6820 636f 6e74 6169 6e73 2074 6865  ich contains the
+00001c10: 2073 7461 7469 7374 6963 616c 206d 6170   statistical map
+00001c20: 2066 696c 6573 2e20 4578 616d 706c 653a   files. Example:
+00001c30: 2074 656d 706f 7261 6c53 4e52 5f72 6570   temporalSNR_rep
+00001c40: 6f72 7429 0672 0b00 0000 720c 0000 0072  ort).r....r....r
+00001c50: 2100 0000 720d 0000 0072 0f00 0000 720e  !...r....r....r.
+00001c60: 0000 00da 0f73 7461 745f 6d61 705f 7375  .....stat_map_su
+00001c70: 6666 6978 7a0c 5f74 534e 522e 6e69 692e  ffixz._tSNR.nii.
+00001c80: 677a 7a16 5374 6174 6973 7469 6361 6c20  gzz.Statistical 
+00001c90: 6d61 7020 7375 6666 6978 7a5d 4669 6c65  map suffixz]File
+00001ca0: 206e 616d 6520 7375 6666 6978 206f 6620   name suffix of 
+00001cb0: 7468 6520 7374 6174 6973 7469 6361 6c20  the statistical 
+00001cc0: 6d61 7020 6669 6c65 732e 2049 6e63 6c75  map files. Inclu
+00001cd0: 6465 2074 6865 2066 696c 6520 6578 7465  de the file exte
+00001ce0: 6e73 696f 6e2e 2045 7861 6d70 6c65 3a20  nsion. Example: 
+00001cf0: 5f74 534e 522e 696d 67da 1163 6f6e 665f  _tSNR.img..conf_
+00001d00: 6c65 7665 6c5f 6e75 6d62 6572 fa09 3935  level_number..95
+00001d10: 252c 2031 2e39 3629 067a 0938 3025 2c20  %, 1.96).z.80%, 
+00001d20: 312e 3238 7a09 3835 252c 2031 2e34 347a  1.28z.85%, 1.44z
+00001d30: 0939 3025 2c20 312e 3634 724d 0000 007a  .90%, 1.64rM...z
+00001d40: 0939 3825 2c20 322e 3333 7a09 3939 252c  .98%, 2.33z.99%,
+00001d50: 2032 2e35 387a 1043 6f6e 6669 6465 6e63   2.58z.Confidenc
+00001d60: 6520 6c65 7665 6c7a a553 6574 2074 6865  e levelz.Set the
+00001d70: 2063 6f6e 6669 6465 6e63 6520 6c65 7665   confidence leve
+00001d80: 6c20 666f 7220 636f 6e66 6964 656e 6365  l for confidence
+00001d90: 2069 6e74 6572 7661 6c20 6361 6c63 756c   interval calcul
+00001da0: 6174 696f 6e73 2e0a 4e75 6d62 6572 7320  ations..Numbers 
+00001db0: 7265 7072 6573 656e 7420 7468 6520 636f  represent the co
+00001dc0: 6e66 6964 656e 6365 206c 6576 656c 2061  nfidence level a
+00001dd0: 6e64 2074 6865 2063 6f72 7265 7370 6f6e  nd the correspon
+00001de0: 6469 6e67 2063 7269 7469 6361 6c20 7a20  ding critical z 
+00001df0: 7661 6c75 652e 0a52 6563 6f6d 6d65 6e64  value..Recommend
+00001e00: 6564 3a20 3935 252c 2031 2e39 362e 2906  ed: 95%, 1.96.).
+00001e10: 720b 0000 0072 0c00 0000 7220 0000 0072  r....r....r ...r
+00001e20: 2100 0000 720f 0000 0072 0e00 0000 da0d  !...r....r......
+00001e30: 6269 6e61 7279 5f70 6172 616d 73da 0744  binary_params..D
+00001e40: 796e 616d 6963 7a1a 5061 7273 696e 675b  ynamicz.Parsing[
+00001e50: 2270 6172 616d 6574 6572 5f64 6963 7431  "parameter_dict1
+00001e60: 225d da0b 4368 6563 6b62 7574 746f 6e7a  "]..Checkbuttonz
+00001e70: 1142 696e 6172 7920 7061 7261 6d65 7465  .Binary paramete
+00001e80: 7273 da04 6c69 7374 7a33 4164 6420 7061  rs..listz3Add pa
+00001e90: 7261 6d65 7465 7273 2068 6572 6520 7768  rameters here wh
+00001ea0: 6963 6820 7769 6c6c 2065 6974 6865 7220  ich will either 
+00001eb0: 6265 206f 6e20 6f72 206f 6666 2e29 0772  be on or off.).r
+00001ec0: 0b00 0000 720c 0000 0072 2000 0000 da07  ....r....r .....
+00001ed0: 7375 6274 7970 6572 0f00 0000 7221 0000  subtyper....r!..
+00001ee0: 0072 0e00 0000 7a11 4f75 746c 6965 7220  .r....z.Outlier 
+00001ef0: 6465 7465 6374 696f 6eda 0c6e 6f69 7365  detection..noise
+00001f00: 5f63 7574 6f66 6661 8001 0000 7472 7565  _cutoffa....true
+00001f10: 206f 7220 6661 6c73 652e 2043 616c 6375   or false. Calcu
+00001f20: 6c61 7465 2061 206d 696e 696d 756d 2063  late a minimum c
+00001f30: 7574 6f66 6620 7661 6c75 6520 746f 2062  utoff value to b
+00001f40: 6520 696e 636c 7564 6564 2069 6e20 616e  e included in an
+00001f50: 2052 4f49 2c62 6173 6564 206f 6e20 766f   ROI,based on vo
+00001f60: 7865 6c73 206e 6f74 2061 7373 6967 6e65  xels not assigne
+00001f70: 6420 616e 2052 4f49 206f 7220 7468 6174  d an ROI or that
+00001f80: 2068 6176 6520 6265 656e 2065 7863 6c75   have been exclu
+00001f90: 6465 6420 6672 6f6d 2061 6e61 6c79 7369  ded from analysi
+00001fa0: 732e 2056 6f78 656c 7320 7769 7468 2076  s. Voxels with v
+00001fb0: 616c 7565 7320 6f66 2030 2061 7265 206e  alues of 0 are n
+00001fc0: 6f74 2069 6e63 6c75 6465 6420 7768 656e  ot included when
+00001fd0: 2063 616c 6375 6c61 7469 6e67 2074 6865   calculating the
+00001fe0: 206e 6f69 7365 2063 7574 6f66 662e 200a   noise cutoff. .
+00001ff0: 5573 6566 756c 2066 6f72 2073 7461 7469  Useful for stati
+00002000: 7374 6963 616c 206d 6170 7320 7768 6572  stical maps wher
+00002010: 6520 6578 7472 6163 7261 6e69 616c 2076  e extracranial v
+00002020: 6f78 656c 7320 6172 6520 6c69 6b65 6c79  oxels are likely
+00002030: 2074 6f20 6861 7665 206d 7563 6820 6c6f   to have much lo
+00002040: 7765 7220 7661 6c75 6573 2074 6861 6e20  wer values than 
+00002050: 7468 6f73 6520 696e 7369 6465 2074 6865  those inside the
+00002060: 2062 7261 696e 2073 7563 6820 6173 2074   brain such as t
+00002070: 534e 5220 6d61 7073 2e20 5265 636f 6d6d  SNR maps. Recomm
+00002080: 656e 6465 643a 2074 7275 652e da1a 6761  ended: true...ga
+00002090: 7573 7369 616e 5f6f 7574 6c69 6572 5f64  ussian_outlier_d
+000020a0: 6574 6563 7469 6f6e 7a21 4761 7573 7369  etectionz!Gaussi
+000020b0: 616e 206f 7574 6c69 6572 2028 4761 754f  an outlier (GauO
+000020c0: 2920 6465 7465 6374 696f 6e7a 6b74 7275  ) detectionzktru
+000020d0: 6520 6f72 2066 616c 7365 2e20 4669 7420  e or false. Fit 
+000020e0: 6120 6761 7573 7369 616e 2074 6f20 7468  a gaussian to th
+000020f0: 6520 6461 7461 2074 6f20 6465 7465 726d  e data to determ
+00002100: 696e 6520 6f75 746c 6965 7273 2075 7369  ine outliers usi
+00002110: 6e67 2045 6c6c 6970 7469 6320 456e 7665  ng Elliptic Enve
+00002120: 6c6f 7065 2e20 5265 636f 6d6d 656e 6465  lope. Recommende
+00002130: 643a 2074 7275 652e da1e 6761 7573 7369  d: true...gaussi
+00002140: 616e 5f6f 7574 6c69 6572 5f63 6f6e 7461  an_outlier_conta
+00002150: 6d69 6e61 7469 6f6e 677b 14ae 47e1 7a84  minationg{..G.z.
+00002160: 3f7a 1d47 6175 4f20 636f 6e74 616d 696e  ?z.GauO contamin
+00002170: 6174 696f 6e20 7065 7263 656e 7461 6765  ation percentage
+00002180: 7a38 5065 7263 656e 7420 6f66 2065 7870  z8Percent of exp
+00002190: 6563 7465 6420 6f75 746c 6965 7273 2069  ected outliers i
+000021a0: 6e20 6461 7461 7365 740a 5265 636f 6d6d  n dataset.Recomm
+000021b0: 656e 6465 643a 2030 2e31 da19 6761 7573  ended: 0.1..gaus
+000021c0: 7369 616e 5f6f 7574 6c69 6572 5f6c 6f63  sian_outlier_loc
+000021d0: 6174 696f 6efa 0e62 656c 6f77 2067 6175  ation..below gau
+000021e0: 7373 6961 6e29 0372 5700 0000 7a0e 6162  ssian).rW...z.ab
+000021f0: 6f76 6520 6761 7573 7369 616e da04 626f  ove gaussian..bo
+00002200: 7468 7a0d 4761 754f 206c 6f63 6174 696f  thz.GauO locatio
+00002210: 6e7a a444 6174 6120 746f 2072 656d 6f76  nz.Data to remov
+00002220: 6520 2869 6620 6761 7573 7369 616e 206f  e (if gaussian o
+00002230: 7574 6c69 6572 2064 6574 6563 7469 6f6e  utlier detection
+00002240: 2069 7320 7472 7565 292e 0a46 6f72 2065   is true)..For e
+00002250: 7861 6d70 6c65 3a20 6966 2073 6574 2074  xample: if set t
+00002260: 6f20 6265 6c6f 7720 6761 7573 7369 616e  o below gaussian
+00002270: 2c20 6461 7461 2062 656c 6f77 2074 6865  , data below the
+00002280: 2067 6175 7373 6961 6e20 7769 6c6c 2062   gaussian will b
+00002290: 6520 7265 6d6f 7665 642e 0a52 6563 6f6d  e removed..Recom
+000022a0: 6d65 6e64 6564 3a20 6265 6c6f 7720 6761  mended: below ga
+000022b0: 7573 7369 616e 2e5a 1e63 7265 6174 655f  ussian.Z.create_
+000022c0: 7374 6174 6973 7469 6373 5f6f 7074 696f  statistics_optio
+000022d0: 6e73 5f66 696c 65da 1663 7265 6174 655f  ns_file..create_
+000022e0: 7374 6174 6973 7469 6373 5f66 696c 657a  statistics_filez
+000022f0: 1c43 7265 6174 6520 7374 6174 6973 7469  .Create statisti
+00002300: 6373 4f70 7469 6f6e 732e 6373 767a 9743  csOptions.csvz.C
+00002310: 7265 6174 6520 6669 6c65 2069 6e20 6261  reate file in ba
+00002320: 7365 2066 6f6c 6465 7220 746f 2063 686f  se folder to cho
+00002330: 6f73 6520 7374 6174 6973 7469 6373 206f  ose statistics o
+00002340: 7074 696f 6e73 2e20 5375 6368 2061 7320  ptions. Such as 
+00002350: 7768 6963 6820 7061 7261 6d65 7465 7273  which parameters
+00002360: 2074 6f20 6578 636c 7564 6520 6672 6f6d   to exclude from
+00002370: 2061 6e61 6c79 7369 7320 616e 6420 7768   analysis and wh
+00002380: 6174 206d 6169 6e20 6566 6665 6374 2063  at main effect c
+00002390: 6f6e 7472 6173 7473 2074 6f20 6361 6c63  ontrasts to calc
+000023a0: 756c 6174 652e 2905 720b 0000 0072 2e00  ulate.).r....r..
+000023b0: 0000 7230 0000 0072 2f00 0000 720e 0000  ..r0...r/...r...
+000023c0: 00da 2c61 7574 6f6d 6174 6963 616c 6c79  ..,automatically
+000023d0: 5f63 7265 6174 655f 7374 6174 6973 7469  _create_statisti
+000023e0: 6373 5f6f 7074 696f 6e73 5f66 696c 6561  cs_options_filea
+000023f0: 0301 0000 7472 7565 206f 7220 6661 6c73  ....true or fals
+00002400: 652e 0a55 7375 616c 6c79 2073 7461 7469  e..Usually stati
+00002410: 7374 6963 734f 7074 696f 6e73 2e63 7376  sticsOptions.csv
+00002420: 2069 7320 6175 746f 6d61 7469 6361 6c6c   is automaticall
+00002430: 7920 6372 6561 7465 6420 7768 656e 2063  y created when c
+00002440: 7265 6174 696e 6720 7061 7261 6d56 616c  reating paramVal
+00002450: 7565 732e 6373 762e 2044 6573 656c 6563  ues.csv. Deselec
+00002460: 7420 7468 6973 206f 7074 696f 6e20 6966  t this option if
+00002470: 2079 6f75 2077 6f6e 2774 2062 6520 7275   you won't be ru
+00002480: 6e6e 696e 6720 7468 6520 7374 6174 6973  nning the statis
+00002490: 7469 6373 2073 7465 702e 2054 6865 2063  tics step. The c
+000024a0: 7265 6174 6520 7374 6174 6973 7469 6373  reate statistics
+000024b0: 4f70 7469 6f6e 732e 6373 7620 6275 7474  Options.csv butt
+000024c0: 6f6e 2061 626f 7665 2063 616e 2061 6c73  on above can als
+000024d0: 6f20 6265 2075 7365 6420 746f 206d 616e  o be used to man
+000024e0: 7561 6c6c 7920 6372 6561 7465 2074 6869  ually create thi
+000024f0: 7320 6669 6c65 2e5a 1973 7461 7469 7374  s file.Z.statist
+00002500: 6963 735f 7375 6266 6f6c 6465 725f 6e61  ics_subfolder_na
+00002510: 6d65 da05 7374 6174 737a 2544 6972 6563  me..statsz%Direc
+00002520: 746f 7279 206e 616d 6520 666f 7220 7374  tory name for st
+00002530: 6174 6973 7469 6373 2066 6f6c 6465 722e  atistics folder.
+00002540: 5a0c 7072 696e 745f 7265 7375 6c74 7a19  Z.print_resultz.
+00002550: 5072 696e 7420 7265 7375 6c74 7320 746f  Print results to
+00002560: 2074 6572 6d69 6e61 6c7a 5874 7275 6520   terminalzXtrue 
+00002570: 6f72 2066 616c 7365 2e20 5072 696e 7473  or false. Prints
+00002580: 2072 6573 756c 7473 2074 6f20 7465 726d   results to term
+00002590: 696e 616c 2069 6620 7472 7565 2069 6e20  inal if true in 
+000025a0: 6164 6469 7469 6f6e 2074 6f20 7361 7669  addition to savi
+000025b0: 6e67 2072 6573 756c 7473 2074 6f20 6669  ng results to fi
+000025c0: 6c65 2e5a 0e6d 696e 696d 756d 5f76 6f78  le.Z.minimum_vox
+000025d0: 656c 7369 9001 0000 6194 0100 0046 6f72  elsi....a....For
+000025e0: 2062 6f6f 7473 7472 6170 7065 6420 6368   bootstrapped ch
+000025f0: 616e 6765 2076 6572 7375 7320 6261 7365  ange versus base
+00002600: 6c69 6e65 2c20 666f 7220 6561 6368 2052  line, for each R
+00002610: 4f49 2c20 7468 6520 6176 6572 6167 6520  OI, the average 
+00002620: 6e75 6d62 6572 206f 6620 766f 7865 6c73  number of voxels
+00002630: 2070 6572 2073 6573 7369 6f6e 2066 6f72   per session for
+00002640: 2061 6e20 524f 4920 6d75 7374 2062 6520   an ROI must be 
+00002650: 6162 6f76 6520 7468 6973 2076 616c 7565  above this value
+00002660: 2074 6f20 6265 2069 6e63 6c75 6465 6420   to be included 
+00002670: 696e 2074 6865 2061 6e61 6c79 7369 732e  in the analysis.
+00002680: 466f 7220 7275 6e6e 696e 6720 7468 6520  For running the 
+00002690: 6c69 6e65 6172 206d 6978 6564 206d 6f64  linear mixed mod
+000026a0: 656c 2c20 666f 7220 6561 6368 2052 4f49  el, for each ROI
+000026b0: 2c20 616e 7920 7365 7373 696f 6e73 2077  , any sessions w
+000026c0: 6974 6820 6120 766f 7865 6c20 636f 756e  ith a voxel coun
+000026d0: 7420 6265 6c6f 7720 7468 6973 2076 616c  t below this val
+000026e0: 7565 2077 696c 6c20 6265 2072 656d 6f76  ue will be remov
+000026f0: 6564 2e0a 4869 6768 6c79 2072 6563 6f6d  ed..Highly recom
+00002700: 6d65 6e64 6564 2074 6f20 7365 7420 6120  mended to set a 
+00002710: 7661 6c75 6520 6865 7265 2c20 6173 2052  value here, as R
+00002720: 4f49 7320 7769 7468 2061 2073 6d61 6c6c  OIs with a small
+00002730: 206e 756d 6265 7220 6f66 2076 6f78 656c   number of voxel
+00002740: 7320 6d61 7920 7375 6767 6573 7420 706f  s may suggest po
+00002750: 6f72 2066 6974 7469 6e67 2e0a 5265 636f  or fitting..Reco
+00002760: 6d6d 656e 6465 6420 7661 6c75 6520 3430  mmended value 40
+00002770: 305a 1162 6f6f 7473 7472 6170 5f73 616d  0Z.bootstrap_sam
+00002780: 706c 6573 69e8 0300 007a 6952 6563 6f6d  plesi....ziRecom
+00002790: 6d65 6e64 6564 2076 616c 7565 2031 3030  mended value 100
+000027a0: 302e 200a 4e6f 7465 3a20 426f 6f74 7374  0. .Note: Bootst
+000027b0: 7261 7070 696e 6720 6973 206f 6e6c 7920  rapping is only 
+000027c0: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+000027d0: 6520 7065 7263 656e 7461 6765 2063 6861  e percentage cha
+000027e0: 6e67 6520 7665 7273 7573 2062 6173 656c  nge versus basel
+000027f0: 696e 652e 5a1d 626f 6f74 7374 7261 705f  ine.Z.bootstrap_
+00002800: 636f 6e66 6964 656e 6365 5f69 6e74 6572  confidence_inter
+00002810: 7661 6ce9 5f00 0000 7a67 5265 636f 6d6d  val._...zgRecomm
+00002820: 656e 6465 6420 7661 6c75 653a 2039 3520  ended value: 95 
+00002830: 0a4e 6f74 653a 2042 6f6f 7473 7472 6170  .Note: Bootstrap
+00002840: 7069 6e67 2069 7320 6f6e 6c79 2075 7365  ping is only use
+00002850: 6420 746f 2063 616c 6375 6c61 7465 2070  d to calculate p
+00002860: 6572 6365 6e74 6167 6520 6368 616e 6765  ercentage change
+00002870: 2076 6572 7375 7320 6261 7365 6c69 6e65   versus baseline
+00002880: 2e5a 1372 6567 696f 6e61 6c5f 7374 6174  .Z.regional_stat
+00002890: 735f 726f 6973 da03 616c 6c7a 2052 4f49  s_rois..allz ROI
+000028a0: 7320 746f 2063 616c 6375 6c61 7465 2073  s to calculate s
+000028b0: 7461 7469 7374 6963 7320 666f 727a 8c50  tatistics forz.P
+000028c0: 726f 7669 6465 2061 2063 6f6d 6d61 2d73  rovide a comma-s
+000028d0: 6570 6172 6174 6564 206c 6973 7420 6f66  eparated list of
+000028e0: 2072 6567 696f 6e73 2c20 652e 672e 2027   regions, e.g. '
+000028f0: 332c 2035 272c 2074 6865 2073 7472 696e  3, 5', the strin
+00002900: 6720 2761 6c6c 2720 666f 7220 616c 6c20  g 'all' for all 
+00002910: 726f 6973 206f 7220 7468 6520 7374 7269  rois or the stri
+00002920: 6e67 2027 5275 6e74 696d 6527 2074 6f20  ng 'Runtime' to 
+00002930: 7072 6f76 6964 6520 7265 6769 6f6e 7320  provide regions 
+00002940: 6174 2072 756e 7469 6d65 2eda 1369 6e63  at runtime...inc
+00002950: 6c75 6465 5f61 735f 7661 7269 6162 6c65  lude_as_variable
+00002960: 7a15 494e 434c 5544 4520 414c 4c20 5641  z.INCLUDE ALL VA
+00002970: 5249 4142 4c45 537a e953 656c 6563 7420  RIABLESz.Select 
+00002980: 7768 6963 6820 7661 7269 6162 6c65 7320  which variables 
+00002990: 746f 2069 6e63 6c75 6465 2069 6e20 7374  to include in st
+000029a0: 6174 6973 7469 6361 6c20 616e 616c 7973  atistical analys
+000029b0: 6973 2e0a 5573 6564 2074 6f20 6465 7465  is..Used to dete
+000029c0: 726d 696e 6520 7768 6963 6820 7661 7269  rmine which vari
+000029d0: 6162 6c65 7320 746f 2075 7365 2061 7320  ables to use as 
+000029e0: 6669 7865 6420 6566 6665 6374 7320 696e  fixed effects in
+000029f0: 206c 696e 6561 7220 6d69 7865 6420 6d6f   linear mixed mo
+00002a00: 6465 6c73 2061 6e64 2077 6869 6368 2076  dels and which v
+00002a10: 6172 6961 626c 6573 2074 6f20 7461 6b65  ariables to take
+00002a20: 2069 6e74 6f20 6163 636f 756e 7420 7768   into account wh
+00002a30: 656e 2062 616c 616e 6369 6e67 2064 6174  en balancing dat
+00002a40: 6120 666f 7220 7468 6520 6d61 696e 2065  a for the main e
+00002a50: 6666 6563 7420 7420 7465 7374 2064 6174  ffect t test dat
+00002a60: 612e 2907 720b 0000 0072 0c00 0000 720d  a.).r....r....r.
+00002a70: 0000 0072 2000 0000 7252 0000 0072 2100  ...r ...rR...r!.
+00002a80: 0000 720e 0000 005a 1262 7261 696e 5f6d  ..r....Z.brain_m
+00002a90: 6170 5f70 5f74 6872 6573 687a 1b43 6f65  ap_p_threshz.Coe
+00002aa0: 6666 6963 6965 6e74 206d 6170 2070 2d74  fficient map p-t
+00002ab0: 6872 6573 686f 6c64 7aba 502d 7661 6c75  hresholdz.P-valu
+00002ac0: 6520 7468 7265 7368 6f6c 6420 746f 2075  e threshold to u
+00002ad0: 7365 2077 6865 6e20 6372 6561 7469 6e67  se when creating
+00002ae0: 2062 7261 696e 2063 6f65 6666 6963 6965   brain coefficie
+00002af0: 6e74 206d 6170 732e 2041 6e79 2066 6978  nt maps. Any fix
+00002b00: 6564 2065 6666 6563 7420 7468 6174 2064  ed effect that d
+00002b10: 6f65 736e 2774 2068 6176 6520 6120 702d  oesn't have a p-
+00002b20: 7661 6c75 6520 6571 7561 6c20 746f 206f  value equal to o
+00002b30: 7220 6c65 7373 2074 6861 6e20 7468 6973  r less than this
+00002b40: 2076 616c 7565 2077 696c 6c20 6e6f 7420   value will not 
+00002b50: 6265 2069 6e63 6c75 6465 6420 696e 2074  be included in t
+00002b60: 6865 2063 6f65 6666 6963 6965 6e74 206d  he coefficient m
+00002b70: 6170 2e0a 2905 720b 0000 0072 0c00 0000  ap..).r....r....
+00002b80: 720f 0000 0072 0e00 0000 720d 0000 007a  r....r....r....z
+00002b90: 0754 2d74 6573 7473 5a0b 7275 6e5f 745f  .T-testsZ.run_t_
+00002ba0: 7465 7374 737a 0f74 7275 6520 6f72 2066  testsz.true or f
+00002bb0: 616c 7365 2e0a 2904 720b 0000 0072 0d00  alse..).r....r..
+00002bc0: 0000 720c 0000 0072 0e00 0000 da07 4956  ..r....r......IV
+00002bd0: 5f74 7970 657a 2046 494c 4c20 4956 2054  _typez FILL IV T
+00002be0: 5950 4520 4153 2042 4554 5745 454e 2d53  YPE AS BETWEEN-S
+00002bf0: 5542 4a45 4354 53da 0b4f 7074 696f 6e4d  UBJECTS..OptionM
+00002c00: 656e 7532 7a0f 5769 7468 696e 2d73 7562  enu2z.Within-sub
+00002c10: 6a65 6374 737a 1042 6574 7765 656e 2d73  jectsz.Between-s
+00002c20: 7562 6a65 6374 737a 0749 5620 7479 7065  ubjectsz.IV type
+00002c30: 7a58 5479 7065 206f 6620 7661 7269 6162  zXType of variab
+00002c40: 6c65 2063 6f6c 6c65 6374 6564 2e20 5573  le collected. Us
+00002c50: 6564 2074 6f20 6368 6f6f 7365 2077 6869  ed to choose whi
+00002c60: 6368 2074 2d74 6573 7420 746f 2075 7365  ch t-test to use
+00002c70: 2066 6f72 2070 6169 7277 6973 6520 636f   for pairwise co
+00002c80: 6d70 6172 6973 6f6e 732e 290a 720b 0000  mparisons.).r...
+00002c90: 0072 0c00 0000 7220 0000 0072 5200 0000  .r....r ...rR...
+00002ca0: 7221 0000 00da 084f 7074 696f 6e73 3272  r!.....Options2r
+00002cb0: 0f00 0000 720d 0000 00da 0d44 6566 6175  ....r......Defau
+00002cc0: 6c74 4e75 6d62 6572 720e 0000 007a 134c  ltNumberr....z.L
+00002cd0: 696e 6561 7220 6d69 7865 6420 6d6f 6465  inear mixed mode
+00002ce0: 6c73 5a17 7275 6e5f 6c69 6e65 6172 5f6d  lsZ.run_linear_m
+00002cf0: 6978 6564 5f6d 6f64 656c 735a 1563 6174  ixed_modelsZ.cat
+00002d00: 6567 6f72 6963 616c 5f76 6172 6961 626c  egorical_variabl
+00002d10: 6573 7a42 5365 6c65 6374 2077 6869 6368  eszBSelect which
+00002d20: 2076 6172 6961 626c 6573 2028 6966 2061   variables (if a
+00002d30: 6e79 2920 6172 6520 6361 7465 676f 7269  ny) are categori
+00002d40: 6361 6c2e 2055 7365 6420 666f 7220 7468  cal. Used for th
+00002d50: 6520 4c4d 4d2e 2906 720b 0000 0072 0c00  e LMM.).r....r..
+00002d60: 0000 7220 0000 0072 5200 0000 7221 0000  ..r ...rR...r!..
+00002d70: 0072 0e00 0000 5a0c 6d61 696e 5f65 6666  .r....Z.main_eff
+00002d80: 6563 7473 7a14 436f 6d70 7574 6520 6d61  ectsz.Compute ma
+00002d90: 696e 2065 6666 6563 7473 7a53 7472 7565  in effectszStrue
+00002da0: 206f 7220 6661 6c73 652e 0a4e 6f74 653a   or false..Note:
+00002db0: 2054 6869 7320 6f70 7469 6f6e 2069 7320   This option is 
+00002dc0: 696e 6465 7065 6e64 656e 7420 6672 6f6d  independent from
+00002dd0: 2074 6865 206f 7468 6572 2065 6666 6563   the other effec
+00002de0: 7420 6361 6c63 756c 6174 696f 6e73 2e7a  t calculations.z
+00002df0: 2443 6f6d 7075 7465 206d 6169 6e20 616e  $Compute main an
+00002e00: 6420 696e 7465 7261 6374 696f 6e20 6566  d interaction ef
+00002e10: 6665 6374 737a 1b43 6f6d 7075 7465 2069  fectsz.Compute i
+00002e20: 6e74 6572 6163 7469 6f6e 2065 6666 6563  nteraction effec
+00002e30: 7473 7a28 4d61 7869 6d75 6d20 7065 7263  tsz(Maximum perc
+00002e40: 656e 7420 6f66 2073 6573 7369 6f6e 7320  ent of sessions 
+00002e50: 6265 6c6f 7720 7468 7265 7368 6149 0100  below threshaI..
+00002e60: 0052 6563 6f6d 6d65 6e64 6564 2076 616c  .Recommended val
+00002e70: 7565 2030 2e20 0a46 6f72 2061 2067 6976  ue 0. .For a giv
+00002e80: 656e 2052 4f49 2c20 7468 6973 2076 616c  en ROI, this val
+00002e90: 7565 2073 6574 7320 7468 6520 6d61 7869  ue sets the maxi
+00002ea0: 6d75 6d20 7065 7263 656e 7420 6f66 2073  mum percent of s
+00002eb0: 6573 7369 6f6e 7320 7468 6174 2063 616e  essions that can
+00002ec0: 2062 6520 6578 636c 7564 6564 2028 6475   be excluded (du
+00002ed0: 6520 746f 2068 6176 696e 6720 696e 7375  e to having insu
+00002ee0: 6666 6963 6965 6e74 2076 6f78 656c 2063  fficient voxel c
+00002ef0: 6f75 6e74 2920 6265 666f 7265 2074 6865  ount) before the
+00002f00: 2052 4f49 2069 7320 6e6f 7420 696e 636c   ROI is not incl
+00002f10: 7564 6564 2069 6e20 7232 2076 7320 766f  uded in r2 vs vo
+00002f20: 7865 6c20 636f 756e 7420 7374 6174 6973  xel count statis
+00002f30: 7469 6373 2e0a 5769 7468 2074 6865 2064  tics..With the d
+00002f40: 6566 6175 6c74 2076 616c 7565 206f 6620  efault value of 
+00002f50: 3130 3028 2529 2061 6e20 524f 4920 7769  100(%) an ROI wi
+00002f60: 6c6c 206e 6f74 2062 6520 696e 636c 7564  ll not be includ
+00002f70: 6564 2069 6e20 7468 6973 2063 616c 6375  ed in this calcu
+00002f80: 6c61 7469 6f6e 2069 6620 616e 7920 7365  lation if any se
+00002f90: 7373 696f 6e73 2068 6176 6520 6265 656e  ssions have been
+00002fa0: 2065 7863 6c75 6465 642e 2904 5a1c 6d61   excluded.).Z.ma
+00002fb0: 696e 5f61 6e64 5f69 6e74 6572 6163 7469  in_and_interacti
+00002fc0: 6f6e 5f65 6666 6563 7473 5a13 696e 7465  on_effectsZ.inte
+00002fd0: 7261 6374 696f 6e5f 6566 6665 6374 737a  raction_effectsz
+00002fe0: 1552 3220 7673 2076 6f78 656c 2063 6f75  .R2 vs voxel cou
+00002ff0: 6e74 204c 4d4d 5a10 6d61 785f 6265 6c6f  nt LMMZ.max_belo
+00003000: 775f 7468 7265 7368 7a09 4d42 2c20 5345  w_threshz.MB, SE
+00003010: 4e53 457a 1343 7269 7469 6361 6c20 7061  NSEz.Critical pa
+00003020: 7261 6d65 7465 7273 615d 0200 0043 6f6d  rametersa]...Com
+00003030: 6d61 2d73 6570 6172 6174 6564 206c 6973  ma-separated lis
+00003040: 7420 6f66 2069 6e64 6570 656e 6465 6e74  t of independent
+00003050: 2076 6172 6961 626c 6573 2e0a 5468 6520   variables..The 
+00003060: 6372 6974 6963 616c 2070 6172 616d 6574  critical paramet
+00003070: 6572 2073 6574 7469 6e67 7320 6172 6520  er settings are 
+00003080: 7573 6564 2074 6f20 7375 7070 6c79 2074  used to supply t
+00003090: 6865 206e 616d 6573 2061 6e64 2066 696c  he names and fil
+000030a0: 6520 6e61 6d65 2061 6262 7265 7669 6174  e name abbreviat
+000030b0: 696f 6e73 206f 6620 7468 6520 696e 6465  ions of the inde
+000030c0: 7065 6e64 656e 7420 7661 7269 6162 6c65  pendent variable
+000030d0: 732c 2074 6865 7265 666f 7265 2060 6652  s, therefore `fR
+000030e0: 4154 6020 7375 7070 6f72 7473 2074 6865  AT` supports the
+000030f0: 2075 7365 206f 6620 616e 7920 7061 7261   use of any para
+00003100: 6d65 7465 7273 2028 616e 6420 616e 7920  meters (and any 
+00003110: 6e75 6d62 6572 206f 6620 7468 656d 292e  number of them).
+00003120: 0a41 7320 7468 6573 6520 6372 6974 6963  .As these critic
+00003130: 616c 2070 6172 616d 6574 6572 7320 7769  al parameters wi
+00003140: 6c6c 2061 6c73 6f20 6265 2075 7365 6420  ll also be used 
+00003150: 7768 656e 206c 6162 656c 6c69 6e67 2074  when labelling t
+00003160: 6865 2072 6f77 7320 616e 6420 636f 6c75  he rows and colu
+00003170: 6d6e 7320 6f66 2062 6f74 6820 7468 6520  mns of both the 
+00003180: 7669 6f6c 696e 2070 6c6f 7473 2061 6e64  violin plots and
+00003190: 2068 6973 746f 6772 616d 732c 2074 6865   histograms, the
+000031a0: 7920 7368 6f75 6c64 2062 6520 7772 6974  y should be writ
+000031b0: 7465 6e20 6173 2079 6f75 2077 616e 7420  ten as you want 
+000031c0: 7468 656d 2074 6f20 6170 7065 6172 2069  them to appear i
+000031d0: 6e20 7468 6573 6520 6669 6775 7265 732e  n these figures.
+000031e0: 0a4e 6f74 653a 204c 6561 7665 2062 6c61  .Note: Leave bla
+000031f0: 6e6b 2069 6620 796f 7520 646f 206e 6f74  nk if you do not
+00003200: 2077 616e 7420 746f 2063 6f6d 7061 7265   want to compare
+00003210: 2062 6574 7765 656e 2064 6966 6665 7265   between differe
+00003220: 6e74 2063 6f6e 6469 7469 6f6e 732c 2066  nt conditions, f
+00003230: 6f72 2065 7861 6d70 6c65 2c20 6966 2079  or example, if y
+00003240: 6f75 2077 6973 6820 746f 2073 6565 2074  ou wish to see t
+00003250: 6865 206f 7665 7261 6c6c 2074 534e 5220  he overall tSNR 
+00003260: 666f 7220 6561 6368 2072 6567 696f 6e20  for each region 
+00003270: 6163 726f 7373 2074 6865 2065 6e74 6972  across the entir
+00003280: 6520 6461 7461 7365 742e 2906 720b 0000  e dataset.).r...
+00003290: 0072 0d00 0000 720c 0000 0072 2100 0000  .r....r....r!...
+000032a0: 720f 0000 0072 0e00 0000 7a05 6d62 2c20  r....r....z.mb, 
+000032b0: 737a 1f43 7269 7469 6361 6c20 7061 7261  sz.Critical para
+000032c0: 6d65 7465 7220 6162 6272 6576 6961 7469  meter abbreviati
+000032d0: 6f6e 6150 0100 0043 6f6d 6d61 2d73 6570  onaP...Comma-sep
+000032e0: 6172 6174 6564 206c 6973 7420 6f66 2074  arated list of t
+000032f0: 6572 6d73 2074 6f20 7061 7273 6520 7468  erms to parse th
+00003300: 6520 6669 6c65 206e 616d 6520 666f 722e  e file name for.
+00003310: 2045 6163 6820 656e 7472 7920 636f 7272   Each entry corr
+00003320: 6573 706f 6e64 7320 746f 2061 2063 7269  esponds to a cri
+00003330: 7469 6361 6c20 7061 7261 6d65 7465 7220  tical parameter 
+00003340: 6162 6f76 652e 200a 4f70 7469 6f6e 616c  above. .Optional
+00003350: 2069 6620 7573 696e 6720 7461 626c 6520   if using table 
+00003360: 7061 7261 6d65 7465 7220 7665 7269 6669  parameter verifi
+00003370: 6361 7469 6f6e 2c20 686f 7765 7665 7220  cation, however 
+00003380: 6966 2074 6865 2066 696c 6520 6e61 6d65  if the file name
+00003390: 2063 6f6e 7461 696e 7320 7468 6973 2069   contains this i
+000033a0: 6e66 6f72 6d61 7469 6f6e 2069 7420 6361  nformation it ca
+000033b0: 6e20 7573 6520 7468 6973 2069 6e66 6f72  n use this infor
+000033c0: 6d61 7469 6f6e 2074 6f20 6175 746f 2d64  mation to auto-d
+000033d0: 6574 6563 7420 7468 6520 6372 6974 6963  etect the critic
+000033e0: 616c 2070 6172 616d 6574 6572 7320 7573  al parameters us
+000033f0: 6564 2066 6f72 2065 6163 6820 664d 5249  ed for each fMRI
+00003400: 2076 6f6c 756d 652e 0a4e 6f74 653a 2054   volume..Note: T
+00003410: 6869 7320 6669 656c 6420 6361 6e20 6265  his field can be
+00003420: 2062 6c61 6e6b 2e7a 4274 7275 6520 6f72   blank.zBtrue or
+00003430: 2066 616c 7365 2e20 4d61 6b65 2066 6f6c   false. Make fol
+00003440: 6465 7220 7374 7275 6374 7572 6520 7768  der structure wh
+00003450: 656e 2063 7265 6174 696e 6720 7061 7261  en creating para
+00003460: 6d56 616c 7565 732e 6373 76da 0466 756e  mValues.csv..fun
+00003470: 637a a946 6f6c 6465 7220 746f 2066 696e  cz.Folder to fin
+00003480: 6420 6669 6c65 7320 746f 2061 6464 2074  d files to add t
+00003490: 6f20 7061 7261 6d56 616c 7565 732e 6373  o paramValues.cs
+000034a0: 762e 2049 6620 7573 696e 6720 224d 616b  v. If using "Mak
+000034b0: 6520 666f 6c64 6572 2073 7472 7563 7475  e folder structu
+000034c0: 7265 2220 6f70 7469 6f6e 2c20 7468 6973  re" option, this
+000034d0: 2077 696c 6c20 6265 2074 6865 2064 6972   will be the dir
+000034e0: 6563 746f 7279 2074 6865 2066 696c 6573  ectory the files
+000034f0: 2069 6e20 7468 6520 7061 7274 6963 6970   in the particip
+00003500: 616e 7420 666f 6c64 6572 2077 696c 6c20  ant folder will 
+00003510: 6265 206d 6f76 6564 2074 6f2e 2904 da0f  be moved to.)...
+00003520: 7061 7261 6d65 7465 725f 6469 6374 31da  parameter_dict1.
+00003530: 0f70 6172 616d 6574 6572 5f64 6963 7432  .parameter_dict2
+00003540: da15 6d61 6b65 5f66 6f6c 6465 725f 7374  ..make_folder_st
+00003550: 7275 6374 7572 65da 0e70 6172 7369 6e67  ructure..parsing
+00003560: 5f66 6f6c 6465 727a 1547 656e 6572 616c  _folderz.General
+00003570: 2070 6c6f 7420 7365 7474 696e 6773 5a08   plot settingsZ.
+00003580: 706c 6f74 5f64 7069 6958 0200 007a 0a46  plot_dpiiX...z.F
+00003590: 6967 7572 6520 4450 497a 1552 6563 6f6d  igure DPIz.Recom
+000035a0: 6d65 6e64 6564 2076 616c 7565 2036 3030  mended value 600
+000035b0: 5a0e 706c 6f74 5f66 6f6e 745f 7369 7a65  Z.plot_font_size
+000035c0: e928 0000 007a 1046 6967 7572 6520 666f  .(...z.Figure fo
+000035d0: 6e74 2073 697a 657a 1452 6563 6f6d 6d65  nt sizez.Recomme
+000035e0: 6e64 6564 2076 616c 7565 2033 305a 0a70  nded value 30Z.p
+000035f0: 6c6f 745f 7363 616c 65e9 0a00 0000 7a0c  lot_scale.....z.
+00003600: 4669 6775 7265 2073 6361 6c65 7a14 5265  Figure scalez.Re
+00003610: 636f 6d6d 656e 6465 6420 7661 6c75 6520  commended value 
+00003620: 3130 5a10 6d61 6b65 5f76 696f 6c69 6e5f  10Z.make_violin_
+00003630: 706c 6f74 7a11 4d61 6b65 2076 696f 6c69  plotz.Make violi
+00003640: 6e20 706c 6f74 735a 106d 616b 655f 6272  n plotsZ.make_br
+00003650: 6169 6e5f 7461 626c 657a 194d 616b 6520  ain_tablez.Make 
+00003660: 6272 6169 6e20 7669 7375 616c 6973 6174  brain visualisat
+00003670: 696f 6e73 5a13 6d61 6b65 5f6f 6e65 5f72  ionsZ.make_one_r
+00003680: 6567 696f 6e5f 6669 677a 174d 616b 6520  egion_figz.Make 
+00003690: 7265 6769 6f6e 616c 2062 6172 6368 6172  regional barchar
+000036a0: 7473 5a0e 6d61 6b65 5f68 6973 746f 6772  tsZ.make_histogr
+000036b0: 616d 7a18 4d61 6b65 2072 6567 696f 6e61  amz.Make regiona
+000036c0: 6c20 6869 7374 6f67 7261 6d73 5a20 636f  l histogramsZ co
+000036d0: 6c6f 7262 6c69 6e64 5f66 7269 656e 646c  lorblind_friendl
+000036e0: 795f 706c 6f74 5f63 6f6c 6f75 7273 7a22  y_plot_coloursz"
+000036f0: 2366 6665 6461 302c 2023 6665 6232 3463  #ffeda0, #feb24c
+00003700: 2c20 2366 6334 6532 612c 2023 6264 3030  , #fc4e2a, #bd00
+00003710: 3236 7a30 4865 7820 7661 6c75 6573 206f  26z0Hex values o
+00003720: 6620 636f 6c6f 7572 626c 696e 6420 6672  f colourblind fr
+00003730: 6965 6e64 6c79 2063 6f6c 6f75 7220 7363  iendly colour sc
+00003740: 616c 652e 5a11 7265 6769 6f6e 616c 5f66  ale.Z.regional_f
+00003750: 6967 5f72 6f69 737a 0c52 4f49 7320 746f  ig_roisz.ROIs to
+00003760: 2070 6c6f 747a 9350 726f 7669 6465 2061   plotz.Provide a
+00003770: 2063 6f6d 6d61 2d73 6570 6172 6174 6564   comma-separated
+00003780: 206c 6973 7420 6f66 2072 6567 696f 6e73   list of regions
+00003790: 2074 6f20 706c 6f74 2065 2e67 2e20 2733   to plot e.g. '3
+000037a0: 2c20 3527 2c20 7468 6520 7374 7269 6e67  , 5', the string
+000037b0: 2027 616c 6c27 2066 6f72 2061 6c6c 2072   'all' for all r
+000037c0: 6f69 7320 6f72 2074 6865 2073 7472 696e  ois or the strin
+000037d0: 6720 2752 756e 7469 6d65 2720 746f 2070  g 'Runtime' to p
+000037e0: 726f 7669 6465 2072 6567 696f 6e73 2061  rovide regions a
+000037f0: 7420 7275 6e74 696d 652e 7a0b 4272 6169  t runtime.z.Brai
+00003800: 6e20 7461 626c 655a 1262 7261 696e 5f74  n tableZ.brain_t
+00003810: 6967 6874 5f6c 6179 6f75 747a 5074 7275  ight_layoutzPtru
+00003820: 6520 6f72 2066 616c 7365 2e20 5573 6520  e or false. Use 
+00003830: 6120 7469 6768 7420 6c61 796f 7574 2077  a tight layout w
+00003840: 6865 6e20 6c61 7969 6e67 206f 7574 2074  hen laying out t
+00003850: 6865 2066 6967 7572 652e 2052 6563 6f6d  he figure. Recom
+00003860: 6d65 6e64 6564 3a20 6661 6c73 655a 1362  mended: falseZ.b
+00003870: 7261 696e 5f66 6967 5f76 616c 7565 5f6d  rain_fig_value_m
+00003880: 696e 7a1d 4d69 6e69 6d75 6d20 6d65 6469  inz.Minimum medi
+00003890: 616e 2061 6e64 206d 6561 6e20 7661 6c75  an and mean valu
+000038a0: 657a b650 726f 7669 6465 7320 7468 6520  ez.Provides the 
+000038b0: 6d69 6e69 6d75 6d20 7661 6c75 6520 6f66  minimum value of
+000038c0: 2074 6865 2063 6f6c 6f75 7262 6172 2077   the colourbar w
+000038d0: 6865 6e20 6372 6561 7469 6e67 206d 6561  hen creating mea
+000038e0: 6e20 616e 6420 6d65 6469 616e 2069 6d61  n and median ima
+000038f0: 6765 732e 2046 6f72 2065 7861 6d70 6c65  ges. For example
+00003900: 2c20 7365 7420 6d69 6e69 6d75 6d20 746f  , set minimum to
+00003910: 2035 3020 746f 206d 616b 6520 6172 6561   50 to make area
+00003920: 7320 7769 7468 2076 616c 7565 7320 6265  s with values be
+00003930: 6c6f 7720 3530 2061 7070 6561 7220 626c  low 50 appear bl
+00003940: 6163 6b2e 0a52 6563 6f6d 6d65 6e64 6564  ack..Recommended
+00003950: 2076 616c 7565 3a20 305a 1362 7261 696e   value: 0Z.brain
+00003960: 5f66 6967 5f76 616c 7565 5f6d 6178 4e7a  _fig_value_maxNz
+00003970: 1d4d 6178 696d 756d 206d 6564 6961 6e20  .Maximum median 
+00003980: 616e 6420 6d65 616e 2076 616c 7565 6107  and mean valuea.
+00003990: 0100 0050 726f 7669 6465 7320 7468 6520  ...Provides the 
+000039a0: 6d61 7869 6d75 6d20 7661 6c75 6520 6f66  maximum value of
+000039b0: 2074 6865 2063 6f6c 6f75 7262 6172 2077   the colourbar w
+000039c0: 6865 6e20 6372 6561 7469 6e67 206d 6561  hen creating mea
+000039d0: 6e20 616e 6420 6d65 6469 616e 2069 6d61  n and median ima
+000039e0: 6765 732e 2046 6f72 2065 7861 6d70 6c65  ges. For example
+000039f0: 2c20 7365 7420 6d61 7869 6d75 6d20 746f  , set maximum to
+00003a00: 2035 3020 746f 206d 616b 6520 6172 6561   50 to make area
+00003a10: 7320 7769 7468 2076 616c 7565 7320 6162  s with values ab
+00003a20: 6f76 6520 3530 2061 7070 6561 7220 6173  ove 50 appear as
+00003a30: 2074 6865 2062 7269 6768 6573 7420 636f   the brighest co
+00003a40: 6c6f 7572 206f 6e20 7468 6520 636f 6c6f  lour on the colo
+00003a50: 7572 6261 722e 0a52 6563 6f6d 6d65 6e64  urbar..Recommend
+00003a60: 6564 2076 616c 7565 3a20 4e6f 6e65 2e20  ed value: None. 
+00003a70: 4e6f 7465 3a20 7769 6c6c 2064 6566 6175  Note: will defau
+00003a80: 6c74 2074 6f20 3130 3020 666f 7220 7363  lt to 100 for sc
+00003a90: 616c 6564 206d 6170 732e 5a0d 6272 6169  aled maps.Z.brai
+00003aa0: 6e5f 785f 636f 6f72 64e9 ffff ffff 7a66  n_x_coord.....zf
+00003ab0: 566f 7865 6c20 6c6f 6361 7469 6f6e 2074  Voxel location t
+00003ac0: 6f20 736c 6963 6520 7468 6520 696d 6167  o slice the imag
+00003ad0: 6573 2061 7420 696e 2074 6865 2078 2061  es at in the x a
+00003ae0: 7869 732e 2052 6563 6f6d 6d65 6e64 6564  xis. Recommended
+00003af0: 2073 6574 7469 6e67 7320 666f 7220 626f   settings for bo
+00003b00: 7468 2076 6172 6961 626c 6573 3a20 3931  th variables: 91
+00003b10: 206f 7220 3538 5a0d 6272 6169 6e5f 7a5f   or 58Z.brain_z_
+00003b20: 636f 6f72 64e9 1300 0000 7a66 566f 7865  coord.....zfVoxe
+00003b30: 6c20 6c6f 6361 7469 6f6e 2074 6f20 736c  l location to sl
+00003b40: 6963 6520 7468 6520 696d 6167 6573 2061  ice the images a
+00003b50: 7420 696e 2074 6865 207a 2061 7869 732e  t in the z axis.
+00003b60: 2052 6563 6f6d 6d65 6e64 6564 2073 6574   Recommended set
+00003b70: 7469 6e67 7320 666f 7220 626f 7468 2076  tings for both v
+00003b80: 6172 6961 626c 6573 3a20 3931 206f 7220  ariables: 91 or 
+00003b90: 3538 da16 6272 6169 6e5f 7461 626c 655f  58..brain_table_
+00003ba0: 636f 6c5f 6c61 6265 6c73 7a17 4348 414e  col_labelsz.CHAN
+00003bb0: 4745 2054 4f20 4445 5349 5245 4420 4c41  GE TO DESIRED LA
+00003bc0: 4245 4c7a 0d43 6f6c 756d 6e20 6c61 6265  BELz.Column labe
+00003bd0: 6c73 7a12 4c61 6265 6c20 666f 7220 636f  lsz.Label for co
+00003be0: 6c75 6d6e 732e 2906 720b 0000 0072 0c00  lumns.).r....r..
+00003bf0: 0000 7221 0000 0072 0f00 0000 7262 0000  ..r!...r....rb..
+00003c00: 0072 0e00 0000 da16 6272 6169 6e5f 7461  .r......brain_ta
+00003c10: 626c 655f 726f 775f 6c61 6265 6c73 7a0a  ble_row_labelsz.
+00003c20: 526f 7720 6c61 6265 6c73 7a0f 4c61 6265  Row labelsz.Labe
+00003c30: 6c20 666f 7220 726f 7773 2eda 1062 7261  l for rows...bra
+00003c40: 696e 5f74 6162 6c65 5f63 6f6c 7329 0772  in_table_cols).r
+00003c50: 0b00 0000 720c 0000 0072 2000 0000 7252  ....r....r ...rR
+00003c60: 0000 0072 2100 0000 7262 0000 0072 0e00  ...r!...rb...r..
+00003c70: 0000 da10 6272 6169 6e5f 7461 626c 655f  ....brain_table_
+00003c80: 726f 7773 7a0b 5669 6f6c 696e 2070 6c6f  rowsz.Violin plo
+00003c90: 745a 0d74 6162 6c65 5f78 5f6c 6162 656c  tZ.table_x_label
+00003ca0: 7a09 7453 4e52 206d 6561 6e5a 0d74 6162  z.tSNR meanZ.tab
+00003cb0: 6c65 5f79 5f6c 6162 656c 5a03 524f 495a  le_y_labelZ.ROIZ
+00003cc0: 1076 696f 6c69 6e5f 7368 6f77 5f64 6174  .violin_show_dat
+00003cd0: 617a 1053 686f 7720 6461 7461 2070 6f69  az.Show data poi
+00003ce0: 6e74 735a 0d76 696f 6c69 6e5f 6a69 7474  ntsZ.violin_jitt
+00003cf0: 6572 7a12 4a69 7474 6572 2064 6174 6120  erz.Jitter data 
+00003d00: 706f 696e 7473 5a0d 7669 6f6c 696e 5f63  pointsZ.violin_c
+00003d10: 6f6c 6f75 727a 0723 6663 3465 3261 7a2c  olourz.#fc4e2az,
+00003d20: 506c 6f74 7469 6e67 5b22 636f 6c6f 7262  Plotting["colorb
+00003d30: 6c69 6e64 5f66 7269 656e 646c 795f 706c  lind_friendly_pl
+00003d40: 6f74 5f63 6f6c 6f75 7273 225d 7a5d 4865  ot_colours"]z]He
+00003d50: 7820 7661 6c75 6520 6f66 2063 6f6c 6f75  x value of colou
+00003d60: 7220 626c 696e 6420 6672 6965 6e64 6c79  r blind friendly
+00003d70: 2063 6f6c 6f75 722e 2056 616c 7565 2074   colour. Value t
+00003d80: 616b 656e 2066 726f 6d20 636f 6c6f 7262  aken from colorb
+00003d90: 6c69 6e64 2066 7269 656e 646c 7920 706c  lind friendly pl
+00003da0: 6f74 2063 6f6c 6f75 7273 2e5a 0e62 6f78  ot colours.Z.box
+00003db0: 706c 6f74 5f63 6f6c 6f75 727a 0723 6665  plot_colourz.#fe
+00003dc0: 6232 3463 da0a 7461 626c 655f 636f 6c73  b24c..table_cols
+00003dd0: da0a 7461 626c 655f 726f 7773 7a12 5265  ..table_rowsz.Re
+00003de0: 6769 6f6e 616c 2062 6172 2063 6861 7274  gional bar chart
+00003df0: 5a16 7369 6e67 6c65 5f72 6f69 5f66 6967  Z.single_roi_fig
+00003e00: 5f6c 6162 656c 5f78 7a10 4d75 6c74 6962  _label_xz.Multib
+00003e10: 616e 6420 6661 6374 6f72 5a16 7369 6e67  and factorZ.sing
+00003e20: 6c65 5f72 6f69 5f66 6967 5f6c 6162 656c  le_roi_fig_label
+00003e30: 5f79 7a1e 7465 6d70 6f72 616c 2053 6967  _yz.temporal Sig
+00003e40: 6e61 6c20 746f 204e 6f69 7365 2052 6174  nal to Noise Rat
+00003e50: 696f 5a19 7369 6e67 6c65 5f72 6f69 5f66  ioZ.single_roi_f
+00003e60: 6967 5f6c 6162 656c 5f66 696c 6c7a 0c53  ig_label_fillz.S
+00003e70: 454e 5345 2066 6163 746f 72da 1573 696e  ENSE factor..sin
+00003e80: 676c 655f 726f 695f 6669 675f 785f 6178  gle_roi_fig_x_ax
+00003e90: 6973 721d 0000 007a 0942 696e 2077 6964  isr....z.Bin wid
+00003ea0: 7468 7a0c 782d 6178 6973 206c 6162 656c  thz.x-axis label
+00003eb0: da09 4672 6571 7565 6e63 797a 0c79 2d61  ..Frequencyz.y-a
+00003ec0: 7869 7320 6c61 6265 6c67 0000 0000 0000  xis labelg......
+00003ed0: f83f 7a13 5374 6174 6973 7469 6320 6c69  .?z.Statistic li
+00003ee0: 6e65 2073 697a 657a 0953 686f 7720 6d65  ne sizez.Show me
+00003ef0: 616e 7a0b 5368 6f77 206d 6564 6961 6e7a  anz.Show medianz
+00003f00: 0b53 686f 7720 6c65 6765 6e64 7a0c 782d  .Show legendz.x-
+00003f10: 6178 6973 2066 6163 6574 2908 720b 0000  axis facet).r...
+00003f20: 0072 0c00 0000 720f 0000 0072 2000 0000  .r....r....r ...
+00003f30: 7252 0000 0072 2100 0000 7262 0000 0072  rR...r!...rb...r
+00003f40: 0e00 0000 7a0c 792d 6178 6973 2066 6163  ....z.y-axis fac
+00003f50: 6574 7a0a 4269 6e20 636f 6c6f 7572 2907  etz.Bin colour).
+00003f60: 720b 0000 0072 0c00 0000 720f 0000 0072  r....r....r....r
+00003f70: 2000 0000 7252 0000 0072 2100 0000 720e   ...rR...r!...r.
+00003f80: 0000 0029 0cda 1573 696e 676c 655f 726f  ...)...single_ro
+00003f90: 695f 6669 675f 636f 6c6f 7572 7a12 5265  i_fig_colourz.Re
+00003fa0: 6769 6f6e 616c 2068 6973 746f 6772 616d  gional histogram
+00003fb0: 5a12 6869 7374 6f67 7261 6d5f 6269 6e77  Z.histogram_binw
+00003fc0: 6964 7468 5a15 6869 7374 6f67 7261 6d5f  idthZ.histogram_
+00003fd0: 6669 675f 6c61 6265 6c5f 785a 1568 6973  fig_label_xZ.his
+00003fe0: 746f 6772 616d 5f66 6967 5f6c 6162 656c  togram_fig_label
+00003ff0: 5f79 5a18 6869 7374 6f67 7261 6d5f 7374  _yZ.histogram_st
+00004000: 6174 5f6c 696e 655f 7369 7a65 5a13 6869  at_line_sizeZ.hi
+00004010: 7374 6f67 7261 6d5f 7368 6f77 5f6d 6561  stogram_show_mea
+00004020: 6e5a 1568 6973 746f 6772 616d 5f73 686f  nZ.histogram_sho
+00004030: 775f 6d65 6469 616e 5a15 6869 7374 6f67  w_medianZ.histog
+00004040: 7261 6d5f 7368 6f77 5f6c 6567 656e 64da  ram_show_legend.
+00004050: 1568 6973 746f 6772 616d 5f66 6967 5f78  .histogram_fig_x
+00004060: 5f66 6163 6574 da15 6869 7374 6f67 7261  _facet..histogra
+00004070: 6d5f 6669 675f 795f 6661 6365 745a 1468  m_fig_y_facetZ.h
+00004080: 6973 746f 6772 616d 5f66 6967 5f63 6f6c  istogram_fig_col
+00004090: 6f75 7229 07da 075f 5f64 6f63 5f5f da05  our)...__doc__..
+000040a0: 7061 6765 7372 0200 0000 7203 0000 0072  pagesr....r....r
+000040b0: 0400 0000 7205 0000 0072 0600 0000 a900  ....r....r......
+000040c0: 7279 0000 0072 7900 0000 fa5c 2f55 7365  ry...ry....\/Use
+000040d0: 7273 2f6c 7078 6568 3130 2f44 6f63 756d  rs/lpxeh10/Docum
+000040e0: 656e 7473 2f52 6570 6f73 6974 6f72 6965  ents/Repositorie
+000040f0: 732f 664d 5249 5f52 4f49 5f61 6e61 6c79  s/fMRI_ROI_analy
+00004100: 7369 735f 746f 6f6c 2f66 5241 542f 7574  sis_tool/fRAT/ut
+00004110: 696c 732f 6652 4154 5f63 6f6e 6669 675f  ils/fRAT_config_
+00004120: 7365 7475 702e 7079 da08 3c6d 6f64 756c  setup.py..<modul
+00004130: 653e 0100 0000 73b8 0300 0004 0008 0102  e>....s.........
+00004140: 0202 0106 0102 0102 0102 0104 fd02 ff06  ................
+00004150: 0602 0104 0104 fe02 fa06 0a02 0104 0104  ................
+00004160: fe02 f606 0e04 0104 ff02 f206 1104 0104  ................
+00004170: ff02 ef06 1402 0104 ff02 ec0c 1702 0102  ................
+00004180: 0104 fe02 e908 1b02 0102 0104 fe02 e508  ................
+00004190: 1f02 0102 0104 fe02 e104 2302 0106 0102  ..........#.....
+000041a0: 0102 0104 fc02 dd08 2d02 0104 ff02 d30e  ........-.......
+000041b0: 3204 0104 ff02 ce08 3502 cb0a 3702 0104  2.......5...7...
+000041c0: ff02 c904 3a02 0106 0102 0102 0104 fc02  ....:...........
+000041d0: c606 4102 0104 ff04 bf02 4602 010a 0106  ..A.......F.....
+000041e0: 0102 0f04 f002 ff08 1302 0104 ff02 ed0a  ................
+000041f0: 1d02 0104 ff02 e308 2202 0104 ff02 de04  ........".......
+00004200: 2602 0102 0106 0102 0102 0104 fb02 da04  &...............
+00004210: 3204 0102 0104 fe02 ce04 3a06 0102 0102  2.........:.....
+00004220: 0102 0202 0104 fa02 c60c 4204 0104 ff02  ..........B.....
+00004230: be08 4502 0102 0102 0104 fd02 bb08 4b02  ..E...........K.
+00004240: 0102 0102 0104 fd02 b506 5406 0104 0102  ..........T.....
+00004250: 0104 fd02 ac0a 5b04 0104 0104 fe02 a508  ......[.........
+00004260: 5f02 a106 6102 0104 ff02 9f06 6802 0102  _...a.......h...
+00004270: 0104 fe02 980c 6d02 0102 0104 fe02 9306  ......m.........
+00004280: 7206 0104 0102 0104 fd04 8e02 7a02 0108  r...........z...
+00004290: 0102 0102 0104 fe02 ff04 0702 0102 0104  ................
+000042a0: fe02 f904 0f02 0102 0102 0104 fd02 f106  ................
+000042b0: 1402 0102 0104 fe02 ec04 1902 0102 0104  ................
+000042c0: fe02 e706 2402 0104 ff02 dc06 2902 0104  ....$.......)...
+000042d0: ff02 d708 2e02 0102 0104 fe02 d206 3302  ..............3.
+000042e0: 0102 0102 0102 0102 0104 fb02 cd06 3d02  ..............=.
+000042f0: 0102 0102 0304 fb02 c308 4402 bc06 4602  ..........D...F.
+00004300: 0102 0104 fe02 ba06 4a02 010a 0106 0102  ........J.......
+00004310: 0104 fc02 b608 5a02 a606 5c02 0102 0104  ......Z...\.....
+00004320: fe02 a40a 6002 0102 0102 0104 fd02 a004  ....`...........
+00004330: 6502 0102 0102 0104 fd02 9b02 6b02 0102  e...........k...
+00004340: 0102 0104 fd02 0602 0102 0102 0104 fd06  ................
+00004350: 0606 0202 0104 ff08 8700 7f02 0302 0202  ................
+00004360: 0106 0102 0104 fd02 0e02 0104 0102 0102  ................
+00004370: 0104 fc04 0b02 0104 ff06 0302 0104 ff06  ................
+00004380: e302 2302 0108 0102 ff08 0302 0104 ff02  ..#.............
+00004390: fd08 0602 0104 ff02 fa08 0902 0104 ff02  ................
+000043a0: f708 0c02 0104 ff02 f408 0f02 0104 ff02  ................
+000043b0: f108 1202 0104 ff02 ee08 1502 0104 ff02  ................
+000043c0: eb06 1802 0102 0104 fe02 e80a 1c02 0104  ................
+000043d0: ff02 e408 2002 e006 2202 0104 ff02 de08  .... ...".......
+000043e0: 2502 0104 ff02 db08 2b02 0104 ff02 d506  %.......+.......
+000043f0: 3102 0104 ff02 cf0a 3504 0104 ff02 cb0c  1.......5.......
+00004400: 3904 0106 0106 fe04 c70c 3d04 0106 0106  9.........=.....
+00004410: fe02 c30a 4104 0104 0106 fe02 bf0a 4504  ....A.........E.
+00004420: 0104 0106 fe02 bb0a 4902 b70c 4b02 0104  ........I...K...
+00004430: ff02 b50c 4e02 0104 ff02 b20c 5102 0104  ....N.......Q...
+00004440: ff02 af0c 5402 0104 ff02 ac0a 5704 0104  ....T.......W...
+00004450: 0104 0104 fd02 a90a 5c04 0104 0104 0104  ........\.......
+00004460: fd02 a40a 6106 0102 0106 fe02 9f0a 6506  ....a.........e.
+00004470: 0102 0106 fe02 9b0a 6902 970c 6b02 0104  ........i...k...
+00004480: ff02 950c 6e02 0104 ff02 920c 7102 0104  ....n.......q...
+00004490: ff02 8f0a 7406 0102 0106 fe04 8c06 7806  ....t.........x.
+000044a0: 0102 0106 fe06 0410 0206 0206 0102 0104  ................
+000044b0: fe06 0406 0102 0104 fe0a 0402 0104 ff08  ................
+000044c0: 0302 0104 ff08 0302 0104 ff08 0302 0104  ................
+000044d0: ff08 0302 0106 0102 0106 fd08 0502 0104  ................
+000044e0: 0104 0106 fd0a 0504 0104 0104 0106 fd00  ................
+000044f0: 810e e1                                  ...
```

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/figures.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/figures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/html_report.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/html_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/printResults.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/printResults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/statistics.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/statistics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/statmap.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/statmap.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar 14 17:05:44 2023 UTC, .py size: 16388 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,709 +1,581 @@
-00000000: 6f0d 0d0a 0000 0000 68a9 1064 0440 0000  o.......h..d.@..
+00000000: 6f0d 0d0a 0000 0000 9dbe 5b64 2d33 0000  o.........[d-3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
+00000020: 0003 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6401 6c05  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6401 6c06 5a06 6403 6404 6c07  Z.d.d.l.Z.d.d.l.
-00000060: 5400 6401 6108 6405 6109 6405 610a 6406  T.d.a.d.a.d.a.d.
-00000070: 6407 8400 5a0b 6408 6409 8400 5a0c 642c  d...Z.d.d...Z.d,
-00000080: 640a 640b 8401 5a0d 640c 640d 8400 5a0e  d.d...Z.d.d...Z.
-00000090: 640e 640f 8400 5a0f 6410 6411 8400 5a10  d.d...Z.d.d...Z.
-000000a0: 6412 6413 8400 5a11 6414 6415 8400 5a12  d.d...Z.d.d...Z.
-000000b0: 6416 6417 8400 5a13 6418 6419 8400 5a14  d.d...Z.d.d...Z.
-000000c0: 641a 641b 8400 5a15 641c 641d 8400 5a16  d.d...Z.d.d...Z.
-000000d0: 641e 641f 8400 5a17 6420 6421 8400 5a18  d.d...Z.d d!..Z.
-000000e0: 6422 6423 8400 5a19 6424 6425 8400 5a1a  d"d#..Z.d$d%..Z.
-000000f0: 6426 6427 8400 5a1b 6428 6429 8400 5a1c  d&d'..Z.d(d)..Z.
-00000100: 642c 642a 642b 8401 5a1d 6401 5300 292d  d,d*d+..Z.d.S.)-
-00000110: e900 0000 004e 2901 da03 6673 6ce9 0100  .....N)...fsl...
-00000120: 0000 2901 da01 2ada 0063 0100 0000 0000  ..)...*..c......
-00000130: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
-00000140: 0000 7332 0100 0074 006a 017d 0174 006a  ..s2...t.j.}.t.j
-00000150: 0264 016b 0372 0f64 0274 006a 029b 009d  .d.k.r.d.t.j....
-00000160: 027d 026e 147c 0064 036b 0272 1664 047d  .}.n.|.d.k.r.d.}
-00000170: 026e 0d7c 0064 056b 0272 1d64 067d 026e  .n.|.d.k.r.d.}.n
-00000180: 067c 0064 076b 0272 2364 087d 0274 006a  .|.d.k.r#d.}.t.j
-00000190: 0364 0976 0072 3374 0464 0a83 0101 0074  .d.v.r3t.d.....t
-000001a0: 056a 0664 0b64 0c8d 017d 036e 0374 006a  .j.d.d...}.n.t.j
-000001b0: 037d 0374 05a0 077c 03a1 015c 027d 047d  .}.t...|...\.}.}
-000001c0: 0564 0d64 0e84 007c 0444 0083 017d 067c  .d.d...|.D...}.|
-000001d0: 0644 005d 4d7d 0774 05a0 087c 079b 0064  .D.]M}.t...|...d
-000001e0: 0f7c 019b 009d 0364 1064 1164 12a1 047c  .|.....d.d.d...|
-000001f0: 067c 073c 0064 137c 0276 0072 8474 05a0  .|.<.d.|.v.r.t..
-00000200: 097c 079b 0064 149d 02a1 0101 0074 056a  .|...d.......t.j
-00000210: 097c 079b 0064 0f7c 029b 009d 0364 1564  .|...d.|.....d.d
-00000220: 168d 0201 0074 056a 0a7c 079b 0064 0f7c  .....t.j.|...d.|
-00000230: 029b 009d 0374 0b74 0c64 177c 009b 0064  .....t.t.d.|...d
-00000240: 189d 0367 0164 1964 1a8d 0501 0071 4674  ...g.d.d.....qFt
-00000250: 056a 097c 079b 0064 0f7c 019b 0064 0f7c  .j.|...d.|...d.|
-00000260: 029b 009d 0564 1564 168d 0201 0071 467c  .....d.d.....qF|
-00000270: 067c 027c 0166 0353 0029 1b4e da07 4445  .|.|.f.S.).N..DE
-00000280: 4641 554c 547a 0973 7461 746d 6170 732f  FAULTz.statmaps/
-00000290: fa09 496d 6167 6520 534e 527a 1873 7461  ..Image SNRz.sta
-000002a0: 746d 6170 732f 696d 6167 6553 4e52 5f72  tmaps/imageSNR_r
-000002b0: 6570 6f72 74fa 0c54 656d 706f 7261 6c20  eport..Temporal 
-000002c0: 534e 527a 1b73 7461 746d 6170 732f 7465  SNRz.statmaps/te
-000002d0: 6d70 6f72 616c 534e 525f 7265 706f 7274  mporalSNR_report
-000002e0: fa12 4164 6420 4761 7573 7369 616e 206e  ..Add Gaussian n
-000002f0: 6f69 7365 5a0b 6164 6465 645f 6e6f 6973  oiseZ.added_nois
-00000300: 6529 0272 0500 0000 fa01 207a 3853 656c  e).r...... z8Sel
-00000310: 6563 7420 7468 6520 6469 7265 6374 6f72  ect the director
-00000320: 7920 7768 6963 6820 636f 6e74 6169 6e73  y which contains
-00000330: 2074 6865 2073 7562 6a65 6374 2066 6f6c   the subject fol
-00000340: 6465 7273 2e7a 3753 656c 6563 7420 7468  ders.z7Select th
-00000350: 6520 6469 7265 6374 6f72 7920 7768 6963  e directory whic
-00000360: 6820 636f 6e74 6169 6e73 2074 6865 2073  h contains the s
-00000370: 7562 6a65 6374 2066 6f6c 6465 7273 2901  ubject folders).
-00000380: da05 7469 746c 6563 0100 0000 0000 0000  ..titlec........
-00000390: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-000003a0: 7312 0000 0069 007c 005d 057d 017c 0164  s....i.|.].}.|.d
-000003b0: 0093 0271 0253 00a9 014e a900 2902 da02  ...q.S...N..)...
-000003c0: 2e30 da0b 7061 7274 6963 6970 616e 7472  .0..participantr
-000003d0: 0d00 0000 720d 0000 00fa 522f 5573 6572  ....r.....R/User
-000003e0: 732f 6c70 7865 6831 302f 446f 6375 6d65  s/lpxeh10/Docume
-000003f0: 6e74 732f 5265 706f 7369 746f 7269 6573  nts/Repositories
-00000400: 2f66 4d52 495f 524f 495f 616e 616c 7973  /fMRI_ROI_analys
-00000410: 6973 5f74 6f6f 6c2f 6652 4154 2f75 7469  is_tool/fRAT/uti
-00000420: 6c73 2f73 7461 746d 6170 2e70 79da 0a3c  ls/statmap.py..<
-00000430: 6469 6374 636f 6d70 3e24 0000 0073 0200  dictcomp>$...s..
-00000440: 0000 1200 7a1e 6669 6c65 5f73 6574 7570  ....z.file_setup
-00000450: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
-00000460: 6f6d 703e fa01 2fda 0368 6472 7a06 6e69  omp>../..hdrz.ni
-00000470: 692e 677a da03 6e69 69da 0873 7461 746d  i.gz..nii..statm
-00000480: 6170 737a 092f 7374 6174 6d61 7073 54a9  apsz./statmapsT.
-00000490: 01da 0a64 656c 6574 655f 6f6c 647a 1b73  ...delete_oldz.s
-000004a0: 7461 7469 7374 6963 616c 5f6d 6170 5f63  tatistical_map_c
-000004b0: 7265 6174 6564 203d 2027 7a02 270a da0e  reated = 'z.'...
-000004c0: 7374 6174 6d61 705f 636f 6e66 6967 2902  statmap_config).
-000004d0: da0f 6164 6469 7469 6f6e 616c 5f69 6e66  ..additional_inf
-000004e0: 6fda 0f6e 6577 5f63 6f6e 6669 675f 6e61  o..new_config_na
-000004f0: 6d65 290d da06 636f 6e66 6967 da11 696e  me)...config..in
-00000500: 7075 745f 666f 6c64 6572 5f6e 616d 65da  put_folder_name.
-00000510: 126f 7574 7075 745f 666f 6c64 6572 5f6e  .output_folder_n
-00000520: 616d 65da 0b62 6173 655f 666f 6c64 6572  ame..base_folder
-00000530: da05 7072 696e 74da 0555 7469 6c73 da0c  ..print..Utils..
-00000540: 6669 6c65 5f62 726f 7773 6572 da15 6669  file_browser..fi
-00000550: 6e64 5f70 6172 7469 6369 7061 6e74 5f64  nd_participant_d
-00000560: 6972 73da 0a66 696e 645f 6669 6c65 73da  irs..find_files.
-00000570: 1263 6865 636b 5f61 6e64 5f6d 616b 655f  .check_and_make_
-00000580: 6469 72da 0b73 6176 655f 636f 6e66 6967  dir..save_config
-00000590: da0b 636f 6e66 6967 5f70 6174 68da 0f63  ..config_path..c
-000005a0: 6f6e 6669 675f 6669 6c65 6e61 6d65 2908  onfig_filename).
-000005b0: da04 6675 6e63 da0d 6669 6c65 5f6c 6f63  ..func..file_loc
-000005c0: 6174 696f 6eda 0d6f 7574 7075 745f 666f  ation..output_fo
-000005d0: 6c64 6572 da11 6261 7365 5f73 7562 5f6c  lder..base_sub_l
-000005e0: 6f63 6174 696f 6eda 0f70 6172 7469 6369  ocation..partici
-000005f0: 7061 6e74 5f64 6972 da01 5fda 0c70 6172  pant_dir.._..par
-00000600: 7469 6369 7061 6e74 7372 0f00 0000 720d  ticipantsr....r.
-00000610: 0000 0072 0d00 0000 7210 0000 00da 0a66  ...r....r......f
-00000620: 696c 655f 7365 7475 700f 0000 0073 3400  ile_setup....s4.
-00000630: 0000 0601 0a02 0e01 0801 0601 0801 0601  ................
-00000640: 0801 0401 0a02 0801 0e01 0603 0e03 0e01  ................
-00000650: 0802 1e02 0802 1001 1801 1401 0c01 0201  ................
-00000660: 08fe 2004 0a02 722f 0000 0063 0100 0000  .. ...r/...c....
-00000670: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00000680: 4300 0000 732a 0000 0074 00a0 017c 00a1  C...s*...t...|..
-00000690: 017d 017c 016a 0264 0119 0064 0219 007d  .}.|.j.d...d...}
-000006a0: 0264 0364 0474 036a 0414 007c 0214 001b  .d.d.t.j...|....
-000006b0: 0053 0029 054e da06 7069 7864 696d e904  .S.).N..pixdim..
-000006c0: 0000 0072 0300 0000 e902 0000 0029 05da  ...r.........)..
-000006d0: 036e 6962 da04 6c6f 6164 da06 6865 6164  .nib..load..head
-000006e0: 6572 721b 0000 00da 1668 6967 6870 6173  err......highpas
-000006f0: 735f 6669 6c74 6572 5f63 7574 6f66 6629  s_filter_cutoff)
-00000700: 03da 0966 696c 655f 7061 7468 da04 6461  ...file_path..da
-00000710: 7461 da02 5452 720d 0000 0072 0d00 0000  ta..TRr....r....
-00000720: 7210 0000 00da 1a63 616c 6375 6c61 7465  r......calculate
-00000730: 5f73 6967 6d61 5f69 6e5f 766f 6c75 6d65  _sigma_in_volume
-00000740: 7336 0000 0073 0600 0000 0a01 0e01 1203  s6...s..........
-00000750: 723a 0000 0063 0500 0000 0000 0000 0000  r:...c..........
-00000760: 0000 0600 0000 0800 0000 4300 0000 733e  ..........C...s>
-00000770: 0000 0074 00a0 017c 0064 007c 04a1 037d  ...t...|.d.|...}
-00000780: 0574 00a0 027c 057c 039b 0064 017c 029b  .t...|.|...d.|..
-00000790: 007c 019b 0064 029d 05a1 0201 007c 039b  .|...d.......|..
-000007a0: 0064 017c 029b 007c 019b 0064 029d 0553  .d.|...|...d...S
-000007b0: 0029 034e 7212 0000 007a 072e 6e69 692e  .).Nr....z..nii.
-000007c0: 677a 2903 7233 0000 00da 0a4e 6966 7469  gz).r3.....Nifti
-000007d0: 3150 6169 72da 0473 6176 6529 0672 3800  1Pair..save).r8.
-000007e0: 0000 da03 6578 74da 0b6e 6f5f 6578 745f  ....ext..no_ext_
-000007f0: 6669 6c65 722a 0000 0072 3500 0000 da05  filer*...r5.....
-00000800: 6272 6169 6e72 0d00 0000 720d 0000 0072  brainr....r....r
-00000810: 1000 0000 da0a 7361 7665 5f62 7261 696e  ......save_brain
-00000820: 3e00 0000 7306 0000 000e 011c 0114 0272  >...s..........r
-00000830: 4000 0000 6303 0000 0000 0000 0000 0000  @...c...........
-00000840: 0003 0000 0008 0000 0043 0000 0073 b000  .........C...s..
-00000850: 0000 7400 6a01 6a02 7c00 7c02 9b00 6401  ..t.j.j.|.|...d.
-00000860: 7c01 9b00 6402 9d04 6403 8d02 a003 a100  |...d...d.......
-00000870: 0100 7400 6a01 6a04 7c00 7c02 9b00 6401  ..t.j.j.|.|...d.
-00000880: 7c01 9b00 6404 9d04 6403 8d02 a003 a100  |...d...d.......
-00000890: 0100 7400 6a01 6a05 6405 7c02 9b00 6401  ..t.j.j.d.|...d.
-000008a0: 7c01 9b00 6402 9d04 7c02 9b00 6401 7c01  |...d...|...d.|.
-000008b0: 9b00 6404 9d04 7c02 9b00 6401 7c01 9b00  ..d...|...d.|...
-000008c0: 6406 9d04 6407 8d04 a003 a100 0100 7400  d...d.........t.
-000008d0: 6a01 6a06 7c02 9b00 6401 7c01 9b00 6406  j.j.|...d.|...d.
-000008e0: 9d04 6408 6409 7c02 9b00 6401 7c01 9b00  ..d.d.|...d.|...
-000008f0: 6406 9d04 640a 8d04 a003 a100 0100 6400  d...d.........d.
-00000900: 5300 290b 4e72 1200 0000 fa0d 5f74 4d65  S.).Nr......_tMe
-00000910: 616e 2e6e 6969 2e67 7aa9 02da 0769 6e5f  an.nii.gz....in_
-00000920: 6669 6c65 da08 6f75 745f 6669 6c65 7a0c  file..out_filez.
-00000930: 5f74 5374 642e 6e69 692e 677a da03 6469  _tStd.nii.gz..di
-00000940: 767a 0c5f 7453 4e52 2e6e 6969 2e67 7aa9  vz._tSNR.nii.gz.
-00000950: 04da 096f 7065 7261 7469 6f6e 7243 0000  ...operationrC..
-00000960: 00da 0c6f 7065 7261 6e64 5f66 696c 6572  ...operand_filer
-00000970: 4400 0000 6700 0000 0000 408f 40da 0561  D...g.....@.@..a
-00000980: 626f 7665 2904 7243 0000 00da 0674 6872  bove).rC.....thr
-00000990: 6573 68da 0964 6972 6563 7469 6f6e 7244  esh..directionrD
-000009a0: 0000 0029 0772 0200 0000 da05 6d61 7468  ...).r......math
-000009b0: 73da 094d 6561 6e49 6d61 6765 da03 7275  s..MeanImage..ru
-000009c0: 6eda 0853 7464 496d 6167 65da 0b42 696e  n..StdImage..Bin
-000009d0: 6172 794d 6174 6873 da09 5468 7265 7368  aryMaths..Thresh
-000009e0: 6f6c 6429 03da 0466 696c 6572 3e00 0000  old)...filer>...
-000009f0: 722a 0000 0072 0d00 0000 720d 0000 0072  r*...r....r....r
-00000a00: 1000 0000 da10 7465 6d70 6f72 616c 534e  ......temporalSN
-00000a10: 525f 6361 6c63 4500 0000 7316 0000 0020  R_calcE...s.... 
-00000a20: 0120 0216 030e 010e 0104 fe06 0218 030e  . ..............
-00000a30: 0104 ff0a 0172 5300 0000 6305 0000 0000  .....rS...c.....
-00000a40: 0000 0000 0000 000b 0000 0008 0000 0043  ...............C
-00000a50: 0000 0073 f600 0000 7400 6a01 6a02 7c00  ...s....t.j.j.|.
-00000a60: 7c03 9b00 6401 7c02 9b00 6402 9d04 6403  |...d.|...d...d.
-00000a70: 8d02 a003 a100 0100 7404 6a05 7216 6404  ........t.j.r.d.
-00000a80: 7d05 6e02 6405 7d05 7404 6a06 722d 7400  }.n.d.}.t.j.r-t.
-00000a90: 6a07 7c01 7c05 6406 6407 8d03 a003 a100  j.|.|.d.d.......
-00000aa0: 7d06 7c06 6a08 a009 a100 6408 1900 7d07  }.|.j.....d...}.
-00000ab0: 6e25 740a 7c04 8301 6a0b 6409 1900 7d08  n%t.|...j.d...}.
-00000ac0: 740c 6a0d a00e 740a 7c04 8301 a101 640a  t.j...t.|.....d.
-00000ad0: 1900 7d09 740f a010 7c08 9b00 640b 9d02  ..}.t...|...d...
-00000ae0: a101 7d0a 7411 7c0a 7c0a 640c 1900 7c09  ..}.t.|.|.d...|.
-00000af0: 6b02 1900 640d 1900 8301 7d07 7400 6a01  k...d.....}.t.j.
-00000b00: 6a12 640e 7c03 9b00 6401 7c02 9b00 6402  j.d.|...d.|...d.
-00000b10: 9d04 7c07 7c03 9b00 6401 7c02 9b00 640f  ..|.|...d.|...d.
-00000b20: 9d04 6410 8d04 a003 a100 0100 7404 6a13  ..d.........t.j.
-00000b30: 7279 7413 7c03 9b00 6401 7c02 9b00 640f  ryt.|...d.|...d.
-00000b40: 9d04 8301 0100 6400 5300 6400 5300 2911  ......d.S.d.S.).
-00000b50: 4e72 1200 0000 7241 0000 0072 4200 0000  Nr....rA...rB...
-00000b60: 7a02 2d53 7a02 2d73 da09 616c 6c61 746f  z.-Sz.-s..allato
-00000b70: 6e63 6529 0372 4300 0000 da09 6f70 5f73  nce).rC.....op_s
-00000b80: 7472 696e 67da 0f74 6572 6d69 6e61 6c5f  tring..terminal_
-00000b90: 6f75 7470 7574 da08 6f75 745f 7374 6174  output..out_stat
-00000ba0: 7201 0000 0072 0300 0000 fa10 2f6e 6f69  r....r....../noi
-00000bb0: 7365 5661 6c75 6573 2e63 7376 da0b 5061  seValues.csv..Pa
-00000bc0: 7274 6963 6970 616e 747a 1042 6163 6b67  rticipantz.Backg
-00000bd0: 726f 756e 6420 6e6f 6973 6572 4500 0000  round noiserE...
-00000be0: 7a0c 5f69 534e 522e 6e69 692e 677a 2904  z._iSNR.nii.gz).
-00000bf0: 7247 0000 0072 4300 0000 da0d 6f70 6572  rG...rC.....oper
-00000c00: 616e 645f 7661 6c75 6572 4400 0000 2914  and_valuerD...).
-00000c10: 7202 0000 0072 4c00 0000 724d 0000 0072  r....rL...rM...r
-00000c20: 4e00 0000 721b 0000 00da 2069 534e 525f  N...r..... iSNR_
-00000c30: 7374 645f 7573 655f 6f6e 6c79 5f6e 6f6e  std_use_only_non
-00000c40: 7a65 726f 5f76 6f78 656c 73da 0c6e 6f69  zero_voxels..noi
-00000c50: 7365 5f76 6f6c 756d 65da 0a49 6d61 6765  se_volume..Image
-00000c60: 5374 6174 73da 076f 7574 7075 7473 da03  Stats..outputs..
-00000c70: 6765 74da 0450 6174 68da 0770 6172 656e  get..Path..paren
-00000c80: 7473 da02 6f73 da04 7061 7468 da05 7370  ts..os..path..sp
-00000c90: 6c69 74da 0270 64da 0872 6561 645f 6373  lit..pd..read_cs
-00000ca0: 76da 0566 6c6f 6174 7250 0000 00da 146d  v..floatrP.....m
-00000cb0: 6167 6e69 7475 6465 5f63 6f72 7265 6374  agnitude_correct
-00000cc0: 696f 6e29 0bda 0966 756e 635f 6669 6c65  ion)...func_file
-00000cd0: da0a 6e6f 6973 655f 6669 6c65 723e 0000  ..noise_filer>..
-00000ce0: 0072 2a00 0000 722c 0000 005a 0a73 7464  .r*...r,...Z.std
-00000cf0: 5f73 7472 696e 67da 0373 7464 5a0b 6e6f  _string..stdZ.no
-00000d00: 6973 655f 7661 6c75 6572 2b00 0000 da10  ise_valuer+.....
-00000d10: 7061 7274 6963 6970 616e 745f 6e61 6d65  participant_name
-00000d20: da0f 6e6f 6973 655f 7661 6c75 655f 6373  ..noise_value_cs
-00000d30: 7672 0d00 0000 720d 0000 0072 1000 0000  vr....r....r....
-00000d40: da0d 696d 6167 6553 4e52 5f63 616c 6354  ..imageSNR_calcT
-00000d50: 0000 0073 3000 0000 2001 0602 0601 0402  ...s0... .......
-00000d60: 0602 0801 0201 04ff 0401 02ff 1002 0e03  ................
-00000d70: 1401 1002 1801 0803 0e01 0201 0e01 04fd  ................
-00000d80: 0603 0602 1801 04ff 726e 0000 0063 0100  ........rn...c..
-00000d90: 0000 0000 0000 0000 0000 0100 0000 0600  ................
-00000da0: 0000 4300 0000 731c 0000 0074 006a 016a  ..C...s....t.j.j
-00000db0: 027c 0064 0164 027c 0064 038d 04a0 03a1  .|.d.d.|.d......
-00000dc0: 0001 0064 0053 0029 044e da03 6d75 6c67  ...d.S.).N..mulg
-00000dd0: 6666 6666 6666 e63f 2904 7243 0000 0072  ffffff.?).rC...r
-00000de0: 4700 0000 725a 0000 0072 4400 0000 2904  G...rZ...rD...).
-00000df0: 7202 0000 0072 4c00 0000 7250 0000 0072  r....rL...rP...r
-00000e00: 4e00 0000 2901 da09 6669 6c65 5f6e 616d  N...)...file_nam
-00000e10: 6572 0d00 0000 720d 0000 0072 1000 0000  er....r....r....
-00000e20: 7268 0000 0072 0000 0073 0200 0000 1c01  rh...r...s......
-00000e30: 7268 0000 0063 0400 0000 0000 0000 0000  rh...c..........
-00000e40: 0000 0a00 0000 0800 0000 4300 0000 73e0  ..........C...s.
-00000e50: 0000 0074 00a0 017c 00a1 015c 027d 047d  ...t...|...\.}.}
-00000e60: 0574 026a 0364 016b 0272 2c7c 0464 0064  .t.j.d.k.r,|.d.d
-00000e70: 0085 0264 0064 0085 0264 0064 0085 0264  ...d.d...d.d...d
-00000e80: 0266 0419 007c 0464 0064 0085 0264 0064  .f...|.d.d...d.d
-00000e90: 0085 0264 0064 0085 0264 0064 0285 0266  ...d.d...d.d...f
-00000ea0: 0419 0002 027d 067d 076e 2974 026a 0364  .....}.}.n)t.j.d
-00000eb0: 036b 0272 517c 0464 0064 0085 0264 0064  .k.rQ|.d.d...d.d
-00000ec0: 0085 0264 0064 0085 0264 0466 0419 007c  ...d.d...d.f...|
-00000ed0: 0464 0064 0085 0264 0064 0085 0264 0064  .d.d...d.d...d.d
-00000ee0: 0085 0264 0564 0085 0266 0419 0002 027d  ...d.d...f.....}
-00000ef0: 067d 076e 0474 0464 0683 0182 0174 057c  .}.n.t.d.....t.|
-00000f00: 0664 077c 017c 027c 0583 057d 0874 067c  .d.|.|.|...}.t.|
-00000f10: 077c 057c 017c 0364 0874 026a 03a0 07a1  .|.|.|.d.t.j....
-00000f20: 009b 0064 099d 0383 057d 097c 097c 0866  ...d.....}.|.|.f
-00000f30: 0253 0029 0a4e da03 456e 64e9 ffff ffff  .S.).N..End.....
-00000f40: da09 4265 6769 6e6e 696e 6772 0100 0000  ..Beginningr....
-00000f50: 7203 0000 007a 204e 6f69 7365 2076 6f6c  r....z Noise vol
-00000f60: 756d 6520 6c6f 6361 7469 6f6e 206e 6f74  ume location not
-00000f70: 2076 616c 6964 2e5a 0d5f 6e6f 6973 655f   valid.Z._noise_
-00000f80: 766f 6c75 6d65 7a1a 5265 6d6f 7665 6420  volumez.Removed 
-00000f90: 6e6f 6973 6520 766f 6c75 6d65 2066 726f  noise volume fro
-00000fa0: 6d20 7a0e 206f 6620 7469 6d65 7365 7269  m z. of timeseri
-00000fb0: 6573 2908 7220 0000 00da 0a6c 6f61 645f  es).r .....load_
-00000fc0: 6272 6169 6e72 1b00 0000 da15 6e6f 6973  brainr......nois
-00000fd0: 655f 766f 6c75 6d65 5f6c 6f63 6174 696f  e_volume_locatio
-00000fe0: 6eda 0945 7863 6570 7469 6f6e 7240 0000  n..Exceptionr@..
-00000ff0: 00da 1673 6176 655f 746f 5f63 6c65 616e  ...save_to_clean
-00001000: 6564 5f66 6f6c 6465 72da 056c 6f77 6572  ed_folder..lower
-00001010: 290a 7252 0000 0072 3e00 0000 722a 0000  ).rR...r>...r*..
-00001020: 0072 0f00 0000 7238 0000 0072 3500 0000  .r....r8...r5...
-00001030: 5a0a 6e6f 6973 655f 6461 7461 5a09 6675  Z.noise_dataZ.fu
-00001040: 6e63 5f64 6174 6172 6a00 0000 7269 0000  nc_datarj...ri..
-00001050: 0072 0d00 0000 720d 0000 0072 1000 0000  .r....r....r....
-00001060: da18 7365 7061 7261 7465 5f6e 6f69 7365  ..separate_noise
-00001070: 5f66 726f 6d5f 6675 6e63 7600 0000 7316  _from_funcv...s.
-00001080: 0000 000e 010a 0240 010a 0140 0108 0210  .......@...@....
-00001090: 020a 0210 0104 ff08 0372 7900 0000 6305  .........ry...c.
-000010a0: 0000 0000 0000 0000 0000 0006 0000 0008  ................
-000010b0: 0000 0043 0000 0073 7a00 0000 7400 7c03  ...C...sz...t.|.
-000010c0: 9b00 6401 7401 6a02 9b00 6402 9d04 6403  ..d.t.j...d...d.
-000010d0: 8302 8f18 7d05 7c05 a003 6404 a101 0100  ....}.|...d.....
-000010e0: 7c05 a004 7c02 9b00 6405 7c04 9b00 6406  |...|...d.|...d.
-000010f0: 9d04 a101 0100 5700 6400 0400 0400 8303  ......W.d.......
-00001100: 0100 6e08 3100 7327 7701 0100 0100 0100  ..n.1.s'w.......
-00001110: 5900 0100 7405 7c00 6407 7c02 7c03 9b00  Y...t.|.d.|.|...
-00001120: 6401 7401 6a02 9b00 6408 9d04 7c01 8305  d.t.j...d...|...
-00001130: 7d00 7c00 5300 2909 4e72 1200 0000 7a22  }.|.S.).Nr....z"
-00001140: 5f63 6c65 616e 6564 2f63 6861 6e67 6573  _cleaned/changes
-00001150: 5f6d 6164 655f 746f 5f66 696c 6573 2e74  _made_to_files.t
-00001160: 7874 7a02 612b 7201 0000 007a 023a 20da  xtz.a+r....z.: .
-00001170: 010a 7205 0000 00da 085f 636c 6561 6e65  ..r......_cleane
-00001180: 6429 06da 046f 7065 6e72 1b00 0000 721c  d)...openr....r.
-00001190: 0000 00da 0473 6565 6bda 0577 7269 7465  .....seek..write
-000011a0: 7240 0000 0029 0672 3800 0000 7235 0000  r@...).r8...r5..
-000011b0: 0072 3e00 0000 720f 0000 00da 066d 6574  .r>...r......met
-000011c0: 686f 64da 0166 720d 0000 0072 0d00 0000  hod..fr....r....
-000011d0: 7210 0000 0072 7700 0000 8800 0000 730c  r....rw.......s.
-000011e0: 0000 001a 010a 0118 011c fe1e 0404 0272  ...............r
-000011f0: 7700 0000 6303 0000 0000 0000 0000 0000  w...c...........
-00001200: 0004 0000 0008 0000 0043 0000 0073 a800  .........C...s..
-00001210: 0000 7400 7c00 8301 7d03 7401 6a02 6a03  ..t.|...}.t.j.j.
-00001220: 7c00 9b00 7c01 9b00 6401 7c02 9b00 6402  |...|...d.|...d.
-00001230: 9d04 6403 8d02 a004 a100 0100 7401 6a05  ..d.........t.j.
-00001240: 7c00 9b00 7c01 9b00 6401 7c02 9b00 6404  |...|...d.|...d.
-00001250: 9d04 7c03 6405 8d03 a004 a100 0100 7401  ..|.d.........t.
-00001260: 6a02 6a06 6406 7c01 9b00 6401 7c02 9b00  j.j.d.|...d.|...
-00001270: 6402 9d04 7c01 9b00 6401 7c02 9b00 6404  d...|...d.|...d.
-00001280: 9d04 7c01 9b00 6401 7c02 9b00 6407 9d04  ..|...d.|...d...
-00001290: 6408 8d04 a004 a100 0100 7c01 9b00 6401  d.........|...d.
-000012a0: 7c02 9b00 6407 9d04 7c01 9b00 6401 7c02  |...d...|...d.|.
-000012b0: 9b00 6404 9d04 6602 5300 2909 4e72 1200  ..d...f.S.).Nr..
-000012c0: 0000 7241 0000 0072 4200 0000 7a10 5f66  ..rA...rB...z._f
-000012d0: 696c 7465 7265 642e 6e69 692e 677a 2903  iltered.nii.gz).
-000012e0: 7243 0000 0072 4400 0000 da0e 6869 6768  rC...rD.....high
-000012f0: 7061 7373 5f73 6967 6d61 da03 6164 647a  pass_sigma..addz
-00001300: 1d5f 6669 6c74 6572 6564 5f72 6573 746f  ._filtered_resto
-00001310: 7265 646d 6561 6e2e 6e69 692e 677a 7246  redmean.nii.gzrF
-00001320: 0000 0029 0772 3a00 0000 7202 0000 0072  ...).r:...r....r
-00001330: 4c00 0000 724d 0000 0072 4e00 0000 da0e  L...rM...rN.....
-00001340: 5465 6d70 6f72 616c 4669 6c74 6572 7250  TemporalFilterrP
-00001350: 0000 0029 0472 3700 0000 722a 0000 0072  ...).r7...r*...r
-00001360: 3e00 0000 5a10 7369 676d 615f 696e 5f76  >...Z.sigma_in_v
-00001370: 6f6c 756d 6573 720d 0000 0072 0d00 0000  olumesr....r....
-00001380: 7210 0000 00da 1268 6967 6870 6173 735f  r......highpass_
-00001390: 6669 6c74 6572 696e 6792 0000 0073 1e00  filtering....s..
-000013a0: 0000 0801 2202 0802 0e01 0201 04fe 0602  ...."...........
-000013b0: 1602 0e01 0e01 04fe 0602 0e02 0e01 04ff  ................
-000013c0: 7284 0000 0063 0100 0000 0000 0000 0000  r....c..........
-000013d0: 0000 0200 0000 0400 0000 4300 0000 7318  ..........C...s.
-000013e0: 0000 007c 0044 005d 077d 0174 00a0 017c  ...|.D.].}.t...|
-000013f0: 01a1 0101 0071 0264 0053 0072 0c00 0000  .....q.d.S.r....
-00001400: 2902 7262 0000 00da 0672 656d 6f76 6529  ).rb.....remove)
-00001410: 02da 0f72 6564 756e 6461 6e74 5f66 696c  ...redundant_fil
-00001420: 6573 7252 0000 0072 0d00 0000 720d 0000  esrR...r....r...
-00001430: 0072 1000 0000 da0c 6465 6c65 7465 5f66  .r......delete_f
-00001440: 696c 6573 a300 0000 7306 0000 0008 010c  iles....s.......
-00001450: 0104 ff72 8700 0000 6306 0000 0000 0000  ...r....c.......
-00001460: 0000 0000 0006 0000 0006 0000 0043 0000  .............C..
-00001470: 0073 3800 0000 7c00 6401 6b02 720e 7400  .s8...|.d.k.r.t.
-00001480: 7c01 7c03 7c02 7c04 7c05 8305 0100 6400  |.|.|.|.|.....d.
-00001490: 5300 7c00 6402 6b02 721a 7401 7c01 7c02  S.|.d.k.r.t.|.|.
-000014a0: 7c04 8303 0100 6400 5300 6400 5300 2903  |.....d.S.d.S.).
-000014b0: 4e72 0700 0000 7208 0000 0029 0272 6e00  Nr....r....).rn.
-000014c0: 0000 7253 0000 0029 0672 2800 0000 7252  ..rS...).r(...rR
-000014d0: 0000 0072 3e00 0000 726a 0000 0072 2a00  ...r>...rj...r*.
-000014e0: 0000 720f 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000014f0: 0072 1000 0000 da0f 6372 6561 7465 5f73  .r......create_s
-00001500: 7461 746d 6170 73a8 0000 0073 0a00 0000  tatmaps....s....
-00001510: 0801 1401 0801 1001 04ff 7288 0000 0063  ..........r....c
-00001520: 0400 0000 0000 0000 0000 0000 0d00 0000  ................
-00001530: 0800 0000 4300 0000 733e 0100 0064 007d  ....C...s>...d.}
-00001540: 0467 007d 0567 007d 0674 00a0 017c 00a1  .g.}.g.}.t...|..
-00001550: 015c 027d 077d 0874 027c 0764 017c 017c  .\.}.}.t.|.d.|.|
-00001560: 039b 0064 0274 036a 049b 0064 039d 047c  ...d.t.j...d...|
-00001570: 0883 0501 0074 036a 0572 2d74 067c 007c  .....t.j.r-t.|.|
-00001580: 017c 027c 0383 045c 027d 007d 047c 05a0  .|.|...\.}.}.|..
-00001590: 077c 04a1 0101 0074 036a 0872 4474 087c  .|.....t.j.rDt.|
-000015a0: 007c 017c 027c 0383 045c 037d 007d 097d  .|.|.|...\.}.}.}
-000015b0: 0a7c 05a0 097c 0aa1 0101 007c 06a0 097c  .|...|.....|...|
-000015c0: 09a1 0101 0074 036a 0a72 697c 029b 0064  .....t.j.ri|...d
-000015d0: 027c 019b 0064 049d 047d 0b74 0b6a 0c7c  .|...d...}.t.j.|
-000015e0: 007c 0b64 058d 02a0 0da1 0001 007c 0b7d  .|.d.........|.}
-000015f0: 0074 00a0 017c 00a1 015c 027d 077d 0874  .t...|...\.}.}.t
-00001600: 0e7c 077c 087c 017c 0364 0683 057d 0074  .|.|.|.|.d...}.t
-00001610: 036a 0f72 8774 0b6a 107c 0074 036a 1174  .j.r.t.j.|.t.j.t
-00001620: 036a 127c 029b 0064 027c 019b 0064 079d  .j.|...d.|...d..
-00001630: 0464 088d 04a0 0da1 0001 007c 029b 0064  .d.........|...d
-00001640: 027c 019b 0064 079d 047d 0074 036a 1372  .|...d...}.t.j.r
-00001650: 9974 147c 007c 027c 0183 035c 027d 007d  .t.|.|.|...\.}.}
-00001660: 0c7c 05a0 097c 007c 0c67 02a1 0101 007c  .|...|.|.g.....|
-00001670: 007c 047c 057c 0666 0453 0029 094e 7205  .|.|.|.f.S.).Nr.
-00001680: 0000 0072 1200 0000 727b 0000 007a 185f  ...r....r{...z._
-00001690: 6d6f 7469 6f6e 5f63 6f72 7265 6374 6564  motion_corrected
-000016a0: 2e6e 6969 2e67 7a72 4200 0000 7a15 4d6f  .nii.gzrB...z.Mo
-000016b0: 7469 6f6e 2063 6f72 7265 6374 6564 2064  tion corrected d
-000016c0: 6174 617a 105f 736d 6f6f 7468 6564 2e6e  ataz._smoothed.n
-000016d0: 6969 2e67 7a29 0472 4300 0000 da04 6677  ii.gz).rC.....fw
-000016e0: 686d da14 6272 6967 6874 6e65 7373 5f74  hm..brightness_t
-000016f0: 6872 6573 686f 6c64 7244 0000 0029 1572  hresholdrD...).r
-00001700: 2000 0000 7274 0000 0072 4000 0000 721b   ...rt...r@...r.
-00001710: 0000 0072 1c00 0000 725c 0000 0072 7900  ...r....r\...ry.
-00001720: 0000 da06 6170 7065 6e64 da16 7265 6d6f  ....append..remo
-00001730: 7665 5f6d 6f74 696f 6e5f 6f75 746c 6965  ve_motion_outlie
-00001740: 7273 da06 6578 7465 6e64 da11 6d6f 7469  rs..extend..moti
-00001750: 6f6e 5f63 6f72 7265 6374 696f 6e72 0200  on_correctionr..
-00001760: 0000 da07 4d43 464c 4952 5472 4e00 0000  ....MCFLIRTrN...
-00001770: 7277 0000 00da 1173 7061 7469 616c 5f73  rw.....spatial_s
-00001780: 6d6f 6f74 6869 6e67 da05 5355 5341 4eda  moothing..SUSAN.
-00001790: 0e73 6d6f 6f74 6869 6e67 5f66 7768 6dda  .smoothing_fwhm.
-000017a0: 1e73 6d6f 6f74 6869 6e67 5f62 7269 6768  .smoothing_brigh
-000017b0: 746e 6573 735f 7468 7265 7368 6f6c 64da  tness_threshold.
-000017c0: 0f74 656d 706f 7261 6c5f 6669 6c74 6572  .temporal_filter
-000017d0: 7284 0000 0029 0d72 5200 0000 723e 0000  r....).rR...r>..
-000017e0: 0072 2a00 0000 720f 0000 0072 6a00 0000  .r*...r....rj...
-000017f0: 7286 0000 00da 086f 7574 6c69 6572 7372  r......outliersr
-00001800: 3800 0000 7235 0000 00da 126f 7574 6c69  8...r5.....outli
-00001810: 6572 5f74 696d 6570 6f69 6e74 735a 0d6f  er_timepointsZ.o
-00001820: 7574 6c69 6572 5f66 696c 6573 da06 6f75  utlier_files..ou
-00001830: 7470 7574 5a0e 7265 6475 6e64 616e 745f  tputZ.redundant_
-00001840: 6669 6c65 720d 0000 0072 0d00 0000 7210  filer....r....r.
-00001850: 0000 00da 1570 7265 7061 7265 5f73 7461  .....prepare_sta
-00001860: 746d 6170 5f66 696c 6573 af00 0000 7338  tmap_files....s8
-00001870: 0000 0004 0104 0204 010e 031e 0106 0212  ................
-00001880: 010a 0106 0214 010a 010a 0106 0210 0112  ................
-00001890: 0204 010e 0210 0106 020e 010e 0104 ff06  ................
-000018a0: 0110 0106 0210 010e 010c 0272 9800 0000  ...........r....
-000018b0: 6304 0000 0000 0000 0000 0000 000f 0000  c...............
-000018c0: 0008 0000 0043 0000 0073 0201 0000 7c02  .....C...s....|.
-000018d0: 9b00 6401 7c01 9b00 6402 9d04 7d04 7c02  ..d.|...d...}.|.
-000018e0: 9b00 6401 7c01 9b00 6403 9d04 7d05 7c02  ..d.|...d...}.|.
-000018f0: 9b00 6401 7c01 9b00 6404 9d04 7d06 7400  ..d.|...d...}.t.
-00001900: 6a01 7c00 7c04 7c05 7c06 6405 8d04 a002  j.|.|.|.|.d.....
-00001910: a100 0100 7403 7c02 9b00 6401 7c01 9b00  ....t.|...d.|...
-00001920: 6402 9d04 8301 8f0c 7d07 7c07 a004 a100  d.......}.|.....
-00001930: 7d08 5700 6400 0400 0400 8303 0100 6e08  }.W.d.........n.
-00001940: 3100 733c 7701 0100 0100 0100 5900 0100  1.s<w.......Y...
-00001950: 6700 7d09 7405 7c08 8301 4400 5d16 5c02  g.}.t.|...D.].\.
-00001960: 7d0a 7d0b 7c0b a006 6406 6407 a102 a007  }.}.|...d.d.....
-00001970: 6408 a101 7d0c 7c0c 6409 6b03 725d 7c09  d...}.|.d.k.r]|.
-00001980: a008 7c0a a101 0100 7147 7409 a00a 7c00  ..|.....qGt...|.
-00001990: a101 5c02 7d0d 7d0e 740b 6a0c 7c0d 7c09  ..\.}.}.t.j.|.|.
-000019a0: 640a 640b 8d03 7d0d 740d 7c0d 7c0e 7c01  d.d...}.t.|.|.|.
-000019b0: 7c03 640c 8305 7d00 7c00 7c01 740e 7c09  |.d...}.|.|.t.|.
-000019c0: 8301 6702 7c04 7c05 7c06 6703 6603 5300  ..g.|.|.|.g.f.S.
-000019d0: 290d 4e72 1200 0000 7a0d 5f6f 7574 6c69  ).Nr....z._outli
-000019e0: 6572 732e 7478 747a 0c5f 6d65 7472 6963  ers.txtz._metric
-000019f0: 732e 706e 677a 0c5f 6d65 7472 6963 732e  s.pngz._metrics.
-00001a00: 7478 7429 0472 4300 0000 7244 0000 00da  txt).rC...rD....
-00001a10: 0f6f 7574 5f6d 6574 7269 635f 706c 6f74  .out_metric_plot
-00001a20: da11 6f75 745f 6d65 7472 6963 5f76 616c  ..out_metric_val
-00001a30: 7565 7372 0a00 0000 7205 0000 00da 0131  uesr....r......1
-00001a40: 7272 0000 00e9 0300 0000 2901 da04 6178  rr........)...ax
-00001a50: 6973 7a21 5265 6d6f 7665 6420 6d6f 7469  isz!Removed moti
-00001a60: 6f6e 206f 7574 6c69 6572 2074 696d 6570  on outlier timep
-00001a70: 6f69 6e74 7329 0f72 0200 0000 da0e 4d6f  oints).r......Mo
-00001a80: 7469 6f6e 4f75 746c 6965 7273 724e 0000  tionOutliersrN..
-00001a90: 0072 7c00 0000 da09 7265 6164 6c69 6e65  .r|.....readline
-00001aa0: 73da 0965 6e75 6d65 7261 7465 da07 7265  s..enumerate..re
-00001ab0: 706c 6163 65da 0466 696e 6472 8b00 0000  place..findr....
-00001ac0: 7220 0000 0072 7400 0000 da02 6e70 da06  r ...rt.....np..
-00001ad0: 6465 6c65 7465 7277 0000 00da 036c 656e  deleterw.....len
-00001ae0: 290f 7252 0000 0072 3e00 0000 722a 0000  ).rR...r>...r*..
-00001af0: 0072 0f00 0000 5a0c 6f75 746c 6965 725f  .r....Z.outlier_
-00001b00: 6669 6c65 5a0c 6f75 746c 6965 725f 706c  fileZ.outlier_pl
-00001b10: 6f74 5a0e 6f75 746c 6965 725f 7661 6c75  otZ.outlier_valu
-00001b20: 6573 7280 0000 00da 056c 696e 6573 7296  esr......linesr.
-00001b30: 0000 005a 0a74 696d 655f 706f 696e 74da  ...Z.time_point.
-00001b40: 046c 696e 655a 0d6f 7574 6c69 6572 5f63  .lineZ.outlier_c
-00001b50: 6865 636b 7238 0000 0072 3500 0000 720d  heckr8...r5...r.
-00001b60: 0000 0072 0d00 0000 7210 0000 0072 8c00  ...r....r....r..
-00001b70: 0000 d700 0000 732a 0000 0010 0110 0110  ......s*........
-00001b80: 0108 0202 0102 0104 fe06 0216 020a 011c  ................
-00001b90: ff04 0310 0112 0108 010a 0102 800e 0210  ................
-00001ba0: 0110 0318 0272 8c00 0000 6306 0000 0000  .....r....c.....
-00001bb0: 0000 0000 0000 000a 0000 0007 0000 0043  ...............C
-00001bc0: 0000 0073 7800 0000 7c05 6100 7401 a002  ...sx...|.a.t...
-00001bd0: 7c00 a101 7d06 7c01 9b00 6401 7c03 9b00  |...}.|...d.|...
-00001be0: 6401 7c00 9b00 9d05 7d00 7c01 9b00 6401  d.|.....}.|...d.
-00001bf0: 7c02 9b00 9d03 7d02 7400 6a03 7222 7404  |.....}.t.j.r"t.
-00001c00: 6402 7c06 9b00 9d02 8301 0100 7405 7c00  d.|.........t.|.
-00001c10: 7c06 7c02 7c01 8304 5c04 7d00 7d07 7d08  |.|.|...\.}.}.}.
-00001c20: 7d09 7406 7c04 7c00 7c06 7c07 7c02 7c01  }.t.|.|.|.|.|.|.
-00001c30: 8306 0100 7407 7c08 8301 0100 7c09 5300  ....t.|.....|.S.
-00001c40: 2903 4e72 1200 0000 7a18 2020 2020 2020  ).Nr....z.      
-00001c50: 2020 416e 616c 7973 696e 6720 6669 6c65    Analysing file
-00001c60: 3a20 2908 721b 0000 0072 2000 0000 da09  : ).r....r .....
-00001c70: 7374 7269 705f 6578 74da 0776 6572 626f  strip_ext..verbo
-00001c80: 7365 721f 0000 0072 9800 0000 7288 0000  ser....r....r...
-00001c90: 0072 8700 0000 290a 7252 0000 0072 0f00  .r....).rR...r..
-00001ca0: 0000 722a 0000 0072 2900 0000 7228 0000  ..r*...r)...r(..
-00001cb0: 00da 0363 6667 723e 0000 0072 6a00 0000  ...cfgr>...rj...
-00001cc0: 7286 0000 0072 9500 0000 720d 0000 0072  r....r....r....r
-00001cd0: 0d00 0000 7210 0000 00da 1a70 726f 6365  ....r......proce
-00001ce0: 7373 5f66 696c 6573 5f66 6f72 5f73 7461  ss_files_for_sta
-00001cf0: 746d 6170 73f2 0000 0073 1400 0000 0402  tmaps....s......
-00001d00: 0a02 1401 0e01 0602 0e01 1602 1201 0802  ................
-00001d10: 0402 72ab 0000 0063 0400 0000 0000 0000  ..r....c........
-00001d20: 0000 0000 0a00 0000 0a00 0000 4300 0000  ............C...
-00001d30: 7362 0100 0074 006a 0172 0874 02a0 03a1  sb...t.j.r.t....
-00001d40: 007d 046e 0264 007d 0474 006a 0472 1874  .}.n.d.}.t.j.r.t
-00001d50: 0564 0174 006a 069b 0064 027c 019b 009d  .d.t.j...d.|....
-00001d60: 0483 0101 007c 00a0 07a1 0044 005d 865c  .....|.....D.].\
-00001d70: 027d 057d 0674 006a 0472 3574 0564 037c  .}.}.t.j.r5t.d.|
-00001d80: 05a0 0864 04a1 0164 0519 009b 0064 0674  ...d...d.....d.t
-00001d90: 097c 0683 019b 0064 079d 0583 0101 0074  .|.....d.......t
-00001da0: 026a 0a7c 059b 0064 0474 006a 069b 0064  .j.|...d.t.j...d
-00001db0: 089d 0464 0964 0a8d 0201 0074 0b7c 0674  ...d.d.....t.|.t
-00001dc0: 0ca0 0d7c 05a1 0174 0ca0 0d7c 01a1 0174  ...|...t...|...t
-00001dd0: 0ca0 0d7c 02a1 0174 0ca0 0d7c 03a1 0174  ...|...t...|...t
-00001de0: 0ca0 0d74 00a1 0183 067d 0774 006a 0172  ...t.....}.t.j.r
-00001df0: 6774 0e7c 04a0 0f74 107c 07a1 0283 017d  gt.|...t.|.....}
-00001e00: 086e 0874 0e74 0ca0 0f74 107c 07a1 0283  .n.t.t...t.|....
-00001e10: 017d 0874 006a 1172 a274 126a 1364 0b64  .}.t.j.r.t.j.d.d
-00001e20: 0c67 027c 0864 0d8d 02a0 1464 0ca1 017d  .g.|.d.....d...}
-00001e30: 0874 157c 059b 0064 047c 019b 0064 0e9d  .t.|...d.|...d..
-00001e40: 0464 0f83 028f 117d 097c 09a0 167c 086a  .d.....}.|...|.j
-00001e50: 1764 1064 118d 01a1 0101 0057 0064 0004  .d.d.......W.d..
-00001e60: 0004 0083 0301 0071 1c31 0073 9d77 0101  .......q.1.s.w..
-00001e70: 0001 0001 0059 0001 0071 1c74 006a 0172  .....Y...q.t.j.r
-00001e80: af74 026a 187c 0464 1064 128d 0201 0064  .t.j.|.d.d.....d
-00001e90: 0053 0064 0053 0029 134e 7a16 0a53 6561  .S.d.S.).Nz..Sea
-00001ea0: 7263 6869 6e67 2069 6e20 666f 6c64 6572  rching in folder
-00001eb0: 3a20 fa1d 0a53 6176 696e 6720 6f75 7470  : ...Saving outp
-00001ec0: 7574 2069 6e20 6469 7265 6374 6f72 793a  ut in directory:
-00001ed0: 207a 2c0a 4372 6561 7469 6e67 2073 7461   z,.Creating sta
-00001ee0: 7469 7374 6963 616c 206d 6170 7320 666f  tistical maps fo
-00001ef0: 7220 7061 7274 6963 6970 616e 743a 2072  r participant: r
-00001f00: 1200 0000 7272 0000 007a 1d0a 2020 2020  ....rr...z..    
-00001f10: 2020 4372 6561 7469 6e67 2073 7461 746d    Creating statm
-00001f20: 6170 7320 666f 7220 fa06 2066 696c 6573  aps for .. files
-00001f30: 727b 0000 0054 7216 0000 00da 0446 696c  r{...Tr......Fil
-00001f40: 657a 104f 7574 6c69 6572 7320 7265 6d6f  ez.Outliers remo
-00001f50: 7665 6429 02da 0763 6f6c 756d 6e73 7238  ved)...columnsr8
-00001f60: 0000 007a 1f2f 6e75 6d62 6572 5f6f 665f  ...z./number_of_
-00001f70: 6f75 746c 6965 7273 5f72 656d 6f76 6564  outliers_removed
-00001f80: 2e63 7376 da01 7746 2901 da05 696e 6465  .csv..wF)...inde
-00001f90: 78a9 01da 0772 6573 7461 7274 2919 721b  x....restart).r.
-00001fa0: 0000 00da 146d 756c 7469 636f 7265 5f70  .....multicore_p
-00001fb0: 726f 6365 7373 696e 6772 2000 0000 da15  rocessingr .....
-00001fc0: 7374 6172 745f 7072 6f63 6573 7369 6e67  start_processing
-00001fd0: 5f70 6f6f 6c72 a900 0000 721f 0000 0072  _poolr....r....r
-00001fe0: 1c00 0000 da05 6974 656d 7372 6400 0000  ......itemsrd...
-00001ff0: 72a5 0000 0072 2400 0000 da03 7a69 70da  r....r$.....zip.
-00002000: 0969 7465 7274 6f6f 6c73 da06 7265 7065  .itertools..repe
-00002010: 6174 da04 6c69 7374 da07 7374 6172 6d61  at..list..starma
-00002020: 7072 ab00 0000 728c 0000 0072 6500 0000  pr....r....re...
-00002030: da09 4461 7461 4672 616d 65da 0b73 6f72  ..DataFrame..sor
-00002040: 745f 7661 6c75 6573 727c 0000 0072 7e00  t_valuesr|...r~.
-00002050: 0000 da06 746f 5f63 7376 da14 6a6f 696e  ....to_csv..join
-00002060: 5f70 726f 6365 7373 696e 675f 706f 6f6c  _processing_pool
-00002070: 290a 722e 0000 0072 2a00 0000 7229 0000  ).r....r*...r)..
-00002080: 0072 2800 0000 da04 706f 6f6c 722c 0000  .r(.....poolr,..
-00002090: 00da 0566 696c 6573 da08 6974 6572 6162  ...files..iterab
-000020a0: 6c65 7295 0000 0072 8000 0000 720d 0000  ler....r....r...
-000020b0: 0072 0d00 0000 7210 0000 00da 1a63 616c  .r....r......cal
-000020c0: 6375 6c61 7465 5f73 7461 7469 7374 6963  culate_statistic
-000020d0: 616c 5f6d 6170 7305 0100 0073 4000 0000  al_maps....s@...
-000020e0: 0601 0a01 0402 0602 0c01 0201 08ff 1003  ................
-000020f0: 0601 1401 0601 0aff 1c03 0402 0801 0801  ................
-00002100: 0801 0801 0801 04fb 0607 1201 1002 0602  ................
-00002110: 1801 1802 1401 1cff 0280 0603 1201 04ff  ................
-00002120: 72c3 0000 0063 0400 0000 0000 0000 0000  r....c..........
-00002130: 0000 0900 0000 0900 0000 4300 0000 73ec  ..........C...s.
-00002140: 0000 0074 006a 0172 0874 02a0 03a1 007d  ...t.j.r.t.....}
-00002150: 046e 0264 007d 0474 006a 0472 1874 0564  .n.d.}.t.j.r.t.d
-00002160: 0174 006a 069b 0064 027c 019b 009d 0483  .t.j...d.|......
-00002170: 0101 007c 00a0 07a1 0044 005d 4b5c 027d  ...|.....D.]K\.}
-00002180: 057d 067c 059b 0064 027c 029b 009d 037d  .}.|...d.|.....}
-00002190: 0774 006a 0472 3f74 0564 037c 039b 0064  .t.j.r?t.d.|...d
-000021a0: 047c 07a0 0864 02a1 0164 0519 009b 0064  .|...d...d.....d
-000021b0: 0674 097c 0683 019b 0064 079d 0783 0101  .t.|.....d......
-000021c0: 0074 0a7c 0674 0ba0 0c7c 07a1 0174 0ba0  .t.|.t...|...t..
-000021d0: 0c7c 01a1 0174 0ba0 0c7c 03a1 0174 0ba0  .|...t...|...t..
-000021e0: 0c74 00a1 0183 057d 0874 006a 0172 5f74  .t.....}.t.j.r_t
-000021f0: 0d7c 04a0 0e74 0f7c 08a1 0283 0101 0071  .|...t.|.......q
-00002200: 1c74 0d74 0ba0 0e74 0f7c 08a1 0283 0101  .t.t...t.|......
-00002210: 0071 1c74 006a 0172 7474 026a 107c 0464  .q.t.j.rtt.j.|.d
-00002220: 0864 098d 0201 0064 0053 0064 0053 0029  .d.....d.S.d.S.)
-00002230: 0a4e 72ac 0000 0072 1200 0000 7a0a 0a52  .Nr....r....z..R
-00002240: 756e 6e69 6e67 2027 7a1a 2720 7574 696c  unning 'z.' util
-00002250: 6974 7920 6f6e 2070 6172 7469 6369 7061  ity on participa
-00002260: 6e74 3a20 e9fe ffff ff7a 1a0a 2020 2020  nt: .....z..    
-00002270: 2020 5275 6e6e 696e 6720 7574 696c 6974    Running utilit
-00002280: 7920 6f6e 2072 ad00 0000 4672 b200 0000  y on r....Fr....
-00002290: 2911 721b 0000 0072 b400 0000 7220 0000  ).r....r....r ..
-000022a0: 0072 b500 0000 72a9 0000 0072 1f00 0000  .r....r....r....
-000022b0: 721c 0000 0072 b600 0000 7264 0000 0072  r....r....rd...r
-000022c0: a500 0000 72b7 0000 0072 b800 0000 72b9  ....r....r....r.
-000022d0: 0000 0072 ba00 0000 72bb 0000 00da 0b72  ...r....r......r
-000022e0: 756e 5f75 7469 6c69 7479 72bf 0000 0029  un_utilityr....)
-000022f0: 0972 2e00 0000 722a 0000 0072 2900 0000  .r....r*...r)...
-00002300: 7228 0000 0072 c000 0000 720f 0000 0072  r(...r....r....r
-00002310: c100 0000 722c 0000 0072 c200 0000 720d  ....r,...r....r.
-00002320: 0000 0072 0d00 0000 7210 0000 00da 1670  ...r....r......p
-00002330: 7265 7061 7265 5f74 6f5f 7275 6e5f 7574  repare_to_run_ut
-00002340: 696c 6974 792c 0100 0073 2e00 0000 0601  ility,...s......
-00002350: 0a01 0402 0602 1601 1002 0e01 0602 1a01  ................
-00002360: 0601 0aff 0403 0801 0801 0801 0801 04fc  ................
-00002370: 0606 1201 1203 0602 1201 04ff 72c6 0000  ............r...
-00002380: 0063 0500 0000 0000 0000 0000 0000 0a00  .c..............
-00002390: 0000 0600 0000 4300 0000 73a0 0000 007c  ......C...s....|
-000023a0: 0461 0074 01a0 027c 00a1 017d 057c 019b  .a.t...|...}.|..
-000023b0: 0064 017c 009b 009d 037d 0074 037c 0183  .d.|.....}.t.|..
-000023c0: 016a 0464 0219 007d 0674 056a 06a0 0774  .j.d...}.t.j...t
-000023d0: 037c 0183 016a 0464 0319 00a1 0164 0219  .|...j.d.....d..
-000023e0: 007d 0774 006a 0872 2c74 0964 047c 059b  .}.t.j.r,t.d.|..
-000023f0: 009d 0283 0101 007c 0364 056b 0272 4e74  .......|.d.k.rNt
-00002400: 0aa0 0b7c 069b 0064 069d 02a1 017d 0874  ...|...d.....}.t
-00002410: 0c7c 087c 0864 0719 007c 076b 0219 0064  .|.|.d...|.k...d
-00002420: 0819 0083 017d 0974 0d7c 007c 057c 017c  .....}.t.|.|.|.|
-00002430: 027c 0983 0501 0064 0053 0064 0053 0029  .|.....d.S.d.S.)
-00002440: 094e 7212 0000 0072 0300 0000 7201 0000  .Nr....r....r...
-00002450: 007a 2120 2020 2020 2020 2052 756e 6e69  .z!        Runni
-00002460: 6e67 2075 7469 6c69 7479 206f 6e20 6669  ng utility on fi
-00002470: 6c65 3a20 7209 0000 0072 5800 0000 7259  le: r....rX...rY
-00002480: 0000 007a 0f4e 6f69 7365 206f 7665 7220  ...z.Noise over 
-00002490: 7469 6d65 290e 721b 0000 0072 2000 0000  time).r....r ...
-000024a0: 72a8 0000 0072 6000 0000 7261 0000 0072  r....r`...ra...r
-000024b0: 6200 0000 7263 0000 0072 6400 0000 72a9  b...rc...rd...r.
-000024c0: 0000 0072 1f00 0000 7265 0000 0072 6600  ...r....re...rf.
-000024d0: 0000 7267 0000 00da 1161 6464 5f6e 6f69  ..rg.....add_noi
-000024e0: 7365 5f74 6f5f 6669 6c65 290a 7252 0000  se_to_file).rR..
-000024f0: 0072 2c00 0000 722a 0000 0072 2800 0000  .r,...r*...r(...
-00002500: 72aa 0000 0072 3e00 0000 722b 0000 0072  r....r>...r+...r
-00002510: 6c00 0000 726d 0000 00da 1770 6172 7469  l...rm.....parti
-00002520: 6369 7061 6e74 5f6e 6f69 7365 5f6c 6576  cipant_noise_lev
-00002530: 656c 720d 0000 0072 0d00 0000 7210 0000  elr....r....r...
-00002540: 0072 c500 0000 4c01 0000 731c 0000 0004  .r....L...s.....
-00002550: 020a 020e 010e 011a 0106 020e 0108 0210  ................
-00002560: 0102 0112 0104 ff14 0204 fc72 c500 0000  ...........r....
-00002570: 6305 0000 0000 0000 0000 0000 000a 0000  c...............
-00002580: 0008 0000 0043 0000 0073 8c00 0000 7400  .....C...s....t.
-00002590: a001 7c00 a101 5c02 7d05 7d06 7402 7c05  ..|...\.}.}.t.|.
-000025a0: 6401 7c01 7c02 9b00 6402 7c03 9b00 9d03  d.|.|...d.|.....
-000025b0: 7c06 6403 8d05 0100 7403 6a04 4400 5d2b  |.d.....t.j.D.]+
-000025c0: 7d07 7405 6a06 a007 a100 6a08 6404 7c04  }.t.j.....j.d.|.
-000025d0: 7c07 1400 7c05 6a09 6405 8d03 7d08 7c05  |...|.j.d...}.|.
-000025e0: 7c08 1700 7d09 6406 7c09 7c09 6406 6b00  |...}.d.|.|.d.k.
-000025f0: 3c00 7402 7c09 6407 7c07 9b00 9d02 7c01  <.t.|.d.|.....|.
-00002600: 7c02 9b00 6402 7c03 9b00 9d03 7c06 6403  |...d.|.....|.d.
-00002610: 8d05 0100 7118 6400 5300 2908 4e5a 0c5f  ....q.d.S.).NZ._
-00002620: 6e6f 6973 656c 6576 656c 3072 1200 0000  noiselevel0r....
-00002630: 2904 723d 0000 0072 3e00 0000 722a 0000  ).r=...r>...r*..
-00002640: 0072 3500 0000 6700 0000 0000 0000 0029  .r5...g........)
-00002650: 03da 036c 6f63 da05 7363 616c 65da 0473  ...loc..scale..s
-00002660: 697a 6572 0100 0000 5a0b 5f6e 6f69 7365  izer....Z._noise
-00002670: 6c65 7665 6c29 0a72 2000 0000 7274 0000  level).r ...rt..
-00002680: 0072 4000 0000 721b 0000 00da 116e 6f69  .r@...r......noi
-00002690: 7365 5f6d 756c 7469 706c 6965 7273 72a3  se_multipliersr.
-000026a0: 0000 00da 0672 616e 646f 6dda 0b64 6566  .....random..def
-000026b0: 6175 6c74 5f72 6e67 da06 6e6f 726d 616c  ault_rng..normal
-000026c0: da05 7368 6170 6529 0a72 5200 0000 723e  ..shape).rR...r>
-000026d0: 0000 0072 2c00 0000 722a 0000 0072 c800  ...r,...r*...r..
-000026e0: 0000 7238 0000 0072 3500 0000 da0a 6d75  ..r8...r5.....mu
-000026f0: 6c74 6970 6c69 6572 5a0e 6761 7573 7369  ltiplierZ.gaussi
-00002700: 616e 5f6e 6f69 7365 5a0a 6e6f 6973 795f  an_noiseZ.noisy_
-00002710: 6461 7461 720d 0000 0072 0d00 0000 7210  datar....r....r.
-00002720: 0000 0072 c700 0000 5f01 0000 731e 0000  ...r...._...s...
-00002730: 000e 0108 030e 0106 ff0a 030c 0106 0104  ................
-00002740: 0106 fe08 040c 010e 020e 0108 ff04 f872  ...............r
-00002750: c700 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00002760: 0008 0000 0005 0000 0043 0000 0073 e400  .........C...s..
-00002770: 0000 7400 a000 a100 7d04 7401 a002 7c01  ..t.....}.t...|.
-00002780: a101 0100 7403 7404 6a05 a006 7407 a101  ....t.t.j...t...
-00002790: 8301 6a08 6401 1900 9b00 6402 9d02 6109  ..j.d.....d...a.
-000027a0: 7c02 610a 7401 6a0b 7409 7c02 7c03 6403  |.a.t.j.t.|.|.d.
-000027b0: 8d03 610c 740c 6a0d 722c 740e 6404 7c00  ..a.t.j.r,t.d.|.
-000027c0: 9b00 6405 9d03 8301 0100 740f a010 6406  ..d.......t...d.
-000027d0: a101 a011 6407 a101 0100 7c00 6408 6b02  ....d.....|.d.k.
-000027e0: 7242 740c 6a12 7342 740c 6a0d 7242 740e  rBt.j.sBt.j.rBt.
-000027f0: 6409 8301 0100 7413 7c00 8301 5c03 7d05  d.....t.|...\.}.
-00002800: 7d06 7d07 7c00 640a 7600 7255 7414 7c05  }.}.|.d.v.rUt.|.
-00002810: 7c06 7c07 7c00 8304 0100 6e07 7415 7c05  |.|.|.....n.t.|.
-00002820: 7c06 7c07 7c00 8304 0100 740c 6a0d 7270  |.|.|.....t.j.rp
-00002830: 740e 640b 7416 7400 a000 a100 7c04 1800  t.d.t.t.....|...
-00002840: 640c 8302 9b00 640d 9d03 8301 0100 6400  d.....d.......d.
-00002850: 5300 6400 5300 290e 4e72 0300 0000 7a1d  S.d.S.).Nr....z.
-00002860: 2f63 6f6e 6669 6775 7261 7469 6f6e 5f70  /configuration_p
-00002870: 726f 6669 6c65 732f 6d61 7073 2f29 0172  rofiles/maps/).r
-00002880: 6300 0000 7a6e 0a2d 2d2d 2d2d 2d2d 2d2d  c...zn.---------
-00002890: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000028a0: 2d2d 2d2d 2d2d 2d0a 2d2d 2d20 5374 6174  -------.--- Stat
-000028b0: 6973 7469 6361 6c20 6d61 7020 6372 6561  istical map crea
-000028c0: 7469 6f6e 202d 2d2d 0a2d 2d2d 2d2d 2d2d  tion ---.-------
-000028d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000028e0: 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 7265 6174  ---------..Creat
-000028f0: 696e 6720 7a07 206d 6170 732e 0a7a 0f6e  ing z. maps..z.n
-00002900: 6970 7970 652e 776f 726b 666c 6f77 7201  ipype.workflowr.
-00002910: 0000 0072 0700 0000 7ac4 224e 6f69 7365  ...r....z."Noise
-00002920: 2076 6f6c 756d 6520 696e 636c 7564 6564   volume included
-00002930: 2069 6e20 7469 6d65 2073 6572 6965 7322   in time series"
-00002940: 2069 7320 6661 6c73 652e 2054 7279 696e   is false. Tryin
-00002950: 6720 746f 2066 696e 6420 7661 6c75 6573  g to find values
-00002960: 2066 6f72 2065 6163 6820 7061 7274 6963   for each partic
-00002970: 6970 616e 7420 696e 206e 6f69 7365 5661  ipant in noiseVa
-00002980: 6c75 6573 2e63 7376 2069 6e73 7465 6164  lues.csv instead
-00002990: 2e20 4966 2074 6869 7320 6973 206e 6f74  . If this is not
-000029a0: 2063 6f72 7265 6374 2c20 7365 7420 224e   correct, set "N
-000029b0: 6f69 7365 2076 6f6c 756d 6520 696e 636c  oise volume incl
-000029c0: 7564 6564 2069 6e20 7469 6d65 2073 6572  uded in time ser
-000029d0: 6965 7322 2074 6f20 7472 7565 2e0a 2901  ies" to true..).
-000029e0: 7209 0000 007a 120a 2d2d 2d20 436f 6d70  r....z..--- Comp
-000029f0: 6c65 7465 6420 696e 2072 3200 0000 7a0e  leted in r2...z.
-00002a00: 2073 6563 6f6e 6473 202d 2d2d 0a0a 2917   seconds ---..).
-00002a10: da04 7469 6d65 7220 0000 00da 0c63 6865  ..timer .....che
-00002a20: 636b 7665 7273 696f 6e72 6000 0000 7262  ckversionr`...rb
-00002a30: 0000 0072 6300 0000 da07 6162 7370 6174  ...rc.....abspat
-00002a40: 68da 085f 5f66 696c 655f 5f72 6100 0000  h..__file__ra...
-00002a50: 7226 0000 0072 2700 0000 da0b 6c6f 6164  r&...r'.....load
-00002a60: 5f63 6f6e 6669 6772 1b00 0000 72a9 0000  _configr....r...
-00002a70: 0072 1f00 0000 da07 6c6f 6767 696e 67da  .r......logging.
-00002a80: 0967 6574 4c6f 6767 6572 da08 7365 744c  .getLogger..setL
-00002a90: 6576 656c 725c 0000 0072 2f00 0000 72c6  evelr\...r/...r.
-00002aa0: 0000 0072 c300 0000 da05 726f 756e 6429  ...r......round)
-00002ab0: 0872 2800 0000 da07 7665 7273 696f 6eda  .r(.....version.
-00002ac0: 0b63 6f6e 6669 675f 6669 6c65 7263 0000  .config_filerc..
-00002ad0: 00da 0a73 7461 7274 5f74 696d 6572 2e00  ...start_timer..
-00002ae0: 0000 722a 0000 0072 2900 0000 720d 0000  ..r*...r)...r...
-00002af0: 0072 0d00 0000 7210 0000 00da 046d 6169  .r....r......mai
-00002b00: 6e72 0100 0073 2600 0000 0803 0a01 1c03  nr...s&.........
-00002b10: 0401 1003 0602 0401 0203 0afd 1005 1402  ................
-00002b20: 0801 0e03 0802 1001 0e03 0602 2201 04ff  ............"...
-00002b30: 72de 0000 0072 0c00 0000 291e 72b8 0000  r....r....).r...
-00002b40: 00da 056e 756d 7079 72a3 0000 005a 116e  ...numpyr....Z.n
-00002b50: 6970 7970 652e 696e 7465 7266 6163 6573  ipype.interfaces
-00002b60: 7202 0000 0072 d700 0000 72d2 0000 00da  r....r....r.....
-00002b70: 0575 7469 6c73 721b 0000 0072 2600 0000  .utilsr....r&...
-00002b80: 7227 0000 0072 2f00 0000 723a 0000 0072  r'...r/...r:...r
-00002b90: 4000 0000 7253 0000 0072 6e00 0000 7268  @...rS...rn...rh
-00002ba0: 0000 0072 7900 0000 7277 0000 0072 8400  ...ry...rw...r..
-00002bb0: 0000 7287 0000 0072 8800 0000 7298 0000  ..r....r....r...
-00002bc0: 0072 8c00 0000 72ab 0000 0072 c300 0000  .r....r....r....
-00002bd0: 72c6 0000 0072 c500 0000 72c7 0000 0072  r....r....r....r
-00002be0: de00 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
-00002bf0: 0000 0072 1000 0000 da08 3c6d 6f64 756c  ...r......<modul
-00002c00: 653e 0100 0000 7338 0000 0008 0008 020c  e>....s8........
-00002c10: 0108 0108 0108 0204 0204 0104 0108 0308  ................
-00002c20: 270a 0808 0708 0f08 1e08 0408 1208 0a08  '...............
-00002c30: 1108 0508 0708 2808 1b08 1308 2708 2008  ......(.....'. .
-00002c40: 130e 13                                  ...
+00000060: 6d08 5a08 0100 6405 6406 6c09 5400 6401  m.Z...d.d.l.T.d.
+00000070: 610a 6407 610b 6407 610c 6408 6409 8400  a.d.a.d.a.d.d...
+00000080: 5a0d 640a 640b 8400 5a0e 640c 640d 8400  Z.d.d...Z.d.d...
+00000090: 5a0f 640e 640f 8400 5a10 6410 6411 8400  Z.d.d...Z.d.d...
+000000a0: 5a11 6412 6413 8400 5a12 6414 6415 8400  Z.d.d...Z.d.d...
+000000b0: 5a13 6416 6417 8400 5a14 6418 6419 8400  Z.d.d...Z.d.d...
+000000c0: 5a15 641a 641b 8400 5a16 641c 641d 8400  Z.d.d...Z.d.d...
+000000d0: 5a17 641e 641f 8400 5a18 6420 6421 8400  Z.d.d...Z.d d!..
+000000e0: 5a19 6424 6422 6423 8401 5a1a 6401 5300  Z.d$d"d#..Z.d.S.
+000000f0: 2925 e900 0000 004e 2901 da03 6673 6ce9  )%.....N)...fsl.
+00000100: 0200 0000 2901 da05 484f 5553 45e9 0100  ....)...HOUSE...
+00000110: 0000 2901 da01 2ada 0063 0100 0000 0000  ..)...*..c......
+00000120: 0000 0000 0000 0800 0000 0800 0000 4300  ..............C.
+00000130: 0000 73fc 0000 0074 006a 017d 0174 006a  ..s....t.j.}.t.j
+00000140: 0264 016b 0372 0f64 0274 006a 029b 009d  .d.k.r.d.t.j....
+00000150: 027d 026e 0d7c 0064 036b 0272 1664 047d  .}.n.|.d.k.r.d.}
+00000160: 026e 067c 0064 056b 0272 1c64 067d 0274  .n.|.d.k.r.d.}.t
+00000170: 006a 0364 0776 0072 2c74 0464 0883 0101  .j.d.v.r,t.d....
+00000180: 0074 056a 0664 0964 0a8d 017d 036e 0374  .t.j.d.d...}.n.t
+00000190: 006a 037d 0374 05a0 077c 03a1 015c 027d  .j.}.t...|...\.}
+000001a0: 047d 0564 0b64 0c84 007c 0444 0083 017d  .}.d.d...|.D...}
+000001b0: 067c 0644 005d 397d 0774 05a0 087c 079b  .|.D.]9}.t...|..
+000001c0: 0064 0d7c 019b 009d 0364 0e64 0f64 10a1  .d.|.....d.d.d..
+000001d0: 047c 067c 073c 0074 05a0 097c 079b 0064  .|.|.<.t...|...d
+000001e0: 119d 02a1 0101 0074 056a 097c 079b 0064  .......t.j.|...d
+000001f0: 0d7c 029b 009d 0364 1264 138d 0201 0074  .|.....d.d.....t
+00000200: 056a 0a7c 079b 0064 0d7c 029b 009d 0374  .j.|...d.|.....t
+00000210: 0b74 0c64 147c 009b 0064 159d 0367 0164  .t.d.|...d...g.d
+00000220: 1664 178d 0501 0071 3f7c 067c 027c 0166  .d.....q?|.|.|.f
+00000230: 0353 0029 184e da07 4445 4641 554c 547a  .S.).N..DEFAULTz
+00000240: 0973 7461 746d 6170 732f fa09 496d 6167  .statmaps/..Imag
+00000250: 6520 534e 527a 1873 7461 746d 6170 732f  e SNRz.statmaps/
+00000260: 696d 6167 6553 4e52 5f72 6570 6f72 74fa  imageSNR_report.
+00000270: 0c54 656d 706f 7261 6c20 534e 527a 1b73  .Temporal SNRz.s
+00000280: 7461 746d 6170 732f 7465 6d70 6f72 616c  tatmaps/temporal
+00000290: 534e 525f 7265 706f 7274 2902 7207 0000  SNR_report).r...
+000002a0: 00fa 0120 7a38 5365 6c65 6374 2074 6865  ... z8Select the
+000002b0: 2064 6972 6563 746f 7279 2077 6869 6368   directory which
+000002c0: 2063 6f6e 7461 696e 7320 7468 6520 7375   contains the su
+000002d0: 626a 6563 7420 666f 6c64 6572 732e 7a37  bject folders.z7
+000002e0: 5365 6c65 6374 2074 6865 2064 6972 6563  Select the direc
+000002f0: 746f 7279 2077 6869 6368 2063 6f6e 7461  tory which conta
+00000300: 696e 7320 7468 6520 7375 626a 6563 7420  ins the subject 
+00000310: 666f 6c64 6572 7329 01da 0574 6974 6c65  folders)...title
+00000320: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000330: 0004 0000 0053 0000 0073 1200 0000 6900  .....S...s....i.
+00000340: 7c00 5d05 7d01 7c01 6400 9302 7102 5300  |.].}.|.d...q.S.
+00000350: a901 4ea9 0029 02da 022e 30da 0b70 6172  ..N..)....0..par
+00000360: 7469 6369 7061 6e74 720e 0000 0072 0e00  ticipantr....r..
+00000370: 0000 fa52 2f55 7365 7273 2f6c 7078 6568  ...R/Users/lpxeh
+00000380: 3130 2f44 6f63 756d 656e 7473 2f52 6570  10/Documents/Rep
+00000390: 6f73 6974 6f72 6965 732f 664d 5249 5f52  ositories/fMRI_R
+000003a0: 4f49 5f61 6e61 6c79 7369 735f 746f 6f6c  OI_analysis_tool
+000003b0: 2f66 5241 542f 7574 696c 732f 7374 6174  /fRAT/utils/stat
+000003c0: 6d61 702e 7079 da0a 3c64 6963 7463 6f6d  map.py..<dictcom
+000003d0: 703e 2300 0000 7302 0000 0012 007a 2673  p>#...s......z&s
+000003e0: 7461 746d 6170 5f66 696c 655f 7365 7475  tatmap_file_setu
+000003f0: 702e 3c6c 6f63 616c 733e 2e3c 6469 6374  p.<locals>.<dict
+00000400: 636f 6d70 3efa 012f da03 6864 727a 066e  comp>../..hdrz.n
+00000410: 6969 2e67 7ada 036e 6969 7a09 2f73 7461  ii.gz..niiz./sta
+00000420: 746d 6170 7354 a901 da0a 6465 6c65 7465  tmapsT....delete
+00000430: 5f6f 6c64 7a1b 7374 6174 6973 7469 6361  _oldz.statistica
+00000440: 6c5f 6d61 705f 6372 6561 7465 6420 3d20  l_map_created = 
+00000450: 277a 0227 0ada 0e73 7461 746d 6170 5f63  'z.'...statmap_c
+00000460: 6f6e 6669 6729 02da 0f61 6464 6974 696f  onfig)...additio
+00000470: 6e61 6c5f 696e 666f da0f 6e65 775f 636f  nal_info..new_co
+00000480: 6e66 6967 5f6e 616d 6529 0dda 0663 6f6e  nfig_name)...con
+00000490: 6669 67da 1169 6e70 7574 5f66 6f6c 6465  fig..input_folde
+000004a0: 725f 6e61 6d65 da12 6f75 7470 7574 5f66  r_name..output_f
+000004b0: 6f6c 6465 725f 6e61 6d65 da0b 6261 7365  older_name..base
+000004c0: 5f66 6f6c 6465 72da 0570 7269 6e74 da05  _folder..print..
+000004d0: 5574 696c 73da 0c66 696c 655f 6272 6f77  Utils..file_brow
+000004e0: 7365 72da 1566 696e 645f 7061 7274 6963  ser..find_partic
+000004f0: 6970 616e 745f 6469 7273 da0a 6669 6e64  ipant_dirs..find
+00000500: 5f66 696c 6573 da12 6368 6563 6b5f 616e  _files..check_an
+00000510: 645f 6d61 6b65 5f64 6972 da0b 7361 7665  d_make_dir..save
+00000520: 5f63 6f6e 6669 67da 0b63 6f6e 6669 675f  _config..config_
+00000530: 7061 7468 da0f 636f 6e66 6967 5f66 696c  path..config_fil
+00000540: 656e 616d 6529 08da 0466 756e 63da 0d66  ename)...func..f
+00000550: 696c 655f 6c6f 6361 7469 6f6e da0d 6f75  ile_location..ou
+00000560: 7470 7574 5f66 6f6c 6465 72da 1162 6173  tput_folder..bas
+00000570: 655f 7375 625f 6c6f 6361 7469 6f6e da0f  e_sub_location..
+00000580: 7061 7274 6963 6970 616e 745f 6469 72da  participant_dir.
+00000590: 015f da0c 7061 7274 6963 6970 616e 7473  ._..participants
+000005a0: 7210 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+000005b0: 1100 0000 da12 7374 6174 6d61 705f 6669  ......statmap_fi
+000005c0: 6c65 5f73 6574 7570 1000 0000 732c 0000  le_setup....s,..
+000005d0: 0006 010a 020e 0108 0106 0108 0104 010a  ................
+000005e0: 0208 010e 0106 030e 030e 0108 021e 0210  ................
+000005f0: 0218 0114 010c 0102 0108 fe0a 0472 2f00  .............r/.
+00000600: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
+00000610: 0000 0003 0000 0043 0000 0073 2a00 0000  .......C...s*...
+00000620: 7400 a001 7c00 a101 7d01 7c01 6a02 6401  t...|...}.|.j.d.
+00000630: 1900 6402 1900 7d02 6403 6404 7403 6a04  ..d...}.d.d.t.j.
+00000640: 1400 7c02 1400 1b00 5300 2905 4eda 0670  ..|.....S.).N..p
+00000650: 6978 6469 6de9 0400 0000 7205 0000 0072  ixdim.....r....r
+00000660: 0300 0000 2905 da03 6e69 62da 046c 6f61  ....)...nib..loa
+00000670: 64da 0668 6561 6465 7272 1b00 0000 da16  d..headerr......
+00000680: 6869 6768 7061 7373 5f66 696c 7465 725f  highpass_filter_
+00000690: 6375 746f 6666 2903 da09 6669 6c65 5f70  cutoff)...file_p
+000006a0: 6174 68da 0464 6174 61da 0254 5272 0e00  ath..data..TRr..
+000006b0: 0000 720e 0000 0072 1100 0000 da1a 6361  ..r....r......ca
+000006c0: 6c63 756c 6174 655f 7369 676d 615f 696e  lculate_sigma_in
+000006d0: 5f76 6f6c 756d 6573 3200 0000 7306 0000  _volumes2...s...
+000006e0: 000a 010e 0112 0372 3900 0000 6303 0000  .......r9...c...
+000006f0: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+00000700: 0043 0000 0073 b000 0000 7400 6a01 6a02  .C...s....t.j.j.
+00000710: 7c00 7c02 9b00 6401 7c01 9b00 6402 9d04  |.|...d.|...d...
+00000720: 6403 8d02 a003 a100 0100 7400 6a01 6a04  d.........t.j.j.
+00000730: 7c00 7c02 9b00 6401 7c01 9b00 6404 9d04  |.|...d.|...d...
+00000740: 6403 8d02 a003 a100 0100 7400 6a01 6a05  d.........t.j.j.
+00000750: 6405 7c02 9b00 6401 7c01 9b00 6402 9d04  d.|...d.|...d...
+00000760: 7c02 9b00 6401 7c01 9b00 6404 9d04 7c02  |...d.|...d...|.
+00000770: 9b00 6401 7c01 9b00 6406 9d04 6407 8d04  ..d.|...d...d...
+00000780: a003 a100 0100 7400 6a01 6a06 7c02 9b00  ......t.j.j.|...
+00000790: 6401 7c01 9b00 6406 9d04 6408 6409 7c02  d.|...d...d.d.|.
+000007a0: 9b00 6401 7c01 9b00 6406 9d04 640a 8d04  ..d.|...d...d...
+000007b0: a003 a100 0100 6400 5300 290b 4e72 1300  ......d.S.).Nr..
+000007c0: 0000 fa0d 5f74 4d65 616e 2e6e 6969 2e67  ...._tMean.nii.g
+000007d0: 7aa9 02da 0769 6e5f 6669 6c65 da08 6f75  z....in_file..ou
+000007e0: 745f 6669 6c65 7a0c 5f74 5374 642e 6e69  t_filez._tStd.ni
+000007f0: 692e 677a da03 6469 767a 0c5f 7453 4e52  i.gz..divz._tSNR
+00000800: 2e6e 6969 2e67 7aa9 04da 096f 7065 7261  .nii.gz....opera
+00000810: 7469 6f6e 723c 0000 00da 0c6f 7065 7261  tionr<.....opera
+00000820: 6e64 5f66 696c 6572 3d00 0000 6700 0000  nd_filer=...g...
+00000830: 0000 408f 40da 0561 626f 7665 2904 723c  ..@.@..above).r<
+00000840: 0000 00da 0674 6872 6573 68da 0964 6972  .....thresh..dir
+00000850: 6563 7469 6f6e 723d 0000 0029 0772 0200  ectionr=...).r..
+00000860: 0000 da05 6d61 7468 73da 094d 6561 6e49  ....maths..MeanI
+00000870: 6d61 6765 da03 7275 6eda 0853 7464 496d  mage..run..StdIm
+00000880: 6167 65da 0b42 696e 6172 794d 6174 6873  age..BinaryMaths
+00000890: da09 5468 7265 7368 6f6c 6429 03da 0466  ..Threshold)...f
+000008a0: 696c 65da 0b6e 6f5f 6578 745f 6669 6c65  ile..no_ext_file
+000008b0: 722a 0000 0072 0e00 0000 720e 0000 0072  r*...r....r....r
+000008c0: 1100 0000 da10 7465 6d70 6f72 616c 534e  ......temporalSN
+000008d0: 525f 6361 6c63 3a00 0000 731c 0000 0020  R_calc:...s.... 
+000008e0: 0108 020e 0104 ff06 0116 030e 010e 0104  ................
+000008f0: fe06 0218 030e 0104 ff0a 0172 4d00 0000  ...........rM...
+00000900: 6305 0000 0000 0000 0000 0000 000b 0000  c...............
+00000910: 0008 0000 0043 0000 0073 f200 0000 7400  .....C...s....t.
+00000920: 6a01 6a02 7c00 7c03 9b00 6401 7c02 9b00  j.j.|.|...d.|...
+00000930: 6402 9d04 6403 8d02 a003 a100 0100 7404  d...d.........t.
+00000940: 6a05 722b 7406 a007 7c01 a101 5c02 7d05  j.r+t...|...\.}.
+00000950: 7d06 7404 6a08 7226 7c05 7c05 6404 6b03  }.t.j.r&|.|.d.k.
+00000960: 1900 a009 a100 7d07 6e2a 7c05 a009 a100  ......}.n*|.....
+00000970: 7d07 6e25 740a 7c04 8301 6a0b 6404 1900  }.n%t.|...j.d...
+00000980: 7d08 740c 6a0d a00e 740a 7c04 8301 a101  }.t.j...t.|.....
+00000990: 6405 1900 7d09 740f a010 7c08 9b00 6406  d...}.t...|...d.
+000009a0: 9d02 a101 7d0a 7411 7c0a 7c0a 6407 1900  ....}.t.|.|.d...
+000009b0: 7c09 6b02 1900 6408 1900 8301 7d07 7400  |.k...d.....}.t.
+000009c0: 6a01 6a12 6409 7c03 9b00 6401 7c02 9b00  j.j.d.|...d.|...
+000009d0: 6402 9d04 7c07 7c03 9b00 6401 7c02 9b00  d...|.|...d.|...
+000009e0: 640a 9d04 640b 8d04 a003 a100 0100 7404  d...d.........t.
+000009f0: 6a13 7277 7413 7c03 9b00 6401 7c02 9b00  j.rwt.|...d.|...
+00000a00: 640a 9d04 8301 0100 6400 5300 6400 5300  d.......d.S.d.S.
+00000a10: 290c 4e72 1300 0000 723a 0000 0072 3b00  ).Nr....r:...r;.
+00000a20: 0000 7201 0000 0072 0500 0000 7a10 2f6e  ..r....r....z./n
+00000a30: 6f69 7365 5661 6c75 6573 2e63 7376 da0b  oiseValues.csv..
+00000a40: 5061 7274 6963 6970 616e 747a 1042 6163  Participantz.Bac
+00000a50: 6b67 726f 756e 6420 6e6f 6973 6572 3e00  kground noiser>.
+00000a60: 0000 7a0c 5f69 534e 522e 6e69 692e 677a  ..z._iSNR.nii.gz
+00000a70: 2904 7240 0000 0072 3c00 0000 da0d 6f70  ).r@...r<.....op
+00000a80: 6572 616e 645f 7661 6c75 6572 3d00 0000  erand_valuer=...
+00000a90: 2914 7202 0000 0072 4500 0000 7246 0000  ).r....rE...rF..
+00000aa0: 0072 4700 0000 721b 0000 00da 0c6e 6f69  .rG...r......noi
+00000ab0: 7365 5f76 6f6c 756d 6572 2000 0000 da0a  se_volumer .....
+00000ac0: 6c6f 6164 5f62 7261 696e da20 6953 4e52  load_brain. iSNR
+00000ad0: 5f73 7464 5f75 7365 5f6f 6e6c 795f 6e6f  _std_use_only_no
+00000ae0: 6e7a 6572 6f5f 766f 7865 6c73 da03 7374  nzero_voxels..st
+00000af0: 64da 0450 6174 68da 0770 6172 656e 7473  d..Path..parents
+00000b00: da02 6f73 da04 7061 7468 da05 7370 6c69  ..os..path..spli
+00000b10: 74da 0270 64da 0872 6561 645f 6373 76da  t..pd..read_csv.
+00000b20: 0566 6c6f 6174 7249 0000 00da 146d 6167  .floatrI.....mag
+00000b30: 6e69 7475 6465 5f63 6f72 7265 6374 696f  nitude_correctio
+00000b40: 6e29 0bda 0966 756e 635f 6669 6c65 da0a  n)...func_file..
+00000b50: 6e6f 6973 655f 6669 6c65 724c 0000 0072  noise_filerL...r
+00000b60: 2a00 0000 722c 0000 0072 4b00 0000 722d  *...r,...rK...r-
+00000b70: 0000 005a 0b6e 6f69 7365 5f76 616c 7565  ...Z.noise_value
+00000b80: 722b 0000 00da 1070 6172 7469 6369 7061  r+.....participa
+00000b90: 6e74 5f6e 616d 655a 0f6e 6f69 7365 5f76  nt_nameZ.noise_v
+00000ba0: 616c 7565 5f63 7376 720e 0000 0072 0e00  alue_csvr....r..
+00000bb0: 0000 7211 0000 00da 0d69 6d61 6765 534e  ..r......imageSN
+00000bc0: 525f 6361 6c63 4a00 0000 732c 0000 0008  R_calcJ...s,....
+00000bd0: 010e 0104 ff06 0106 020e 0106 0312 010a  ................
+00000be0: 020e 0314 0110 0218 0108 030e 0102 010e  ................
+00000bf0: 0104 fd06 0306 0218 0104 ff72 6000 0000  ...........r`...
+00000c00: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000c10: 0006 0000 0043 0000 0073 1c00 0000 7400  .....C...s....t.
+00000c20: 6a01 6a02 7c00 6401 6402 7c00 6403 8d04  j.j.|.d.d.|.d...
+00000c30: a003 a100 0100 6400 5300 2904 4eda 036d  ......d.S.).N..m
+00000c40: 756c 6766 6666 6666 66e6 3f29 0472 3c00  ulgffffff.?).r<.
+00000c50: 0000 7240 0000 0072 4f00 0000 723d 0000  ..r@...rO...r=..
+00000c60: 0029 0472 0200 0000 7245 0000 0072 4900  .).r....rE...rI.
+00000c70: 0000 7247 0000 0029 01da 0966 696c 655f  ..rG...)...file_
+00000c80: 6e61 6d65 720e 0000 0072 0e00 0000 7211  namer....r....r.
+00000c90: 0000 0072 5c00 0000 6800 0000 7302 0000  ...r\...h...s...
+00000ca0: 001c 0172 5c00 0000 6305 0000 0000 0000  ...r\...c.......
+00000cb0: 0000 0000 0006 0000 0009 0000 0043 0000  .............C..
+00000cc0: 0073 7c00 0000 7400 7c03 9b00 6401 7401  .s|...t.|...d.t.
+00000cd0: 6a02 9b00 6402 9d04 6403 8302 8f18 7d05  j...d...d.....}.
+00000ce0: 7c05 a003 6404 a101 0100 7c05 a004 7c02  |...d.....|...|.
+00000cf0: 9b00 6405 7c04 9b00 6406 9d04 a101 0100  ..d.|...d.......
+00000d00: 5700 6400 0400 0400 8303 0100 6e08 3100  W.d.........n.1.
+00000d10: 7327 7701 0100 0100 0100 5900 0100 7405  s'w.......Y...t.
+00000d20: a006 7c00 6407 7c02 7c03 9b00 6401 7401  ..|.d.|.|...d.t.
+00000d30: 6a02 9b00 6408 9d04 7c01 a105 7d00 7c00  j...d...|...}.|.
+00000d40: 5300 2909 4e72 1300 0000 fa27 5f70 7265  S.).Nr.....'_pre
+00000d50: 7072 6f63 6573 7365 642f 6368 616e 6765  processed/change
+00000d60: 735f 6d61 6465 5f74 6f5f 6669 6c65 732e  s_made_to_files.
+00000d70: 7478 747a 0261 2b72 0100 0000 7a02 3a20  txtz.a+r....z.: 
+00000d80: da01 0a72 0700 0000 da0d 5f70 7265 7072  ...r......_prepr
+00000d90: 6f63 6573 7365 6429 07da 046f 7065 6e72  ocessed)...openr
+00000da0: 1b00 0000 721c 0000 00da 0473 6565 6bda  ....r......seek.
+00000db0: 0577 7269 7465 7220 0000 00da 0a73 6176  .writer .....sav
+00000dc0: 655f 6272 6169 6e29 0672 3700 0000 7234  e_brain).r7...r4
+00000dd0: 0000 0072 4c00 0000 7210 0000 00da 066d  ...rL...r......m
+00000de0: 6574 686f 64da 0166 720e 0000 0072 0e00  ethod..fr....r..
+00000df0: 0000 7211 0000 00da 1b73 6176 655f 746f  ..r......save_to
+00000e00: 5f70 7265 7072 6f63 6573 7365 645f 666f  _preprocessed_fo
+00000e10: 6c64 6572 6c00 0000 730c 0000 001a 010a  lderl...s.......
+00000e20: 0118 011c fe20 0404 0272 6c00 0000 6303  ..... ...rl...c.
+00000e30: 0000 0000 0000 0000 0000 0004 0000 0008  ................
+00000e40: 0000 0043 0000 0073 a800 0000 7400 7c00  ...C...s....t.|.
+00000e50: 8301 7d03 7401 6a02 6a03 7c00 9b00 7c01  ..}.t.j.j.|...|.
+00000e60: 9b00 6401 7c02 9b00 6402 9d04 6403 8d02  ..d.|...d...d...
+00000e70: a004 a100 0100 7401 6a05 7c00 9b00 7c01  ......t.j.|...|.
+00000e80: 9b00 6401 7c02 9b00 6404 9d04 7c03 6405  ..d.|...d...|.d.
+00000e90: 8d03 a004 a100 0100 7401 6a02 6a06 6406  ........t.j.j.d.
+00000ea0: 7c01 9b00 6401 7c02 9b00 6402 9d04 7c01  |...d.|...d...|.
+00000eb0: 9b00 6401 7c02 9b00 6404 9d04 7c01 9b00  ..d.|...d...|...
+00000ec0: 6401 7c02 9b00 6407 9d04 6408 8d04 a004  d.|...d...d.....
+00000ed0: a100 0100 7c01 9b00 6401 7c02 9b00 6407  ....|...d.|...d.
+00000ee0: 9d04 7c01 9b00 6401 7c02 9b00 6404 9d04  ..|...d.|...d...
+00000ef0: 6602 5300 2909 4e72 1300 0000 723a 0000  f.S.).Nr....r:..
+00000f00: 0072 3b00 0000 7a10 5f66 696c 7465 7265  .r;...z._filtere
+00000f10: 642e 6e69 692e 677a 2903 723c 0000 0072  d.nii.gz).r<...r
+00000f20: 3d00 0000 da0e 6869 6768 7061 7373 5f73  =.....highpass_s
+00000f30: 6967 6d61 da03 6164 647a 1d5f 6669 6c74  igma..addz._filt
+00000f40: 6572 6564 5f72 6573 746f 7265 646d 6561  ered_restoredmea
+00000f50: 6e2e 6e69 692e 677a 723f 0000 0029 0772  n.nii.gzr?...).r
+00000f60: 3900 0000 7202 0000 0072 4500 0000 7246  9...r....rE...rF
+00000f70: 0000 0072 4700 0000 da0e 5465 6d70 6f72  ...rG.....Tempor
+00000f80: 616c 4669 6c74 6572 7249 0000 0029 0472  alFilterrI...).r
+00000f90: 3600 0000 722a 0000 0072 4c00 0000 5a10  6...r*...rL...Z.
+00000fa0: 7369 676d 615f 696e 5f76 6f6c 756d 6573  sigma_in_volumes
+00000fb0: 720e 0000 0072 0e00 0000 7211 0000 00da  r....r....r.....
+00000fc0: 1268 6967 6870 6173 735f 6669 6c74 6572  .highpass_filter
+00000fd0: 696e 6776 0000 0073 1e00 0000 0801 2202  ingv...s......".
+00000fe0: 0802 0e01 0201 04fe 0602 1602 0e01 0e01  ................
+00000ff0: 04fe 0602 0e02 0e01 04ff 7270 0000 0063  ..........rp...c
+00001000: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001010: 0400 0000 4300 0000 7318 0000 007c 0044  ....C...s....|.D
+00001020: 005d 077d 0174 00a0 017c 01a1 0101 0071  .].}.t...|.....q
+00001030: 0264 0053 0072 0d00 0000 2902 7256 0000  .d.S.r....).rV..
+00001040: 00da 0672 656d 6f76 6529 02da 0f72 6564  ...remove)...red
+00001050: 756e 6461 6e74 5f66 696c 6573 724b 0000  undant_filesrK..
+00001060: 0072 0e00 0000 720e 0000 0072 1100 0000  .r....r....r....
+00001070: da0c 6465 6c65 7465 5f66 696c 6573 8700  ..delete_files..
+00001080: 0000 7306 0000 0008 010c 0104 ff72 7300  ..s..........rs.
+00001090: 0000 6306 0000 0000 0000 0000 0000 0006  ..c.............
+000010a0: 0000 0006 0000 0043 0000 0073 3800 0000  .......C...s8...
+000010b0: 7c00 6401 6b02 720e 7400 7c01 7c03 7c02  |.d.k.r.t.|.|.|.
+000010c0: 7c04 7c05 8305 0100 6400 5300 7c00 6402  |.|.....d.S.|.d.
+000010d0: 6b02 721a 7401 7c01 7c02 7c04 8303 0100  k.r.t.|.|.|.....
+000010e0: 6400 5300 6400 5300 2903 4e72 0900 0000  d.S.d.S.).Nr....
+000010f0: 720a 0000 0029 0272 6000 0000 724d 0000  r....).r`...rM..
+00001100: 0029 0672 2800 0000 724b 0000 0072 4c00  .).r(...rK...rL.
+00001110: 0000 725e 0000 0072 2a00 0000 7210 0000  ..r^...r*...r...
+00001120: 0072 0e00 0000 720e 0000 0072 1100 0000  .r....r....r....
+00001130: da0f 6372 6561 7465 5f73 7461 746d 6170  ..create_statmap
+00001140: 738c 0000 0073 0a00 0000 0801 1401 0801  s....s..........
+00001150: 1001 04ff 7274 0000 0063 0400 0000 0000  ....rt...c......
+00001160: 0000 0000 0000 0d00 0000 0900 0000 4300  ..............C.
+00001170: 0000 7364 0100 0064 007d 0467 007d 0567  ..sd...d.}.g.}.g
+00001180: 007d 0674 00a0 017c 00a1 015c 027d 077d  .}.t...|...\.}.}
+00001190: 0874 00a0 027c 0764 017c 017c 039b 0064  .t...|.d.|.|...d
+000011a0: 0274 036a 049b 0064 039d 047c 08a1 0501  .t.j...d...|....
+000011b0: 0074 036a 0572 407c 039b 0064 047c 019b  .t.j.r@|...d.|..
+000011c0: 0064 059d 047d 007c 039b 0064 067c 019b  .d...}.|...d.|..
+000011d0: 0064 079d 047d 0474 066a 07a0 087c 00a1  .d...}.t.j...|..
+000011e0: 0172 3c74 066a 07a0 087c 04a1 0173 4074  .r<t.j...|...s@t
+000011f0: 0964 0883 0182 0174 036a 0a72 5774 0a7c  .d.....t.j.rWt.|
+00001200: 007c 017c 027c 0383 045c 037d 007d 097d  .|.|.|...\.}.}.}
+00001210: 0a7c 05a0 0b7c 0aa1 0101 007c 06a0 0b7c  .|...|.....|...|
+00001220: 09a1 0101 0074 036a 0c72 7c7c 029b 0064  .....t.j.r||...d
+00001230: 027c 019b 0064 099d 047d 0b74 0d6a 0e7c  .|...d...}.t.j.|
+00001240: 007c 0b64 0a8d 02a0 0fa1 0001 007c 0b7d  .|.d.........|.}
+00001250: 0074 00a0 017c 00a1 015c 027d 077d 0874  .t...|...\.}.}.t
+00001260: 107c 077c 087c 017c 0364 0b83 057d 0074  .|.|.|.|.d...}.t
+00001270: 036a 1172 9a74 0d6a 127c 0074 036a 1374  .j.r.t.j.|.t.j.t
+00001280: 036a 147c 029b 0064 027c 019b 0064 0c9d  .j.|...d.|...d..
+00001290: 0464 0d8d 04a0 0fa1 0001 007c 029b 0064  .d.........|...d
+000012a0: 027c 019b 0064 0c9d 047d 0074 036a 1572  .|...d...}.t.j.r
+000012b0: ac74 167c 007c 027c 0183 035c 027d 007d  .t.|.|.|...\.}.}
+000012c0: 0c7c 05a0 0b7c 007c 0c67 02a1 0101 007c  .|...|.|.g.....|
+000012d0: 007c 047c 057c 0666 0453 0029 0e4e 7207  .|.|.|.f.S.).Nr.
+000012e0: 0000 0072 1300 0000 7265 0000 007a 0e2f  ...r....re...z./
+000012f0: 6675 6e63 5f76 6f6c 756d 6573 2f7a 072e  func_volumes/z..
+00001300: 6e69 692e 677a 7a0e 2f6e 6f69 7365 5f76  nii.gzz./noise_v
+00001310: 6f6c 756d 652f 7a14 5f6e 6f69 7365 5f76  olume/z._noise_v
+00001320: 6f6c 756d 652e 6e69 692e 677a 7a75 436f  olume.nii.gzzuCo
+00001330: 756c 6420 6e6f 7420 6669 6e64 2073 6570  uld not find sep
+00001340: 6172 6174 6520 6e6f 6973 6520 616e 6420  arate noise and 
+00001350: 6675 6e63 7469 6f6e 616c 2076 6f6c 756d  functional volum
+00001360: 6573 2e20 5275 6e20 7468 6520 2273 6570  es. Run the "sep
+00001370: 6172 6174 6520 6e6f 6973 6520 766f 6c75  arate noise volu
+00001380: 6d65 7322 2075 7469 6c69 7479 2074 6f20  mes" utility to 
+00001390: 6372 6561 7465 2074 6865 7365 2066 696c  create these fil
+000013a0: 6573 2e7a 185f 6d6f 7469 6f6e 5f63 6f72  es.z._motion_cor
+000013b0: 7265 6374 6564 2e6e 6969 2e67 7a72 3b00  rected.nii.gzr;.
+000013c0: 0000 7a15 4d6f 7469 6f6e 2063 6f72 7265  ..z.Motion corre
+000013d0: 6374 6564 2064 6174 617a 105f 736d 6f6f  cted dataz._smoo
+000013e0: 7468 6564 2e6e 6969 2e67 7a29 0472 3c00  thed.nii.gz).r<.
+000013f0: 0000 da04 6677 686d da14 6272 6967 6874  ....fwhm..bright
+00001400: 6e65 7373 5f74 6872 6573 686f 6c64 723d  ness_thresholdr=
+00001410: 0000 0029 1772 2000 0000 7251 0000 0072  ...).r ...rQ...r
+00001420: 6900 0000 721b 0000 0072 1c00 0000 7250  i...r....r....rP
+00001430: 0000 0072 5600 0000 7257 0000 00da 0665  ...rV...rW.....e
+00001440: 7869 7374 73da 1146 696c 654e 6f74 466f  xists..FileNotFo
+00001450: 756e 6445 7272 6f72 da16 7265 6d6f 7665  undError..remove
+00001460: 5f6d 6f74 696f 6e5f 6f75 746c 6965 7273  _motion_outliers
+00001470: da06 6578 7465 6e64 da11 6d6f 7469 6f6e  ..extend..motion
+00001480: 5f63 6f72 7265 6374 696f 6e72 0200 0000  _correctionr....
+00001490: da07 4d43 464c 4952 5472 4700 0000 726c  ..MCFLIRTrG...rl
+000014a0: 0000 00da 1173 7061 7469 616c 5f73 6d6f  .....spatial_smo
+000014b0: 6f74 6869 6e67 da05 5355 5341 4eda 0e73  othing..SUSAN..s
+000014c0: 6d6f 6f74 6869 6e67 5f66 7768 6dda 1e73  moothing_fwhm..s
+000014d0: 6d6f 6f74 6869 6e67 5f62 7269 6768 746e  moothing_brightn
+000014e0: 6573 735f 7468 7265 7368 6f6c 64da 0f74  ess_threshold..t
+000014f0: 656d 706f 7261 6c5f 6669 6c74 6572 7270  emporal_filterrp
+00001500: 0000 0029 0d72 4b00 0000 724c 0000 0072  ...).rK...rL...r
+00001510: 2a00 0000 7210 0000 0072 5e00 0000 7272  *...r....r^...rr
+00001520: 0000 00da 086f 7574 6c69 6572 7372 3700  .....outliersr7.
+00001530: 0000 7234 0000 00da 126f 7574 6c69 6572  ..r4.....outlier
+00001540: 5f74 696d 6570 6f69 6e74 735a 0d6f 7574  _timepointsZ.out
+00001550: 6c69 6572 5f66 696c 6573 da06 6f75 7470  lier_files..outp
+00001560: 7574 5a0e 7265 6475 6e64 616e 745f 6669  utZ.redundant_fi
+00001570: 6c65 720e 0000 0072 0e00 0000 7211 0000  ler....r....r...
+00001580: 00da 1570 7265 7061 7265 5f73 7461 746d  ...prepare_statm
+00001590: 6170 5f66 696c 6573 9300 0000 733c 0000  ap_files....s<..
+000015a0: 0004 0104 0204 010e 0320 0106 0210 0110  ......... ......
+000015b0: 0118 0208 0106 0314 010a 010a 0106 0210  ................
+000015c0: 0112 0204 010e 0210 0106 020e 010e 0104  ................
+000015d0: ff06 0110 0106 0210 010e 010c 0272 8500  .............r..
+000015e0: 0000 6304 0000 0000 0000 0000 0000 000f  ..c.............
+000015f0: 0000 0008 0000 0043 0000 0073 0201 0000  .......C...s....
+00001600: 7c02 9b00 6401 7c01 9b00 6402 9d04 7d04  |...d.|...d...}.
+00001610: 7c02 9b00 6401 7c01 9b00 6403 9d04 7d05  |...d.|...d...}.
+00001620: 7c02 9b00 6401 7c01 9b00 6404 9d04 7d06  |...d.|...d...}.
+00001630: 7400 6a01 7c00 7c04 7c05 7c06 6405 8d04  t.j.|.|.|.|.d...
+00001640: a002 a100 0100 7403 7c02 9b00 6401 7c01  ......t.|...d.|.
+00001650: 9b00 6402 9d04 8301 8f0c 7d07 7c07 a004  ..d.......}.|...
+00001660: a100 7d08 5700 6400 0400 0400 8303 0100  ..}.W.d.........
+00001670: 6e08 3100 733c 7701 0100 0100 0100 5900  n.1.s<w.......Y.
+00001680: 0100 6700 7d09 7405 7c08 8301 4400 5d16  ..g.}.t.|...D.].
+00001690: 5c02 7d0a 7d0b 7c0b a006 6406 6407 a102  \.}.}.|...d.d...
+000016a0: a007 6408 a101 7d0c 7c0c 6409 6b03 725d  ..d...}.|.d.k.r]
+000016b0: 7c09 a008 7c0a a101 0100 7147 7409 a00a  |...|.....qGt...
+000016c0: 7c00 a101 5c02 7d0d 7d0e 740b 6a0c 7c0d  |...\.}.}.t.j.|.
+000016d0: 7c09 640a 640b 8d03 7d0d 740d 7c0d 7c0e  |.d.d...}.t.|.|.
+000016e0: 7c01 7c03 640c 8305 7d00 7c00 7c01 740e  |.|.d...}.|.|.t.
+000016f0: 7c09 8301 6702 7c04 7c05 7c06 6703 6603  |...g.|.|.|.g.f.
+00001700: 5300 290d 4e72 1300 0000 7a0d 5f6f 7574  S.).Nr....z._out
+00001710: 6c69 6572 732e 7478 747a 0c5f 6d65 7472  liers.txtz._metr
+00001720: 6963 732e 706e 677a 0c5f 6d65 7472 6963  ics.pngz._metric
+00001730: 732e 7478 7429 0472 3c00 0000 723d 0000  s.txt).r<...r=..
+00001740: 00da 0f6f 7574 5f6d 6574 7269 635f 706c  ...out_metric_pl
+00001750: 6f74 da11 6f75 745f 6d65 7472 6963 5f76  ot..out_metric_v
+00001760: 616c 7565 7372 0b00 0000 7207 0000 00da  aluesr....r.....
+00001770: 0131 e9ff ffff ffe9 0300 0000 2901 da04  .1..........)...
+00001780: 6178 6973 7a21 5265 6d6f 7665 6420 6d6f  axisz!Removed mo
+00001790: 7469 6f6e 206f 7574 6c69 6572 2074 696d  tion outlier tim
+000017a0: 6570 6f69 6e74 7329 0f72 0200 0000 da0e  epoints).r......
+000017b0: 4d6f 7469 6f6e 4f75 746c 6965 7273 7247  MotionOutliersrG
+000017c0: 0000 0072 6600 0000 da09 7265 6164 6c69  ...rf.....readli
+000017d0: 6e65 73da 0965 6e75 6d65 7261 7465 da07  nes..enumerate..
+000017e0: 7265 706c 6163 65da 0466 696e 64da 0661  replace..find..a
+000017f0: 7070 656e 6472 2000 0000 7251 0000 00da  ppendr ...rQ....
+00001800: 026e 70da 0664 656c 6574 6572 6c00 0000  .np..deleterl...
+00001810: da03 6c65 6e29 0f72 4b00 0000 724c 0000  ..len).rK...rL..
+00001820: 0072 2a00 0000 7210 0000 005a 0c6f 7574  .r*...r....Z.out
+00001830: 6c69 6572 5f66 696c 655a 0c6f 7574 6c69  lier_fileZ.outli
+00001840: 6572 5f70 6c6f 745a 0e6f 7574 6c69 6572  er_plotZ.outlier
+00001850: 5f76 616c 7565 7372 6b00 0000 da05 6c69  _valuesrk.....li
+00001860: 6e65 7372 8300 0000 5a0a 7469 6d65 5f70  nesr....Z.time_p
+00001870: 6f69 6e74 da04 6c69 6e65 5a0d 6f75 746c  oint..lineZ.outl
+00001880: 6965 725f 6368 6563 6b72 3700 0000 7234  ier_checkr7...r4
+00001890: 0000 0072 0e00 0000 720e 0000 0072 1100  ...r....r....r..
+000018a0: 0000 7279 0000 00bf 0000 0073 2a00 0000  ..ry.......s*...
+000018b0: 1001 1001 1001 0802 0201 0201 04fe 0602  ................
+000018c0: 1602 0a01 1cff 0403 1001 1201 0801 0a01  ................
+000018d0: 0280 0e02 1001 1003 1802 7279 0000 0063  ..........ry...c
+000018e0: 0600 0000 0000 0000 0000 0000 0a00 0000  ................
+000018f0: 0700 0000 4300 0000 7378 0000 007c 0561  ....C...sx...|.a
+00001900: 0074 01a0 027c 00a1 017d 067c 019b 0064  .t...|...}.|...d
+00001910: 017c 039b 0064 017c 009b 009d 057d 007c  .|...d.|.....}.|
+00001920: 019b 0064 017c 029b 009d 037d 0274 006a  ...d.|.....}.t.j
+00001930: 0372 2274 0464 027c 069b 009d 0283 0101  .r"t.d.|........
+00001940: 0074 057c 007c 067c 027c 0183 045c 047d  .t.|.|.|.|...\.}
+00001950: 007d 077d 087d 0974 067c 047c 007c 067c  .}.}.}.t.|.|.|.|
+00001960: 077c 027c 0183 0601 0074 077c 0883 0101  .|.|.....t.|....
+00001970: 007c 0953 0029 034e 7213 0000 007a 1820  .|.S.).Nr....z. 
+00001980: 2020 2020 2020 2041 6e61 6c79 7369 6e67         Analysing
+00001990: 2066 696c 653a 2029 0872 1b00 0000 7220   file: ).r....r 
+000019a0: 0000 00da 0973 7472 6970 5f65 7874 da07  .....strip_ext..
+000019b0: 7665 7262 6f73 6572 1f00 0000 7285 0000  verboser....r...
+000019c0: 0072 7400 0000 7273 0000 0029 0a72 4b00  .rt...rs...).rK.
+000019d0: 0000 7210 0000 0072 2a00 0000 7229 0000  ..r....r*...r)..
+000019e0: 0072 2800 0000 da03 6366 6772 4c00 0000  .r(.....cfgrL...
+000019f0: 725e 0000 0072 7200 0000 7282 0000 0072  r^...rr...r....r
+00001a00: 0e00 0000 720e 0000 0072 1100 0000 da1a  ....r....r......
+00001a10: 7072 6f63 6573 735f 6669 6c65 735f 666f  process_files_fo
+00001a20: 725f 7374 6174 6d61 7073 da00 0000 7314  r_statmaps....s.
+00001a30: 0000 0004 020a 0214 010e 0106 020e 0116  ................
+00001a40: 0212 0108 0204 0272 9a00 0000 6304 0000  .......r....c...
+00001a50: 0000 0000 0000 0000 000a 0000 000a 0000  ................
+00001a60: 0043 0000 0073 a401 0000 7400 6a01 7208  .C...s....t.j.r.
+00001a70: 7402 a003 a100 7d04 6e02 6400 7d04 7400  t.....}.n.d.}.t.
+00001a80: 6a04 7218 7405 6401 7400 6a06 9b00 6402  j.r.t.d.t.j...d.
+00001a90: 7c01 9b00 9d04 8301 0100 7c00 a007 a100  |.........|.....
+00001aa0: 4400 5da7 5c02 7d05 7d06 7400 6a04 7235  D.].\.}.}.t.j.r5
+00001ab0: 7405 6403 7c05 a008 6404 a101 6405 1900  t.d.|...d...d...
+00001ac0: 9b00 6406 7409 7c06 8301 9b00 6407 9d05  ..d.t.|.....d...
+00001ad0: 8301 0100 7402 6a0a 7c05 9b00 6404 7400  ....t.j.|...d.t.
+00001ae0: 6a06 9b00 6408 9d04 6409 640a 8d02 0100  j...d...d.d.....
+00001af0: 740b 7c05 9b00 6404 7400 6a06 9b00 640b  t.|...d.t.j...d.
+00001b00: 9d04 640c 8302 8f0d 7d07 7c07 a00c 640d  ..d.....}.|...d.
+00001b10: a101 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
+00001b20: 6e08 3100 735f 7701 0100 0100 0100 5900  n.1.s_w.......Y.
+00001b30: 0100 740d 7c06 740e a00f 7c05 a101 740e  ..t.|.t...|...t.
+00001b40: a00f 7c01 a101 740e a00f 7c02 a101 740e  ..|...t...|...t.
+00001b50: a00f 7c03 a101 740e a00f 7400 a101 8306  ..|...t...t.....
+00001b60: 7d08 7400 6a01 7288 7410 7c04 a011 7412  }.t.j.r.t.|...t.
+00001b70: 7c08 a102 8301 7d09 6e08 7410 740e a011  |.....}.n.t.t...
+00001b80: 7412 7c08 a102 8301 7d09 7400 6a13 72c3  t.|.....}.t.j.r.
+00001b90: 7414 6a15 640e 640f 6702 7c09 6410 8d02  t.j.d.d.g.|.d...
+00001ba0: a016 640f a101 7d09 740b 7c05 9b00 6404  ..d...}.t.|...d.
+00001bb0: 7c01 9b00 6411 9d04 640c 8302 8f11 7d07  |...d...d.....}.
+00001bc0: 7c07 a00c 7c09 6a17 6412 6413 8d01 a101  |...|.j.d.d.....
+00001bd0: 0100 5700 6400 0400 0400 8303 0100 711c  ..W.d.........q.
+00001be0: 3100 73be 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+00001bf0: 711c 7400 6a01 72d0 7402 6a18 7c04 6412  q.t.j.r.t.j.|.d.
+00001c00: 6414 8d02 0100 6400 5300 6400 5300 2915  d.....d.S.d.S.).
+00001c10: 4e7a 160a 5365 6172 6368 696e 6720 696e  Nz..Searching in
+00001c20: 2066 6f6c 6465 723a 207a 1d0a 5361 7669   folder: z..Savi
+00001c30: 6e67 206f 7574 7075 7420 696e 2064 6972  ng output in dir
+00001c40: 6563 746f 7279 3a20 7a2c 0a43 7265 6174  ectory: z,.Creat
+00001c50: 696e 6720 7374 6174 6973 7469 6361 6c20  ing statistical 
+00001c60: 6d61 7073 2066 6f72 2070 6172 7469 6369  maps for partici
+00001c70: 7061 6e74 3a20 7213 0000 0072 8900 0000  pant: r....r....
+00001c80: 7a1d 0a20 2020 2020 2043 7265 6174 696e  z..      Creatin
+00001c90: 6720 7374 6174 6d61 7073 2066 6f72 207a  g statmaps for z
+00001ca0: 0620 6669 6c65 7372 6500 0000 5472 1600  . filesre...Tr..
+00001cb0: 0000 7263 0000 00da 0177 7207 0000 00da  ..rc.....wr.....
+00001cc0: 0446 696c 657a 104f 7574 6c69 6572 7320  .Filez.Outliers 
+00001cd0: 7265 6d6f 7665 6429 02da 0763 6f6c 756d  removed)...colum
+00001ce0: 6e73 7237 0000 007a 1f2f 6e75 6d62 6572  nsr7...z./number
+00001cf0: 5f6f 665f 6f75 746c 6965 7273 5f72 656d  _of_outliers_rem
+00001d00: 6f76 6564 2e63 7376 4629 01da 0569 6e64  oved.csvF)...ind
+00001d10: 6578 2901 da07 7265 7374 6172 7429 1972  ex)...restart).r
+00001d20: 1b00 0000 da14 6d75 6c74 6963 6f72 655f  ......multicore_
+00001d30: 7072 6f63 6573 7369 6e67 7220 0000 00da  processingr ....
+00001d40: 1573 7461 7274 5f70 726f 6365 7373 696e  .start_processin
+00001d50: 675f 706f 6f6c 7298 0000 0072 1f00 0000  g_poolr....r....
+00001d60: 721c 0000 00da 0569 7465 6d73 7258 0000  r......itemsrX..
+00001d70: 0072 9400 0000 7224 0000 0072 6600 0000  .r....r$...rf...
+00001d80: 7268 0000 00da 037a 6970 da09 6974 6572  rh.....zip..iter
+00001d90: 746f 6f6c 73da 0672 6570 6561 74da 046c  tools..repeat..l
+00001da0: 6973 74da 0773 7461 726d 6170 729a 0000  ist..starmapr...
+00001db0: 0072 7900 0000 7259 0000 00da 0944 6174  .ry...rY.....Dat
+00001dc0: 6146 7261 6d65 da0b 736f 7274 5f76 616c  aFrame..sort_val
+00001dd0: 7565 73da 0674 6f5f 6373 76da 146a 6f69  ues..to_csv..joi
+00001de0: 6e5f 7072 6f63 6573 7369 6e67 5f70 6f6f  n_processing_poo
+00001df0: 6c29 0a72 2e00 0000 722a 0000 0072 2900  l).r....r*...r).
+00001e00: 0000 7228 0000 00da 0470 6f6f 6c72 2c00  ..r(.....poolr,.
+00001e10: 0000 da05 6669 6c65 7372 6b00 0000 da08  ....filesrk.....
+00001e20: 6974 6572 6162 6c65 7282 0000 0072 0e00  iterabler....r..
+00001e30: 0000 720e 0000 0072 1100 0000 da1a 6361  ..r....r......ca
+00001e40: 6c63 756c 6174 655f 7374 6174 6973 7469  lculate_statisti
+00001e50: 6361 6c5f 6d61 7073 ed00 0000 7346 0000  cal_maps....sF..
+00001e60: 0006 010a 0104 0206 020c 0102 0108 ff10  ................
+00001e70: 0306 0114 0106 010a ff1c 031a 030c 011c  ................
+00001e80: ff04 0308 0108 0108 0108 0108 0104 fb06  ................
+00001e90: 0712 0110 0206 0218 0118 0214 011c ff02  ................
+00001ea0: 8006 0312 0104 ff72 af00 0000 6304 0000  .......r....c...
+00001eb0: 0000 0000 0000 0000 0008 0000 0005 0000  ................
+00001ec0: 0043 0000 0073 f000 0000 7400 a000 a100  .C...s....t.....
+00001ed0: 7d04 7401 a002 7c01 a101 0100 7403 7404  }.t...|.....t.t.
+00001ee0: 6a05 a006 7407 a101 8301 6a08 6401 1900  j...t.....j.d...
+00001ef0: 9b00 6402 9d02 6109 7c02 610a 7401 6a0b  ..d...a.|.a.t.j.
+00001f00: 7409 7c02 7c03 6403 8d03 610c 740d a00e  t.|.|.d...a.t...
+00001f10: 6404 a101 a00f 6405 a101 0100 7c00 6406  d.....d.....|.d.
+00001f20: 6b02 7237 740c 6a10 7337 740c 6a11 7237  k.r7t.j.s7t.j.r7
+00001f30: 7412 6407 8301 0100 7c00 6408 7600 7249  t.d.....|.d.v.rI
+00001f40: 7412 6409 7c00 9b00 640a 9d03 8301 0100  t.d.|...d.......
+00001f50: 7413 740c 7c00 8302 0100 6e19 740c 6a11  t.t.|.....n.t.j.
+00001f60: 7254 7412 640b 7c00 9b00 640c 9d03 8301  rTt.d.|...d.....
+00001f70: 0100 7414 7c00 8301 5c03 7d05 7d06 7d07  ..t.|...\.}.}.}.
+00001f80: 7415 7c05 7c06 7c07 7c00 8304 0100 740c  t.|.|.|.|.....t.
+00001f90: 6a11 7276 7412 640d 7416 7400 a000 a100  j.rvt.d.t.t.....
+00001fa0: 7c04 1800 640e 8302 9b00 640f 9d03 8301  |...d.....d.....
+00001fb0: 0100 6400 5300 6400 5300 2910 4e72 0500  ..d.S.d.S.).Nr..
+00001fc0: 0000 7a1d 2f63 6f6e 6669 6775 7261 7469  ..z./configurati
+00001fd0: 6f6e 5f70 726f 6669 6c65 732f 6d61 7073  on_profiles/maps
+00001fe0: 2f29 0172 5700 0000 7a0f 6e69 7079 7065  /).rW...z.nipype
+00001ff0: 2e77 6f72 6b66 6c6f 7772 0100 0000 7209  .workflowr....r.
+00002000: 0000 007a c422 4e6f 6973 6520 766f 6c75  ...z."Noise volu
+00002010: 6d65 2069 6e63 6c75 6465 6420 696e 2074  me included in t
+00002020: 696d 6520 7365 7269 6573 2220 6973 2066  ime series" is f
+00002030: 616c 7365 2e20 5472 7969 6e67 2074 6f20  alse. Trying to 
+00002040: 6669 6e64 2076 616c 7565 7320 666f 7220  find values for 
+00002050: 6561 6368 2070 6172 7469 6369 7061 6e74  each participant
+00002060: 2069 6e20 6e6f 6973 6556 616c 7565 732e   in noiseValues.
+00002070: 6373 7620 696e 7374 6561 642e 2049 6620  csv instead. If 
+00002080: 7468 6973 2069 7320 6e6f 7420 636f 7272  this is not corr
+00002090: 6563 742c 2073 6574 2022 4e6f 6973 6520  ect, set "Noise 
+000020a0: 766f 6c75 6d65 2069 6e63 6c75 6465 6420  volume included 
+000020b0: 696e 2074 696d 6520 7365 7269 6573 2220  in time series" 
+000020c0: 746f 2074 7275 652e 0a29 037a 1241 6464  to true..).z.Add
+000020d0: 2047 6175 7373 6961 6e20 6e6f 6973 657a   Gaussian noisez
+000020e0: 0a41 6464 206d 6f74 696f 6e7a 1653 6570  .Add motionz.Sep
+000020f0: 6172 6174 6520 6e6f 6973 6520 766f 6c75  arate noise volu
+00002100: 6d65 737a 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d  meszn.----------
+00002110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002120: 2d2d 2d2d 2d2d 0a2d 2d2d 2d2d 2d2d 2d20  ------.-------- 
+00002130: 5275 6e6e 696e 6720 7574 696c 6974 7920  Running utility 
+00002140: 2d2d 2d2d 2d2d 2d2d 0a2d 2d2d 2d2d 2d2d  --------.-------
+00002150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002160: 2d2d 2d2d 2d2d 2d2d 2d0a 0a52 756e 6e69  ---------..Runni
+00002170: 6e67 207a 0a20 7574 696c 6974 792e 0a7a  ng z. utility..z
+00002180: 6e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  n.--------------
+00002190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000021a0: 2d2d 0a2d 2d2d 2053 7461 7469 7374 6963  --.--- Statistic
+000021b0: 616c 206d 6170 2063 7265 6174 696f 6e20  al map creation 
+000021c0: 2d2d 2d0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---.------------
+000021d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000021e0: 2d2d 2d2d 0a0a 4372 6561 7469 6e67 207a  ----..Creating z
+000021f0: 0720 6d61 7073 2e0a 7a12 0a2d 2d2d 2043  . maps..z..--- C
+00002200: 6f6d 706c 6574 6564 2069 6e20 7203 0000  ompleted in r...
+00002210: 007a 0e20 7365 636f 6e64 7320 2d2d 2d0a  .z. seconds ---.
+00002220: 0a29 17da 0474 696d 6572 2000 0000 da0c  .)...timer .....
+00002230: 6368 6563 6b76 6572 7369 6f6e 7254 0000  checkversionrT..
+00002240: 0072 5600 0000 7257 0000 00da 0761 6273  .rV...rW.....abs
+00002250: 7061 7468 da08 5f5f 6669 6c65 5f5f 7255  path..__file__rU
+00002260: 0000 0072 2600 0000 7227 0000 00da 0b6c  ...r&...r'.....l
+00002270: 6f61 645f 636f 6e66 6967 721b 0000 00da  oad_configr.....
+00002280: 076c 6f67 6769 6e67 da09 6765 744c 6f67  .logging..getLog
+00002290: 6765 72da 0873 6574 4c65 7665 6c72 5000  ger..setLevelrP.
+000022a0: 0000 7298 0000 0072 1f00 0000 7204 0000  ..r....r....r...
+000022b0: 0072 2f00 0000 72af 0000 00da 0572 6f75  .r/...r......rou
+000022c0: 6e64 2908 7228 0000 00da 0776 6572 7369  nd).r(.....versi
+000022d0: 6f6e da0b 636f 6e66 6967 5f66 696c 6572  on..config_filer
+000022e0: 5700 0000 da0a 7374 6172 745f 7469 6d65  W.....start_time
+000022f0: 722e 0000 0072 2a00 0000 7229 0000 0072  r....r*...r)...r
+00002300: 0e00 0000 720e 0000 0072 1100 0000 da04  ....r....r......
+00002310: 6d61 696e 1801 0000 732c 0000 0008 030a  main....s,......
+00002320: 011c 0304 0110 0310 0214 0208 0108 0304  ................
+00002330: 0102 030a fd0c 0506 0304 0102 030a fd0e  ................
+00002340: 050e 0106 0222 0104 ff72 bc00 0000 720d  ....."...r....r.
+00002350: 0000 0029 1b72 a400 0000 da05 6e75 6d70  ...).r......nump
+00002360: 7972 9200 0000 5a11 6e69 7079 7065 2e69  yr....Z.nipype.i
+00002370: 6e74 6572 6661 6365 7372 0200 0000 72b5  nterfacesr....r.
+00002380: 0000 0072 b000 0000 5a0d 484f 5553 452e  ...r....Z.HOUSE.
+00002390: 6861 6e64 6c65 7272 0400 0000 da05 7574  handlerr......ut
+000023a0: 696c 7372 1b00 0000 7226 0000 0072 2700  ilsr....r&...r'.
+000023b0: 0000 722f 0000 0072 3900 0000 724d 0000  ..r/...r9...rM..
+000023c0: 0072 6000 0000 725c 0000 0072 6c00 0000  .r`...r\...rl...
+000023d0: 7270 0000 0072 7300 0000 7274 0000 0072  rp...rs...rt...r
+000023e0: 8500 0000 7279 0000 0072 9a00 0000 72af  ....ry...r....r.
+000023f0: 0000 0072 bc00 0000 720e 0000 0072 0e00  ...r....r....r..
+00002400: 0000 720e 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
+00002410: 6f64 756c 653e 0100 0000 7330 0000 0008  odule>....s0....
+00002420: 0008 020c 0108 0108 010c 0208 0104 0204  ................
+00002430: 0104 0108 0308 2208 0808 1008 1e08 0408  ......".........
+00002440: 0a08 1108 0508 0708 2c08 1b08 130e 2b    ........,.....+
```

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jan 31 14:53:42 2023 UTC, .py size: 8967 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 762b d963 0723 0000  o.......v+.c.#..
+00000000: 6f0d 0d0a 0000 0000 fe65 5a64 3825 0000  o........eZd8%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000e 0000 0040 0000 0073 6001 0000 6900  .....@...s`...i.
+00000020: 000f 0000 0040 0000 0073 6e01 0000 6900  .....@...sn...i.
 00000030: 6400 6401 6402 6901 9301 6403 6404 6405  d.d.d.i...d.d.d.
 00000040: 6406 6407 6408 9c04 9301 6409 6404 6405  d.d.d.....d.d.d.
 00000050: 640a 640b 9c03 9301 640c 640d 640e 6700  d.d.....d.d.d.g.
 00000060: 640f a201 6410 6411 6412 9c05 9301 6413  d...d.d.d.....d.
 00000070: 6414 6415 6410 6416 6417 6418 9c05 9301  d.d.d.d.d.d.....
 00000080: 6419 6414 641a 6410 641b 641c 9c04 9301  d.d.d.d.d.d.....
 00000090: 641d 6414 641e 6410 641f 641c 9c04 9301  d.d.d.d.d.d.....
@@ -18,319 +18,337 @@
 00000110: 6408 9c04 9301 6434 6414 6435 6436 6437  d.....d4d.d5d6d7
 00000120: 6408 9c04 9301 6401 6402 6901 6404 6405  d.....d.d.i.d.d.
 00000130: 6438 640b 9c03 6404 642e 6439 643a 6408  d8d...d.d.d9d:d.
 00000140: 9c04 640d 643b 643c 643b 6702 6410 6411  ..d.d;d<d;g.d.d.
 00000150: 6412 9c05 6404 6405 643d 643e 6408 9c04  d...d.d.d=d>d...
 00000160: 6401 6402 6901 643f 6440 6441 6442 6443  d.d.i.d?d@dAdBdC
 00000170: 6444 9c05 6414 6445 6446 6447 6448 6418  dD..d.dEdFdGdHd.
-00000180: 9c05 6449 9c08 a501 5a00 644a 5300 294b  ..dI....Z.dJS.)K
-00000190: 7a10 4765 6e65 7261 6c20 7365 7474 696e  z.General settin
-000001a0: 6773 da04 7479 7065 da0a 7375 6268 6561  gs..type..subhea
-000001b0: 6469 6e67 da07 7665 7262 6f73 65da 0b43  ding..verbose..C
-000001c0: 6865 636b 4275 7474 6f6e da04 7472 7565  heckButton..true
-000001d0: 7a1e 5665 7262 6f73 6520 7374 6174 6973  z.Verbose statis
-000001e0: 7469 6361 6c20 6d61 7020 7374 6167 6573  tical map stages
-000001f0: 7a2a 7472 7565 206f 7220 6661 6c73 652e  z*true or false.
-00000200: 2050 7269 6e74 2070 726f 6772 6573 7320   Print progress 
-00000210: 746f 2074 6572 6d69 6e61 6c2e 2904 7201  to terminal.).r.
-00000220: 0000 00da 0b52 6563 6f6d 6d65 6e64 6564  .....Recommended
-00000230: da05 6c61 6265 6cda 0b44 6573 6372 6970  ..label..Descrip
-00000240: 7469 6f6e da14 6d75 6c74 6963 6f72 655f  tion..multicore_
-00000250: 7072 6f63 6573 7369 6e67 7a95 7472 7565  processingz.true
-00000260: 206f 7220 6661 6c73 652e 2055 7365 206d   or false. Use m
-00000270: 756c 7469 636f 7265 2070 726f 6365 7373  ulticore process
-00000280: 696e 6720 6475 7269 6e67 2061 6e61 6c79  ing during analy
-00000290: 7369 733f 204d 756c 7469 636f 7265 2070  sis? Multicore p
-000002a0: 726f 6365 7373 696e 6720 6375 7272 656e  rocessing curren
-000002b0: 746c 7920 776f 726b 7320 7769 7468 696e  tly works within
-000002c0: 2070 6172 7469 6369 7061 6e74 7320 6e6f   participants no
-000002d0: 7420 6265 7477 6565 6e20 7468 656d 2e20  t between them. 
-000002e0: 5265 636f 6d6d 656e 6465 643a 2074 7275  Recommended: tru
-000002f0: 6529 0372 0100 0000 7206 0000 0072 0800  e).r....r....r..
-00000300: 0000 da0e 6d61 785f 636f 7265 5f75 7361  ....max_core_usa
-00000310: 6765 da0a 4f70 7469 6f6e 4d65 6e75 da03  ge..OptionMenu..
-00000320: 6d61 7829 0772 0c00 0000 e906 0000 00e9  max).r..........
-00000330: 0500 0000 e904 0000 00e9 0300 0000 e902  ................
-00000340: 0000 00e9 0100 0000 da06 7374 7269 6e67  ..........string
-00000350: 7a8b 276d 6178 2720 746f 2073 656c 6563  z.'max' to selec
-00000360: 7420 6e75 6d62 6572 206f 6620 636f 7265  t number of core
-00000370: 7320 6176 6169 6c61 626c 6520 6f6e 2074  s available on t
-00000380: 6865 2073 7973 7465 6d2c 2061 6c74 6572  he system, alter
-00000390: 6e61 7469 7665 6c79 2061 6e20 696e 7420  natively an int 
-000003a0: 746f 206d 616e 7561 6c6c 7920 7365 6c65  to manually sele
-000003b0: 6374 206e 756d 6265 7220 6f66 2063 6f72  ct number of cor
-000003c0: 6573 2074 6f20 7573 652e 2052 6563 6f6d  es to use. Recom
-000003d0: 6d65 6e64 6564 3a20 276d 6178 2729 0572  mended: 'max').r
-000003e0: 0100 0000 7206 0000 00da 074f 7074 696f  ....r......Optio
-000003f0: 6e73 da07 7361 7665 5f61 7372 0800 0000  ns..save_asr....
-00000400: da0b 6261 7365 5f66 6f6c 6465 72da 0545  ..base_folder..E
-00000410: 6e74 7279 da00 7a14 4261 7365 2066 6f6c  ntry..z.Base fol
-00000420: 6465 7220 6c6f 6361 7469 6f6e 7a9e 4569  der locationz.Ei
-00000430: 7468 6572 2074 6865 2061 6273 6f6c 7574  ther the absolut
-00000440: 6520 6c6f 6361 7469 6f6e 206f 6620 7468  e location of th
-00000450: 6520 666f 6c64 6572 2063 6f6e 7461 696e  e folder contain
-00000460: 696e 6720 7468 6520 7375 626a 6563 7473  ing the subjects
-00000470: 206f 7220 626c 616e 6b2c 2069 6620 626c   or blank, if bl
-00000480: 616e 6b20 7468 656e 2061 2062 726f 7773  ank then a brows
-00000490: 6572 2077 696e 646f 7720 7769 6c6c 2061  er window will a
-000004a0: 6c6c 6f77 2079 6f75 2074 6f20 7365 6172  llow you to sear
-000004b0: 6368 2066 6f72 2074 6865 2066 696c 6573  ch for the files
-000004c0: 2061 7420 7275 6e74 696d 652e 2905 7201   at runtime.).r.
-000004d0: 0000 0072 0600 0000 7215 0000 0072 0700  ...r....r....r..
-000004e0: 0000 7208 0000 00da 1169 6e70 7574 5f66  ..r......input_f
-000004f0: 6f6c 6465 725f 6e61 6d65 da04 6675 6e63  older_name..func
-00000500: 7a4c 466f 6c64 6572 2066 6f75 6e64 2069  zLFolder found i
-00000510: 6e20 6561 6368 2073 7562 6a65 6374 7320  n each subjects 
-00000520: 6469 7265 6374 6f72 7920 636f 6e74 6169  directory contai
-00000530: 6e69 6e67 2074 6865 2066 696c 6573 2074  ning the files t
-00000540: 6f20 6265 2061 6e61 6c79 7365 642e 2904  o be analysed.).
-00000550: 7201 0000 0072 0600 0000 7215 0000 0072  r....r....r....r
-00000560: 0800 0000 da12 6f75 7470 7574 5f66 6f6c  ......output_fol
-00000570: 6465 725f 6e61 6d65 da07 4445 4641 554c  der_name..DEFAUL
-00000580: 547a 8044 6972 6563 746f 7279 2074 6f20  Tz.Directory to 
-00000590: 7361 7665 206f 7574 7075 742e 2049 6620  save output. If 
-000005a0: 7365 7420 746f 2044 4546 4155 4c54 2c20  set to DEFAULT, 
-000005b0: 7468 6520 6465 6661 756c 7420 6e61 6d65  the default name
-000005c0: 2066 6f72 2074 6865 2073 7461 7469 7374   for the statist
-000005d0: 6963 616c 206d 6170 2063 7265 6174 6564  ical map created
-000005e0: 2077 696c 6c20 6265 2075 7365 642e 2052   will be used. R
-000005f0: 6563 6f6d 6d65 6e64 6564 3a20 4445 4641  ecommended: DEFA
-00000600: 554c 547a 1348 6967 6820 7061 7373 2066  ULTz.High pass f
-00000610: 696c 7465 7269 6e67 5a0f 7465 6d70 6f72  ilteringZ.tempor
-00000620: 616c 5f66 696c 7465 727a 5674 7275 6520  al_filterzVtrue 
-00000630: 6f72 2066 616c 7365 2e20 5573 6520 6120  or false. Use a 
-00000640: 6869 6768 2070 6173 7320 6669 6c74 6572  high pass filter
-00000650: 2074 6f20 7265 6d6f 7665 206c 6f77 2066   to remove low f
-00000660: 7265 7175 656e 6379 2064 7269 6674 2e20  requency drift. 
-00000670: 5265 636f 6d6d 656e 6465 643a 2074 7275  Recommended: tru
-00000680: 655a 1668 6967 6870 6173 735f 6669 6c74  eZ.highpass_filt
-00000690: 6572 5f63 7574 6f66 6667 7b14 ae47 e17a  er_cutoffg{..G.z
-000006a0: 843f 7a25 4869 6768 7061 7373 2066 696c  .?z%Highpass fil
-000006b0: 7465 7220 6375 746f 6666 2066 7265 7175  ter cutoff frequ
-000006c0: 656e 6379 2028 487a 297a 7048 6967 6870  ency (Hz)zpHighp
-000006d0: 6173 7320 6669 6c74 6572 2063 7574 6f66  ass filter cutof
-000006e0: 6620 6672 6571 7565 6e63 7920 636f 6e76  f frequency conv
-000006f0: 6572 7465 6420 696e 746f 2073 6967 6d61  erted into sigma
-00000700: 2069 6e20 7365 636f 6e64 7320 7573 696e   in seconds usin
-00000710: 6720 7468 6520 666f 726d 756c 6120 312f  g the formula 1/
-00000720: 2832 2a66 2a54 5229 2e20 5265 636f 6d6d  (2*f*TR). Recomm
-00000730: 656e 6465 643a 2030 2e30 317a 114d 6f74  ended: 0.01z.Mot
-00000740: 696f 6e20 636f 7272 6563 7469 6f6e 5a16  ion correctionZ.
-00000750: 7265 6d6f 7665 5f6d 6f74 696f 6e5f 6f75  remove_motion_ou
-00000760: 746c 6965 7273 7a7e 7472 7565 206f 7220  tliersz~true or 
-00000770: 6661 6c73 652e 2055 7365 2066 736c 5f6d  false. Use fsl_m
-00000780: 6f74 696f 6e5f 6f75 746c 6965 7273 2074  otion_outliers t
-00000790: 6f20 7265 6d6f 7665 206d 6f74 696f 6e20  o remove motion 
-000007a0: 6f75 746c 6965 7273 2875 7365 7320 6465  outliers(uses de
-000007b0: 6661 756c 7420 6673 6c5f 6d6f 7469 6f6e  fault fsl_motion
-000007c0: 5f6f 7574 6c69 6572 7320 7365 7474 696e  _outliers settin
-000007d0: 6773 292e 2052 6563 6f6d 6d65 6e64 6564  gs). Recommended
-000007e0: 3a20 7472 7565 5a11 6d6f 7469 6f6e 5f63  : trueZ.motion_c
-000007f0: 6f72 7265 6374 696f 6e7a 6774 7275 6520  orrectionzgtrue 
-00000800: 6f72 2066 616c 7365 2e20 5573 6520 4d43  or false. Use MC
-00000810: 464c 4952 5420 746f 206d 6f74 696f 6e20  FLIRT to motion 
-00000820: 636f 7272 6563 7420 766f 6c75 6d65 7320  correct volumes 
-00000830: 2875 7365 7320 6465 6661 756c 7420 4d43  (uses default MC
-00000840: 464c 4952 5420 7365 7474 696e 6773 292e  FLIRT settings).
-00000850: 2052 6563 6f6d 6d65 6e64 6564 3a20 7472   Recommended: tr
-00000860: 7565 7a11 5370 6174 6961 6c20 736d 6f6f  uez.Spatial smoo
-00000870: 7468 696e 675a 1173 7061 7469 616c 5f73  thingZ.spatial_s
-00000880: 6d6f 6f74 6869 6e67 da05 6661 6c73 657a  moothing..falsez
-00000890: 3e74 7275 6520 6f72 2066 616c 7365 2e20  >true or false. 
-000008a0: 5573 6573 2053 5553 414e 2074 6f20 7370  Uses SUSAN to sp
-000008b0: 6174 6961 6c20 736d 6f6f 7468 2e20 5265  atial smooth. Re
-000008c0: 636f 6d6d 656e 6465 643a 2074 7275 65da  commended: true.
-000008d0: 0e73 6d6f 6f74 6869 6e67 5f66 7768 6d67  .smoothing_fwhmg
-000008e0: 0000 0000 0000 2040 7a1b 5370 6174 6961  ...... @z.Spatia
-000008f0: 6c20 736d 6f6f 7468 696e 6720 6677 686d  l smoothing fwhm
-00000900: 2028 6d6d 297a 4f66 7768 6d20 6f66 2073   (mm)zOfwhm of s
-00000910: 6d6f 6f74 6869 6e67 2c20 696e 206d 6d2c  moothing, in mm,
-00000920: 2067 6574 7320 636f 6e76 6572 7465 6420   gets converted 
-00000930: 7573 696e 6720 7371 7274 2838 2a6c 6f67  using sqrt(8*log
-00000940: 2832 2929 2e20 5265 636f 6d6d 656e 6465  (2)). Recommende
-00000950: 643a 2038 2e30 5a1e 736d 6f6f 7468 696e  d: 8.0Z.smoothin
-00000960: 675f 6272 6967 6874 6e65 7373 5f74 6872  g_brightness_thr
-00000970: 6573 686f 6c64 6700 0000 0000 409f 407a  esholdg.....@.@z
-00000980: 2653 7061 7469 616c 2073 6d6f 6f74 6869  &Spatial smoothi
-00000990: 6e67 2062 7269 6768 746e 6573 7320 7468  ng brightness th
-000009a0: 7265 7368 6f6c 647a 6753 686f 756c 6420  resholdzgShould 
-000009b0: 6265 2067 7265 6174 6572 2074 6861 6e20  be greater than 
-000009c0: 6e6f 6973 6520 6c65 7665 6c20 616e 6420  noise level and 
-000009d0: 6c65 7373 2074 6861 6e20 636f 6e74 7261  less than contra
-000009e0: 7374 206f 6620 6564 6765 7320 746f 2062  st of edges to b
-000009f0: 6520 7072 6573 6572 7665 642e 2052 6563  e preserved. Rec
-00000a00: 6f6d 6d65 6e64 6564 3a20 3230 3030 2e30  ommended: 2000.0
-00000a10: 6132 0100 0074 7275 6520 6f72 2066 616c  a2...true or fal
-00000a20: 7365 2e20 436f 7272 6563 7469 6f6e 2066  se. Correction f
-00000a30: 6163 746f 7220 6f66 2030 2e37 2061 7070  actor of 0.7 app
-00000a40: 6c69 6564 2077 6865 6e20 7275 6e6e 696e  lied when runnin
-00000a50: 6720 6953 4e52 2063 616c 6375 6c61 7469  g iSNR calculati
-00000a60: 6f6e 732c 2074 6f20 636f 7272 6563 7420  ons, to correct 
-00000a70: 666f 7220 5261 796c 6569 6768 2064 6973  for Rayleigh dis
-00000a80: 7472 6962 7574 6564 206e 6f69 7365 2077  tributed noise w
-00000a90: 6865 6e20 7573 696e 6720 6d61 676e 6974  hen using magnit
-00000aa0: 7564 6520 7673 2063 6f6d 706c 6578 2069  ude vs complex i
-00000ab0: 6d61 6765 732e 200a 5265 6665 7265 6e63  mages. .Referenc
-00000ac0: 653a 2043 6f6e 7374 616e 7469 6e69 6465  e: Constantinide
-00000ad0: 732c 2043 2e20 442e 2c20 4174 616c 6172  s, C. D., Atalar
-00000ae0: 2c20 452e 2c20 2620 4d63 5665 6967 682c  , E., & McVeigh,
-00000af0: 2045 2e20 522e 2028 3139 3937 292e 2053   E. R. (1997). S
-00000b00: 6967 6e61 6c2d 746f 2d4e 6f69 7365 204d  ignal-to-Noise M
-00000b10: 6561 7375 7265 6d65 6e74 7320 696e 204d  easurements in M
-00000b20: 6167 6e69 7475 6465 2049 6d61 6765 7320  agnitude Images 
-00000b30: 6672 6f6d 204e 4d52 2050 6861 7365 6420  from NMR Phased 
-00000b40: 4172 7261 7973 2e7a 244e 6f69 7365 2076  Arrays.z$Noise v
-00000b50: 6f6c 756d 6520 696e 636c 7564 6564 2069  olume included i
-00000b60: 6e20 7469 6d65 2073 6572 6965 7361 9901  n time seriesa..
-00000b70: 0000 7472 7565 206f 7220 6661 6c73 652e  ..true or false.
-00000b80: 2053 656c 6563 7420 7472 7565 2069 6620   Select true if 
-00000b90: 6120 6e6f 6973 6520 766f 6c75 6d65 2068  a noise volume h
-00000ba0: 6173 2062 6565 6e20 636f 6c6c 6563 7465  as been collecte
-00000bb0: 6420 6173 2070 6172 7420 6f66 2074 6865  d as part of the
-00000bc0: 2066 4d52 4920 7469 6d65 2073 6572 6965   fMRI time serie
-00000bd0: 732e 0a4e 4f54 453a 2049 6620 7472 7565  s..NOTE: If true
-00000be0: 2c20 7468 6520 6e6f 6973 6520 766f 6c75  , the noise volu
-00000bf0: 6d65 2069 6e20 7468 6520 7469 6d65 2073  me in the time s
-00000c00: 6572 6965 7320 7769 6c6c 2062 6520 7365  eries will be se
-00000c10: 7061 7261 7465 6420 6672 6f6d 2074 6865  parated from the
-00000c20: 2066 756e 6374 696f 6e61 6c20 766f 6c75   functional volu
-00000c30: 6d65 7320 616e 6420 7769 6c6c 2062 6520  mes and will be 
-00000c40: 706c 6163 6564 2069 6e74 6f20 7468 6520  placed into the 
-00000c50: 666f 6c64 6572 2022 6675 6e63 5f6e 6f69  folder "func_noi
-00000c60: 7365 566f 6c75 6d65 5265 6d6f 7665 6422  seVolumeRemoved"
-00000c70: 2e0a 4966 2022 6e6f 6973 6520 766f 6c75  ..If "noise volu
-00000c80: 6d65 2220 6973 2074 7275 6520 616e 6420  me" is true and 
-00000c90: 226e 6f69 7365 2076 616c 7565 2220 6973  "noise value" is
-00000ca0: 206e 6f74 206e 6f6e 652c 2074 6865 206e   not none, the n
-00000cb0: 6f69 7365 2076 6f6c 756d 6520 7769 6c6c  oise volume will
-00000cc0: 2062 6520 7573 6564 2069 6e20 696d 6167   be used in imag
-00000cd0: 6520 534e 5220 6361 6c63 756c 6174 696f  e SNR calculatio
-00000ce0: 6e20 7261 7468 6572 2074 6861 6e20 7468  n rather than th
-00000cf0: 6520 7573 6572 2064 6566 696e 6564 206e  e user defined n
-00000d00: 6f69 7365 2076 616c 7565 2eda 0345 6e64  oise value...End
-00000d10: 5a09 4265 6769 6e6e 696e 677a 2555 7365  Z.Beginningz%Use
-00000d20: 206f 6e6c 7920 6e6f 6e7a 6572 6f20 766f   only nonzero vo
-00000d30: 7865 6c73 2066 6f72 2069 534e 5220 6361  xels for iSNR ca
-00000d40: 6c63 7a0e 7472 7565 206f 7220 6661 6c73  lcz.true or fals
-00000d50: 652e da06 4275 7474 6f6e da11 6372 6561  e...Button..crea
-00000d60: 7465 5f6e 6f69 7365 5f66 696c 657a 1643  te_noise_filez.C
-00000d70: 7265 6174 6520 6e6f 6973 6556 616c 7565  reate noiseValue
-00000d80: 732e 6373 7646 61f9 0300 0043 7265 6174  s.csvFa....Creat
-00000d90: 6520 6120 6e6f 6973 6556 616c 7565 732e  e a noiseValues.
-00000da0: 6373 7620 6669 6c65 2074 6f20 6465 7465  csv file to dete
-00000db0: 726d 696e 6520 7768 6174 2074 6865 2073  rmine what the s
-00000dc0: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
-00000dd0: 6e6f 6620 7468 6520 4761 7573 7369 616e  nof the Gaussian
-00000de0: 2073 686f 756c 6420 6265 2077 6865 6e20   should be when 
-00000df0: 6164 6469 6e67 206e 6f69 7365 2074 6f20  adding noise to 
-00000e00: 6561 6368 2070 6172 7469 6369 7061 6e74  each participant
-00000e10: 2773 2064 6174 6120 2874 6865 2064 6973  's data (the dis
-00000e20: 7472 6962 7574 696f 6e20 7769 6c6c 2068  tribution will h
-00000e30: 6176 6520 6120 6d65 616e 206f 6620 3029  ave a mean of 0)
-00000e40: 2e54 6869 7320 7769 6c6c 206e 6f74 206f  .This will not o
-00000e50: 7665 7277 7269 7465 2074 6865 206f 7269  verwrite the ori
-00000e60: 6769 6e61 6c20 6669 6c65 732e 2052 6563  ginal files. Rec
-00000e70: 6f6d 6d65 6e64 6564 3a20 5468 6520 7374  ommended: The st
-00000e80: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-00000e90: 206f 7665 7220 7469 6d65 2066 6f75 6e64   over time found
-00000ea0: 2069 6e20 7468 6520 6461 7461 7365 742e   in the dataset.
-00000eb0: 0a4e 4f54 453a 2043 616e 2062 6520 7573  .NOTE: Can be us
-00000ec0: 6564 2074 6f20 7365 6520 686f 7720 6164  ed to see how ad
-00000ed0: 6469 7469 6f6e 616c 206e 6f69 7365 2061  ditional noise a
-00000ee0: 6666 6563 7473 2061 6e61 6c79 7369 732e  ffects analysis.
-00000ef0: 2054 6f20 6361 6c63 756c 6174 6520 7468   To calculate th
-00000f00: 6520 6e6f 6973 6520 6c65 7665 6c20 666f  e noise level fo
-00000f10: 7220 6561 6368 2070 6172 7469 6369 7061  r each participa
-00000f20: 6e74 2c20 6372 6561 7465 2074 534e 5220  nt, create tSNR 
-00000f30: 6d61 7073 2077 6974 6820 7468 6520 6652  maps with the fR
-00000f40: 4154 2061 6e64 2072 756e 2074 6865 2066  AT and run the f
-00000f50: 756c 6c20 616e 616c 7973 6973 2075 7369  ull analysis usi
-00000f60: 6e67 2074 6865 2074 5374 6420 6669 6c65  ng the tStd file
-00000f70: 732e 2054 6865 206d 6561 6e20 7661 6c75  s. The mean valu
-00000f80: 6573 206f 6620 7468 6973 2061 6e61 6c79  es of this analy
-00000f90: 7369 7320 696e 2065 6163 6820 7061 7274  sis in each part
-00000fa0: 6963 6970 616e 7473 2073 7562 666f 6c64  icipants subfold
-00000fb0: 6572 2c20 7769 6c6c 2074 6865 6e20 7368  er, will then sh
-00000fc0: 6f77 2079 6f75 2074 6865 2061 7665 7261  ow you the avera
-00000fd0: 6765 206e 6f69 7365 2066 6f72 2065 6163  ge noise for eac
-00000fe0: 6820 7265 6769 6f6e 2066 6f72 2065 6163  h region for eac
-00000ff0: 6820 7061 7274 6963 6970 616e 742e 0a0a  h participant...
-00001000: 5468 6973 2066 696c 6520 6361 6e20 616c  This file can al
-00001010: 736f 2062 6520 7573 6564 2074 6f20 6d61  so be used to ma
-00001020: 6e75 616c 6c79 2073 6574 2061 206e 6f69  nually set a noi
-00001030: 7365 2076 616c 7565 2066 6f72 2065 6163  se value for eac
-00001040: 6820 7061 7274 6963 6970 616e 7420 666f  h participant fo
-00001050: 7220 7573 6520 696e 2069 534e 5220 6361  r use in iSNR ca
-00001060: 6c63 756c 6174 696f 6e2e 2054 6869 7320  lculation. This 
-00001070: 6e6f 6973 6520 7661 6c75 6520 6361 6e20  noise value can 
-00001080: 6265 2063 616c 6375 6c61 7465 6420 6173  be calculated as
-00001090: 2074 6865 2073 7461 6e64 6172 6420 6465   the standard de
-000010a0: 7669 6174 696f 6e20 6f66 2076 6f78 656c  viation of voxel
-000010b0: 2076 616c 7565 7320 6f75 7473 6964 6520   values outside 
-000010c0: 6f66 2074 6865 2062 7261 696e 2e20 4966  of the brain. If
-000010d0: 2022 4e6f 6973 6520 766f 6c75 6d65 2069   "Noise volume i
-000010e0: 6e63 6c75 6465 6420 696e 2074 696d 6520  ncluded in time 
-000010f0: 7365 7269 6573 2220 6973 2073 6574 2074  series" is set t
-00001100: 6f20 7472 7565 2c20 7374 616e 6461 7264  o true, standard
-00001110: 2064 6576 6961 7469 6f6e 206f 6620 6e6f   deviation of no
-00001120: 6973 6520 7769 6c6c 2062 6520 6361 6c63  ise will be calc
-00001130: 756c 6174 6564 2075 7369 6e67 2074 6865  ulated using the
-00001140: 206e 6f69 7365 2076 6f6c 756d 652c 2065   noise volume, e
-00001150: 7665 6e20 6966 2061 206e 6f69 7365 2076  ven if a noise v
-00001160: 616c 7565 2068 6173 2062 6565 6e20 7072  alue has been pr
-00001170: 6f76 6964 6564 2069 6e20 7468 6973 2066  ovided in this f
-00001180: 696c 652e 2905 7201 0000 00da 0743 6f6d  ile.).r......Com
-00001190: 6d61 6e64 da04 5465 7874 7a09 5061 7373  mand..Textz.Pass
-000011a0: 2073 656c 6672 0800 0000 7212 0000 00da   selfr....r.....
-000011b0: 046c 6973 747a 134e 6f69 7365 206d 756c  .listz.Noise mul
-000011c0: 7469 706c 6965 7228 7329 6131 0100 0050  tiplier(s)a1...P
-000011d0: 726f 7669 6465 2061 2063 6f6d 6d61 2d73  rovide a comma-s
-000011e0: 6570 6172 6174 6564 206c 6973 7420 6f66  eparated list of
-000011f0: 206d 756c 7469 706c 6965 7273 2066 6f72   multipliers for
-00001200: 2074 6865 2073 7461 6e64 6172 6420 6465   the standard de
-00001210: 7669 6174 696f 6e20 6f66 2074 6865 2067  viation of the g
-00001220: 6175 7373 6961 6e20 6e6f 6973 6520 746f  aussian noise to
-00001230: 2070 6c6f 7420 652e 672e 2027 312c 2035   plot e.g. '1, 5
-00001240: 272e 2041 2073 6570 6172 6174 6520 6669  '. A separate fi
-00001250: 6c65 2077 696c 6c20 6265 2070 726f 6475  le will be produ
-00001260: 6365 6420 666f 7220 6561 6368 206d 756c  ced for each mul
-00001270: 7469 706c 6965 722e 0a4e 4f54 453a 204e  tiplier..NOTE: N
-00001280: 6f69 7365 2068 6173 2061 2067 6175 7373  oise has a gauss
-00001290: 6961 6e20 6469 7374 7269 6275 7469 6f6e  ian distribution
-000012a0: 2c20 7769 7468 2061 206d 6561 6e20 6f66  , with a mean of
-000012b0: 2030 2061 6e64 2061 2073 7461 6e64 6172   0 and a standar
-000012c0: 6420 6465 7669 6174 696f 6e20 6f66 2074  d deviation of t
-000012d0: 6865 206e 6f69 7365 206c 6576 656c 206f  he noise level o
-000012e0: 6620 6561 6368 2070 6172 7469 6369 7061  f each participa
-000012f0: 6e74 202a 206d 756c 7469 706c 6965 722e  nt * multiplier.
-00001300: 2908 7a15 496d 6167 6520 534e 5220 6361  ).z.Image SNR ca
-00001310: 6c63 756c 6174 696f 6e5a 146d 6167 6e69  lculationZ.magni
-00001320: 7475 6465 5f63 6f72 7265 6374 696f 6e5a  tude_correctionZ
-00001330: 0c6e 6f69 7365 5f76 6f6c 756d 655a 156e  .noise_volumeZ.n
-00001340: 6f69 7365 5f76 6f6c 756d 655f 6c6f 6361  oise_volume_loca
-00001350: 7469 6f6e 5a20 6953 4e52 5f73 7464 5f75  tionZ iSNR_std_u
-00001360: 7365 5f6f 6e6c 795f 6e6f 6e7a 6572 6f5f  se_only_nonzero_
-00001370: 766f 7865 6c73 7a12 4164 6420 4761 7573  voxelsz.Add Gaus
-00001380: 7369 616e 206e 6f69 7365 5a17 6372 6561  sian noiseZ.crea
-00001390: 7465 5f6e 6f69 7365 5f6c 6576 656c 5f66  te_noise_level_f
-000013a0: 696c 655a 116e 6f69 7365 5f6d 756c 7469  ileZ.noise_multi
-000013b0: 706c 6965 7273 4e29 01da 1053 7461 7469  pliersN)...Stati
-000013c0: 7374 6963 616c 5f6d 6170 73a9 0072 2600  stical_maps..r&.
-000013d0: 0000 7226 0000 00fa 5f2f 5573 6572 732f  ..r&...._/Users/
-000013e0: 6c70 7865 6831 302f 446f 6375 6d65 6e74  lpxeh10/Document
-000013f0: 732f 5265 706f 7369 746f 7269 6573 2f66  s/Repositories/f
-00001400: 4d52 495f 524f 495f 616e 616c 7973 6973  MRI_ROI_analysis
-00001410: 5f74 6f6f 6c2f 6652 4154 2f75 7469 6c73  _tool/fRAT/utils
-00001420: 2f73 7461 746d 6170 5f63 6f6e 6669 675f  /statmap_config_
-00001430: 7365 7475 702e 7079 da08 3c6d 6f64 756c  setup.py..<modul
-00001440: 653e 0100 0000 73b4 0000 0002 0008 0102  e>....s.........
-00001450: ff08 0302 0104 ff02 fd06 0602 0104 ff02  ................
-00001460: fa0c 0b02 0102 0104 fe02 f508 1002 0102  ................
-00001470: 0104 fe02 f008 1602 0104 ff02 ea08 1a02  ................
-00001480: 0104 ff02 e608 1f02 e106 2102 0104 ff02  ..........!.....
-00001490: df06 2502 0102 0104 fe02 db08 2a02 d606  ..%.........*...
-000014a0: 2c02 0104 ff02 d406 3002 0104 ff02 d008  ,.......0.......
-000014b0: 3402 cc06 3602 0104 ff02 ca06 3902 0102  4...6.......9...
-000014c0: 0104 fe02 c706 3d02 0102 0104 fe02 c306  ......=.........
-000014d0: 4204 0202 0104 ff06 0702 0104 ff0a 0802  B...............
-000014e0: 0102 0104 fe04 0502 0102 0104 fe06 0406  ................
-000014f0: 0202 0102 0104 fe08 1502 0104 ff0c 8d    ...............
+00000180: 9c05 6414 6445 6446 6449 644a 6418 9c05  ..d.dEdFdIdJd...
+00000190: 644b 9c09 a501 5a00 644c 5300 294d 7a10  dK....Z.dLS.)Mz.
+000001a0: 4765 6e65 7261 6c20 7365 7474 696e 6773  General settings
+000001b0: da04 7479 7065 da0a 7375 6268 6561 6469  ..type..subheadi
+000001c0: 6e67 da07 7665 7262 6f73 65da 0b43 6865  ng..verbose..Che
+000001d0: 636b 4275 7474 6f6e da04 7472 7565 7a1e  ckButton..truez.
+000001e0: 5665 7262 6f73 6520 7374 6174 6973 7469  Verbose statisti
+000001f0: 6361 6c20 6d61 7020 7374 6167 6573 7a2a  cal map stagesz*
+00000200: 7472 7565 206f 7220 6661 6c73 652e 2050  true or false. P
+00000210: 7269 6e74 2070 726f 6772 6573 7320 746f  rint progress to
+00000220: 2074 6572 6d69 6e61 6c2e 2904 7201 0000   terminal.).r...
+00000230: 00da 0b52 6563 6f6d 6d65 6e64 6564 da05  ...Recommended..
+00000240: 6c61 6265 6cda 0b44 6573 6372 6970 7469  label..Descripti
+00000250: 6f6e da14 6d75 6c74 6963 6f72 655f 7072  on..multicore_pr
+00000260: 6f63 6573 7369 6e67 7a95 7472 7565 206f  ocessingz.true o
+00000270: 7220 6661 6c73 652e 2055 7365 206d 756c  r false. Use mul
+00000280: 7469 636f 7265 2070 726f 6365 7373 696e  ticore processin
+00000290: 6720 6475 7269 6e67 2061 6e61 6c79 7369  g during analysi
+000002a0: 733f 204d 756c 7469 636f 7265 2070 726f  s? Multicore pro
+000002b0: 6365 7373 696e 6720 6375 7272 656e 746c  cessing currentl
+000002c0: 7920 776f 726b 7320 7769 7468 696e 2070  y works within p
+000002d0: 6172 7469 6369 7061 6e74 7320 6e6f 7420  articipants not 
+000002e0: 6265 7477 6565 6e20 7468 656d 2e20 5265  between them. Re
+000002f0: 636f 6d6d 656e 6465 643a 2074 7275 6529  commended: true)
+00000300: 0372 0100 0000 7206 0000 0072 0800 0000  .r....r....r....
+00000310: da0e 6d61 785f 636f 7265 5f75 7361 6765  ..max_core_usage
+00000320: da0a 4f70 7469 6f6e 4d65 6e75 da03 6d61  ..OptionMenu..ma
+00000330: 7829 0772 0c00 0000 e906 0000 00e9 0500  x).r............
+00000340: 0000 e904 0000 00e9 0300 0000 e902 0000  ................
+00000350: 00e9 0100 0000 da06 7374 7269 6e67 7a8b  ........stringz.
+00000360: 276d 6178 2720 746f 2073 656c 6563 7420  'max' to select 
+00000370: 6e75 6d62 6572 206f 6620 636f 7265 7320  number of cores 
+00000380: 6176 6169 6c61 626c 6520 6f6e 2074 6865  available on the
+00000390: 2073 7973 7465 6d2c 2061 6c74 6572 6e61   system, alterna
+000003a0: 7469 7665 6c79 2061 6e20 696e 7420 746f  tively an int to
+000003b0: 206d 616e 7561 6c6c 7920 7365 6c65 6374   manually select
+000003c0: 206e 756d 6265 7220 6f66 2063 6f72 6573   number of cores
+000003d0: 2074 6f20 7573 652e 2052 6563 6f6d 6d65   to use. Recomme
+000003e0: 6e64 6564 3a20 276d 6178 2729 0572 0100  nded: 'max').r..
+000003f0: 0000 7206 0000 00da 074f 7074 696f 6e73  ..r......Options
+00000400: da07 7361 7665 5f61 7372 0800 0000 da0b  ..save_asr......
+00000410: 6261 7365 5f66 6f6c 6465 72da 0545 6e74  base_folder..Ent
+00000420: 7279 da00 7a14 4261 7365 2066 6f6c 6465  ry..z.Base folde
+00000430: 7220 6c6f 6361 7469 6f6e 7a9e 4569 7468  r locationz.Eith
+00000440: 6572 2074 6865 2061 6273 6f6c 7574 6520  er the absolute 
+00000450: 6c6f 6361 7469 6f6e 206f 6620 7468 6520  location of the 
+00000460: 666f 6c64 6572 2063 6f6e 7461 696e 696e  folder containin
+00000470: 6720 7468 6520 7375 626a 6563 7473 206f  g the subjects o
+00000480: 7220 626c 616e 6b2c 2069 6620 626c 616e  r blank, if blan
+00000490: 6b20 7468 656e 2061 2062 726f 7773 6572  k then a browser
+000004a0: 2077 696e 646f 7720 7769 6c6c 2061 6c6c   window will all
+000004b0: 6f77 2079 6f75 2074 6f20 7365 6172 6368  ow you to search
+000004c0: 2066 6f72 2074 6865 2066 696c 6573 2061   for the files a
+000004d0: 7420 7275 6e74 696d 652e 2905 7201 0000  t runtime.).r...
+000004e0: 0072 0600 0000 7215 0000 0072 0700 0000  .r....r....r....
+000004f0: 7208 0000 00da 1169 6e70 7574 5f66 6f6c  r......input_fol
+00000500: 6465 725f 6e61 6d65 da04 6675 6e63 7a4c  der_name..funczL
+00000510: 466f 6c64 6572 2066 6f75 6e64 2069 6e20  Folder found in 
+00000520: 6561 6368 2073 7562 6a65 6374 7320 6469  each subjects di
+00000530: 7265 6374 6f72 7920 636f 6e74 6169 6e69  rectory containi
+00000540: 6e67 2074 6865 2066 696c 6573 2074 6f20  ng the files to 
+00000550: 6265 2061 6e61 6c79 7365 642e 2904 7201  be analysed.).r.
+00000560: 0000 0072 0600 0000 7215 0000 0072 0800  ...r....r....r..
+00000570: 0000 da12 6f75 7470 7574 5f66 6f6c 6465  ....output_folde
+00000580: 725f 6e61 6d65 da07 4445 4641 554c 547a  r_name..DEFAULTz
+00000590: 8044 6972 6563 746f 7279 2074 6f20 7361  .Directory to sa
+000005a0: 7665 206f 7574 7075 742e 2049 6620 7365  ve output. If se
+000005b0: 7420 746f 2044 4546 4155 4c54 2c20 7468  t to DEFAULT, th
+000005c0: 6520 6465 6661 756c 7420 6e61 6d65 2066  e default name f
+000005d0: 6f72 2074 6865 2073 7461 7469 7374 6963  or the statistic
+000005e0: 616c 206d 6170 2063 7265 6174 6564 2077  al map created w
+000005f0: 696c 6c20 6265 2075 7365 642e 2052 6563  ill be used. Rec
+00000600: 6f6d 6d65 6e64 6564 3a20 4445 4641 554c  ommended: DEFAUL
+00000610: 547a 1348 6967 6820 7061 7373 2066 696c  Tz.High pass fil
+00000620: 7465 7269 6e67 5a0f 7465 6d70 6f72 616c  teringZ.temporal
+00000630: 5f66 696c 7465 727a 5674 7275 6520 6f72  _filterzVtrue or
+00000640: 2066 616c 7365 2e20 5573 6520 6120 6869   false. Use a hi
+00000650: 6768 2070 6173 7320 6669 6c74 6572 2074  gh pass filter t
+00000660: 6f20 7265 6d6f 7665 206c 6f77 2066 7265  o remove low fre
+00000670: 7175 656e 6379 2064 7269 6674 2e20 5265  quency drift. Re
+00000680: 636f 6d6d 656e 6465 643a 2074 7275 655a  commended: trueZ
+00000690: 1668 6967 6870 6173 735f 6669 6c74 6572  .highpass_filter
+000006a0: 5f63 7574 6f66 6667 7b14 ae47 e17a 843f  _cutoffg{..G.z.?
+000006b0: 7a25 4869 6768 7061 7373 2066 696c 7465  z%Highpass filte
+000006c0: 7220 6375 746f 6666 2066 7265 7175 656e  r cutoff frequen
+000006d0: 6379 2028 487a 297a 7048 6967 6870 6173  cy (Hz)zpHighpas
+000006e0: 7320 6669 6c74 6572 2063 7574 6f66 6620  s filter cutoff 
+000006f0: 6672 6571 7565 6e63 7920 636f 6e76 6572  frequency conver
+00000700: 7465 6420 696e 746f 2073 6967 6d61 2069  ted into sigma i
+00000710: 6e20 7365 636f 6e64 7320 7573 696e 6720  n seconds using 
+00000720: 7468 6520 666f 726d 756c 6120 312f 2832  the formula 1/(2
+00000730: 2a66 2a54 5229 2e20 5265 636f 6d6d 656e  *f*TR). Recommen
+00000740: 6465 643a 2030 2e30 317a 114d 6f74 696f  ded: 0.01z.Motio
+00000750: 6e20 636f 7272 6563 7469 6f6e 5a16 7265  n correctionZ.re
+00000760: 6d6f 7665 5f6d 6f74 696f 6e5f 6f75 746c  move_motion_outl
+00000770: 6965 7273 7a7e 7472 7565 206f 7220 6661  iersz~true or fa
+00000780: 6c73 652e 2055 7365 2066 736c 5f6d 6f74  lse. Use fsl_mot
+00000790: 696f 6e5f 6f75 746c 6965 7273 2074 6f20  ion_outliers to 
+000007a0: 7265 6d6f 7665 206d 6f74 696f 6e20 6f75  remove motion ou
+000007b0: 746c 6965 7273 2875 7365 7320 6465 6661  tliers(uses defa
+000007c0: 756c 7420 6673 6c5f 6d6f 7469 6f6e 5f6f  ult fsl_motion_o
+000007d0: 7574 6c69 6572 7320 7365 7474 696e 6773  utliers settings
+000007e0: 292e 2052 6563 6f6d 6d65 6e64 6564 3a20  ). Recommended: 
+000007f0: 7472 7565 5a11 6d6f 7469 6f6e 5f63 6f72  trueZ.motion_cor
+00000800: 7265 6374 696f 6e7a 6774 7275 6520 6f72  rectionzgtrue or
+00000810: 2066 616c 7365 2e20 5573 6520 4d43 464c   false. Use MCFL
+00000820: 4952 5420 746f 206d 6f74 696f 6e20 636f  IRT to motion co
+00000830: 7272 6563 7420 766f 6c75 6d65 7320 2875  rrect volumes (u
+00000840: 7365 7320 6465 6661 756c 7420 4d43 464c  ses default MCFL
+00000850: 4952 5420 7365 7474 696e 6773 292e 2052  IRT settings). R
+00000860: 6563 6f6d 6d65 6e64 6564 3a20 7472 7565  ecommended: true
+00000870: 7a11 5370 6174 6961 6c20 736d 6f6f 7468  z.Spatial smooth
+00000880: 696e 675a 1173 7061 7469 616c 5f73 6d6f  ingZ.spatial_smo
+00000890: 6f74 6869 6e67 da05 6661 6c73 657a 3e74  othing..falsez>t
+000008a0: 7275 6520 6f72 2066 616c 7365 2e20 5573  rue or false. Us
+000008b0: 6573 2053 5553 414e 2074 6f20 7370 6174  es SUSAN to spat
+000008c0: 6961 6c20 736d 6f6f 7468 2e20 5265 636f  ial smooth. Reco
+000008d0: 6d6d 656e 6465 643a 2074 7275 65da 0e73  mmended: true..s
+000008e0: 6d6f 6f74 6869 6e67 5f66 7768 6d67 0000  moothing_fwhmg..
+000008f0: 0000 0000 2040 7a1b 5370 6174 6961 6c20  .... @z.Spatial 
+00000900: 736d 6f6f 7468 696e 6720 6677 686d 2028  smoothing fwhm (
+00000910: 6d6d 297a 4f66 7768 6d20 6f66 2073 6d6f  mm)zOfwhm of smo
+00000920: 6f74 6869 6e67 2c20 696e 206d 6d2c 2067  othing, in mm, g
+00000930: 6574 7320 636f 6e76 6572 7465 6420 7573  ets converted us
+00000940: 696e 6720 7371 7274 2838 2a6c 6f67 2832  ing sqrt(8*log(2
+00000950: 2929 2e20 5265 636f 6d6d 656e 6465 643a  )). Recommended:
+00000960: 2038 2e30 5a1e 736d 6f6f 7468 696e 675f   8.0Z.smoothing_
+00000970: 6272 6967 6874 6e65 7373 5f74 6872 6573  brightness_thres
+00000980: 686f 6c64 6700 0000 0000 409f 407a 2653  holdg.....@.@z&S
+00000990: 7061 7469 616c 2073 6d6f 6f74 6869 6e67  patial smoothing
+000009a0: 2062 7269 6768 746e 6573 7320 7468 7265   brightness thre
+000009b0: 7368 6f6c 647a 6753 686f 756c 6420 6265  sholdzgShould be
+000009c0: 2067 7265 6174 6572 2074 6861 6e20 6e6f   greater than no
+000009d0: 6973 6520 6c65 7665 6c20 616e 6420 6c65  ise level and le
+000009e0: 7373 2074 6861 6e20 636f 6e74 7261 7374  ss than contrast
+000009f0: 206f 6620 6564 6765 7320 746f 2062 6520   of edges to be 
+00000a00: 7072 6573 6572 7665 642e 2052 6563 6f6d  preserved. Recom
+00000a10: 6d65 6e64 6564 3a20 3230 3030 2e30 6132  mended: 2000.0a2
+00000a20: 0100 0074 7275 6520 6f72 2066 616c 7365  ...true or false
+00000a30: 2e20 436f 7272 6563 7469 6f6e 2066 6163  . Correction fac
+00000a40: 746f 7220 6f66 2030 2e37 2061 7070 6c69  tor of 0.7 appli
+00000a50: 6564 2077 6865 6e20 7275 6e6e 696e 6720  ed when running 
+00000a60: 6953 4e52 2063 616c 6375 6c61 7469 6f6e  iSNR calculation
+00000a70: 732c 2074 6f20 636f 7272 6563 7420 666f  s, to correct fo
+00000a80: 7220 5261 796c 6569 6768 2064 6973 7472  r Rayleigh distr
+00000a90: 6962 7574 6564 206e 6f69 7365 2077 6865  ibuted noise whe
+00000aa0: 6e20 7573 696e 6720 6d61 676e 6974 7564  n using magnitud
+00000ab0: 6520 7673 2063 6f6d 706c 6578 2069 6d61  e vs complex ima
+00000ac0: 6765 732e 200a 5265 6665 7265 6e63 653a  ges. .Reference:
+00000ad0: 2043 6f6e 7374 616e 7469 6e69 6465 732c   Constantinides,
+00000ae0: 2043 2e20 442e 2c20 4174 616c 6172 2c20   C. D., Atalar, 
+00000af0: 452e 2c20 2620 4d63 5665 6967 682c 2045  E., & McVeigh, E
+00000b00: 2e20 522e 2028 3139 3937 292e 2053 6967  . R. (1997). Sig
+00000b10: 6e61 6c2d 746f 2d4e 6f69 7365 204d 6561  nal-to-Noise Mea
+00000b20: 7375 7265 6d65 6e74 7320 696e 204d 6167  surements in Mag
+00000b30: 6e69 7475 6465 2049 6d61 6765 7320 6672  nitude Images fr
+00000b40: 6f6d 204e 4d52 2050 6861 7365 6420 4172  om NMR Phased Ar
+00000b50: 7261 7973 2e7a 244e 6f69 7365 2076 6f6c  rays.z$Noise vol
+00000b60: 756d 6520 696e 636c 7564 6564 2069 6e20  ume included in 
+00000b70: 7469 6d65 2073 6572 6965 7361 9901 0000  time seriesa....
+00000b80: 7472 7565 206f 7220 6661 6c73 652e 2053  true or false. S
+00000b90: 656c 6563 7420 7472 7565 2069 6620 6120  elect true if a 
+00000ba0: 6e6f 6973 6520 766f 6c75 6d65 2068 6173  noise volume has
+00000bb0: 2062 6565 6e20 636f 6c6c 6563 7465 6420   been collected 
+00000bc0: 6173 2070 6172 7420 6f66 2074 6865 2066  as part of the f
+00000bd0: 4d52 4920 7469 6d65 2073 6572 6965 732e  MRI time series.
+00000be0: 0a4e 4f54 453a 2049 6620 7472 7565 2c20  .NOTE: If true, 
+00000bf0: 7468 6520 6e6f 6973 6520 766f 6c75 6d65  the noise volume
+00000c00: 2069 6e20 7468 6520 7469 6d65 2073 6572   in the time ser
+00000c10: 6965 7320 7769 6c6c 2062 6520 7365 7061  ies will be sepa
+00000c20: 7261 7465 6420 6672 6f6d 2074 6865 2066  rated from the f
+00000c30: 756e 6374 696f 6e61 6c20 766f 6c75 6d65  unctional volume
+00000c40: 7320 616e 6420 7769 6c6c 2062 6520 706c  s and will be pl
+00000c50: 6163 6564 2069 6e74 6f20 7468 6520 666f  aced into the fo
+00000c60: 6c64 6572 2022 6675 6e63 5f6e 6f69 7365  lder "func_noise
+00000c70: 566f 6c75 6d65 5265 6d6f 7665 6422 2e0a  VolumeRemoved"..
+00000c80: 4966 2022 6e6f 6973 6520 766f 6c75 6d65  If "noise volume
+00000c90: 2220 6973 2074 7275 6520 616e 6420 226e  " is true and "n
+00000ca0: 6f69 7365 2076 616c 7565 2220 6973 206e  oise value" is n
+00000cb0: 6f74 206e 6f6e 652c 2074 6865 206e 6f69  ot none, the noi
+00000cc0: 7365 2076 6f6c 756d 6520 7769 6c6c 2062  se volume will b
+00000cd0: 6520 7573 6564 2069 6e20 696d 6167 6520  e used in image 
+00000ce0: 534e 5220 6361 6c63 756c 6174 696f 6e20  SNR calculation 
+00000cf0: 7261 7468 6572 2074 6861 6e20 7468 6520  rather than the 
+00000d00: 7573 6572 2064 6566 696e 6564 206e 6f69  user defined noi
+00000d10: 7365 2076 616c 7565 2eda 0345 6e64 5a09  se value...EndZ.
+00000d20: 4265 6769 6e6e 696e 677a 2555 7365 206f  Beginningz%Use o
+00000d30: 6e6c 7920 6e6f 6e7a 6572 6f20 766f 7865  nly nonzero voxe
+00000d40: 6c73 2066 6f72 2069 534e 5220 6361 6c63  ls for iSNR calc
+00000d50: 7a0e 7472 7565 206f 7220 6661 6c73 652e  z.true or false.
+00000d60: da06 4275 7474 6f6e da11 6372 6561 7465  ..Button..create
+00000d70: 5f6e 6f69 7365 5f66 696c 657a 1643 7265  _noise_filez.Cre
+00000d80: 6174 6520 6e6f 6973 6556 616c 7565 732e  ate noiseValues.
+00000d90: 6373 7646 61f9 0300 0043 7265 6174 6520  csvFa....Create 
+00000da0: 6120 6e6f 6973 6556 616c 7565 732e 6373  a noiseValues.cs
+00000db0: 7620 6669 6c65 2074 6f20 6465 7465 726d  v file to determ
+00000dc0: 696e 6520 7768 6174 2074 6865 2073 7461  ine what the sta
+00000dd0: 6e64 6172 6420 6465 7669 6174 696f 6e6f  ndard deviationo
+00000de0: 6620 7468 6520 4761 7573 7369 616e 2073  f the Gaussian s
+00000df0: 686f 756c 6420 6265 2077 6865 6e20 6164  hould be when ad
+00000e00: 6469 6e67 206e 6f69 7365 2074 6f20 6561  ding noise to ea
+00000e10: 6368 2070 6172 7469 6369 7061 6e74 2773  ch participant's
+00000e20: 2064 6174 6120 2874 6865 2064 6973 7472   data (the distr
+00000e30: 6962 7574 696f 6e20 7769 6c6c 2068 6176  ibution will hav
+00000e40: 6520 6120 6d65 616e 206f 6620 3029 2e54  e a mean of 0).T
+00000e50: 6869 7320 7769 6c6c 206e 6f74 206f 7665  his will not ove
+00000e60: 7277 7269 7465 2074 6865 206f 7269 6769  rwrite the origi
+00000e70: 6e61 6c20 6669 6c65 732e 2052 6563 6f6d  nal files. Recom
+00000e80: 6d65 6e64 6564 3a20 5468 6520 7374 616e  mended: The stan
+00000e90: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
+00000ea0: 7665 7220 7469 6d65 2066 6f75 6e64 2069  ver time found i
+00000eb0: 6e20 7468 6520 6461 7461 7365 742e 0a4e  n the dataset..N
+00000ec0: 4f54 453a 2043 616e 2062 6520 7573 6564  OTE: Can be used
+00000ed0: 2074 6f20 7365 6520 686f 7720 6164 6469   to see how addi
+00000ee0: 7469 6f6e 616c 206e 6f69 7365 2061 6666  tional noise aff
+00000ef0: 6563 7473 2061 6e61 6c79 7369 732e 2054  ects analysis. T
+00000f00: 6f20 6361 6c63 756c 6174 6520 7468 6520  o calculate the 
+00000f10: 6e6f 6973 6520 6c65 7665 6c20 666f 7220  noise level for 
+00000f20: 6561 6368 2070 6172 7469 6369 7061 6e74  each participant
+00000f30: 2c20 6372 6561 7465 2074 534e 5220 6d61  , create tSNR ma
+00000f40: 7073 2077 6974 6820 7468 6520 6652 4154  ps with the fRAT
+00000f50: 2061 6e64 2072 756e 2074 6865 2066 756c   and run the ful
+00000f60: 6c20 616e 616c 7973 6973 2075 7369 6e67  l analysis using
+00000f70: 2074 6865 2074 5374 6420 6669 6c65 732e   the tStd files.
+00000f80: 2054 6865 206d 6561 6e20 7661 6c75 6573   The mean values
+00000f90: 206f 6620 7468 6973 2061 6e61 6c79 7369   of this analysi
+00000fa0: 7320 696e 2065 6163 6820 7061 7274 6963  s in each partic
+00000fb0: 6970 616e 7473 2073 7562 666f 6c64 6572  ipants subfolder
+00000fc0: 2c20 7769 6c6c 2074 6865 6e20 7368 6f77  , will then show
+00000fd0: 2079 6f75 2074 6865 2061 7665 7261 6765   you the average
+00000fe0: 206e 6f69 7365 2066 6f72 2065 6163 6820   noise for each 
+00000ff0: 7265 6769 6f6e 2066 6f72 2065 6163 6820  region for each 
+00001000: 7061 7274 6963 6970 616e 742e 0a0a 5468  participant...Th
+00001010: 6973 2066 696c 6520 6361 6e20 616c 736f  is file can also
+00001020: 2062 6520 7573 6564 2074 6f20 6d61 6e75   be used to manu
+00001030: 616c 6c79 2073 6574 2061 206e 6f69 7365  ally set a noise
+00001040: 2076 616c 7565 2066 6f72 2065 6163 6820   value for each 
+00001050: 7061 7274 6963 6970 616e 7420 666f 7220  participant for 
+00001060: 7573 6520 696e 2069 534e 5220 6361 6c63  use in iSNR calc
+00001070: 756c 6174 696f 6e2e 2054 6869 7320 6e6f  ulation. This no
+00001080: 6973 6520 7661 6c75 6520 6361 6e20 6265  ise value can be
+00001090: 2063 616c 6375 6c61 7465 6420 6173 2074   calculated as t
+000010a0: 6865 2073 7461 6e64 6172 6420 6465 7669  he standard devi
+000010b0: 6174 696f 6e20 6f66 2076 6f78 656c 2076  ation of voxel v
+000010c0: 616c 7565 7320 6f75 7473 6964 6520 6f66  alues outside of
+000010d0: 2074 6865 2062 7261 696e 2e20 4966 2022   the brain. If "
+000010e0: 4e6f 6973 6520 766f 6c75 6d65 2069 6e63  Noise volume inc
+000010f0: 6c75 6465 6420 696e 2074 696d 6520 7365  luded in time se
+00001100: 7269 6573 2220 6973 2073 6574 2074 6f20  ries" is set to 
+00001110: 7472 7565 2c20 7374 616e 6461 7264 2064  true, standard d
+00001120: 6576 6961 7469 6f6e 206f 6620 6e6f 6973  eviation of nois
+00001130: 6520 7769 6c6c 2062 6520 6361 6c63 756c  e will be calcul
+00001140: 6174 6564 2075 7369 6e67 2074 6865 206e  ated using the n
+00001150: 6f69 7365 2076 6f6c 756d 652c 2065 7665  oise volume, eve
+00001160: 6e20 6966 2061 206e 6f69 7365 2076 616c  n if a noise val
+00001170: 7565 2068 6173 2062 6565 6e20 7072 6f76  ue has been prov
+00001180: 6964 6564 2069 6e20 7468 6973 2066 696c  ided in this fil
+00001190: 652e 2905 7201 0000 00da 0743 6f6d 6d61  e.).r......Comma
+000011a0: 6e64 da04 5465 7874 7a09 5061 7373 2073  nd..Textz.Pass s
+000011b0: 656c 6672 0800 0000 7212 0000 00da 046c  elfr....r......l
+000011c0: 6973 747a 134e 6f69 7365 206d 756c 7469  istz.Noise multi
+000011d0: 706c 6965 7228 7329 7af9 5072 6f76 6964  plier(s)z.Provid
+000011e0: 6520 6120 636f 6d6d 612d 7365 7061 7261  e a comma-separa
+000011f0: 7465 6420 6c69 7374 206f 6620 6d75 6c74  ted list of mult
+00001200: 6970 6c69 6572 732c 2065 2e67 2e20 2731  ipliers, e.g. '1
+00001210: 2c20 3527 2e20 4120 7365 7061 7261 7465  , 5'. A separate
+00001220: 2066 696c 6520 7769 6c6c 2062 6520 7072   file will be pr
+00001230: 6f64 7563 6564 2066 6f72 2065 6163 6820  oduced for each 
+00001240: 6d75 6c74 6970 6c69 6572 2e0a 4e4f 5445  multiplier..NOTE
+00001250: 3a20 4164 6465 6420 6861 7320 6120 6761  : Added has a ga
+00001260: 7573 7369 616e 2064 6973 7472 6962 7574  ussian distribut
+00001270: 696f 6e2c 2077 6974 6820 6120 6d65 616e  ion, with a mean
+00001280: 206f 6620 3020 616e 6420 6120 7374 616e   of 0 and a stan
+00001290: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
+000012a0: 6620 7468 6520 6e6f 6973 6520 6c65 7665  f the noise leve
+000012b0: 6c20 6f66 2065 6163 6820 7061 7274 6963  l of each partic
+000012c0: 6970 616e 7420 2a20 6d75 6c74 6970 6c69  ipant * multipli
+000012d0: 6572 2e7a 144d 6f74 696f 6e20 6d75 6c74  er.z.Motion mult
+000012e0: 6970 6c69 6572 2873 2961 1101 0000 5072  iplier(s)a....Pr
+000012f0: 6f76 6964 6520 6120 636f 6d6d 612d 7365  ovide a comma-se
+00001300: 7061 7261 7465 6420 6c69 7374 206f 6620  parated list of 
+00001310: 6d75 6c74 6970 6c69 6572 732c 2065 2e67  multipliers, e.g
+00001320: 2e20 2731 2c20 3527 2e20 4120 7365 7061  . '1, 5'. A sepa
+00001330: 7261 7465 2066 696c 6520 7769 6c6c 2062  rate file will b
+00001340: 6520 7072 6f64 7563 6564 2066 6f72 2065  e produced for e
+00001350: 6163 6820 6d75 6c74 6970 6c69 6572 2e0a  ach multiplier..
+00001360: 4e4f 5445 3a20 4164 6465 6420 6d6f 7469  NOTE: Added moti
+00001370: 6f6e 2068 6173 2061 2067 6175 7373 6961  on has a gaussia
+00001380: 6e20 6469 7374 7269 6275 7469 6f6e 2c20  n distribution, 
+00001390: 7769 7468 2061 206d 6561 6e20 6f66 2030  with a mean of 0
+000013a0: 2061 6e64 2061 2073 7461 6e64 6172 6420   and a standard 
+000013b0: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
+000013c0: 2061 7665 7261 6765 2072 6f74 6174 696f   average rotatio
+000013d0: 6e2f 7472 616e 736c 6174 696f 6e20 6f66  n/translation of
+000013e0: 2065 6163 6820 7061 7274 6963 6970 616e   each participan
+000013f0: 7420 2a20 6d75 6c74 6970 6c69 6572 2e29  t * multiplier.)
+00001400: 097a 1549 6d61 6765 2053 4e52 2063 616c  .z.Image SNR cal
+00001410: 6375 6c61 7469 6f6e 5a14 6d61 676e 6974  culationZ.magnit
+00001420: 7564 655f 636f 7272 6563 7469 6f6e 5a0c  ude_correctionZ.
+00001430: 6e6f 6973 655f 766f 6c75 6d65 5a15 6e6f  noise_volumeZ.no
+00001440: 6973 655f 766f 6c75 6d65 5f6c 6f63 6174  ise_volume_locat
+00001450: 696f 6e5a 2069 534e 525f 7374 645f 7573  ionZ iSNR_std_us
+00001460: 655f 6f6e 6c79 5f6e 6f6e 7a65 726f 5f76  e_only_nonzero_v
+00001470: 6f78 656c 737a 1241 6464 2047 6175 7373  oxelsz.Add Gauss
+00001480: 6961 6e20 6e6f 6973 655a 1763 7265 6174  ian noiseZ.creat
+00001490: 655f 6e6f 6973 655f 6c65 7665 6c5f 6669  e_noise_level_fi
+000014a0: 6c65 5a11 6e6f 6973 655f 6d75 6c74 6970  leZ.noise_multip
+000014b0: 6c69 6572 735a 126d 6f74 696f 6e5f 6d75  liersZ.motion_mu
+000014c0: 6c74 6970 6c69 6572 734e 2901 da10 5374  ltipliersN)...St
+000014d0: 6174 6973 7469 6361 6c5f 6d61 7073 a900  atistical_maps..
+000014e0: 7226 0000 0072 2600 0000 fa5f 2f55 7365  r&...r&...._/Use
+000014f0: 7273 2f6c 7078 6568 3130 2f44 6f63 756d  rs/lpxeh10/Docum
+00001500: 656e 7473 2f52 6570 6f73 6974 6f72 6965  ents/Repositorie
+00001510: 732f 664d 5249 5f52 4f49 5f61 6e61 6c79  s/fMRI_ROI_analy
+00001520: 7369 735f 746f 6f6c 2f66 5241 542f 7574  sis_tool/fRAT/ut
+00001530: 696c 732f 7374 6174 6d61 705f 636f 6e66  ils/statmap_conf
+00001540: 6967 5f73 6574 7570 2e70 79da 083c 6d6f  ig_setup.py..<mo
+00001550: 6475 6c65 3e01 0000 0073 ba00 0000 0200  dule>....s......
+00001560: 0801 02ff 0803 0201 04ff 02fd 0606 0201  ................
+00001570: 04ff 02fa 0c0b 0201 0201 04fe 02f5 0810  ................
+00001580: 0201 0201 04fe 02f0 0816 0201 04ff 02ea  ................
+00001590: 081a 0201 04ff 02e6 081f 02e1 0621 0201  .............!..
+000015a0: 04ff 02df 0625 0201 0201 04fe 02db 082a  .....%.........*
+000015b0: 02d6 062c 0201 04ff 02d4 0630 0201 04ff  ...,.......0....
+000015c0: 02d0 0834 02cc 0636 0201 04ff 02ca 0639  ...4...6.......9
+000015d0: 0201 0201 04fe 02c7 063d 0201 0201 04fe  .........=......
+000015e0: 02c3 0642 0402 0201 04ff 0607 0201 04ff  ...B............
+000015f0: 0a08 0201 0201 04fe 0405 0201 0201 04fe  ................
+00001600: 0604 0602 0201 0201 04fe 0815 0201 04ff  ................
+00001610: 0806 0201 04ff 0c87                      ........
```

### Comparing `frat_brain-1.4.0/fRAT/utils/__pycache__/utils.cpython-310.pyc` & `frat_brain-1.5.0/fRAT/utils/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr 20 10:26:54 2023 UTC, .py size: 18883 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6e13 4164 c349 0000  o.......n.Ad.I..
+00000000: 6f0d 0d0a 0000 0000 49db 5364 d44a 0000  o.......I.Sd.J..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -13,924 +13,941 @@
 000000c0: 6117 4700 6407 6408 8400 6408 8302 5a18  a.G.d.d...d...Z.
 000000d0: 6401 5300 2909 e900 0000 004e 2901 da04  d.S.)......N)...
 000000e0: 676c 6f62 2901 da04 5061 7468 2902 da02  glob)...Path)...
 000000f0: 546b da0a 6669 6c65 6469 616c 6f67 2901  Tk..filedialog).
 00000100: da0f 5369 6d70 6c65 4e61 6d65 7370 6163  ..SimpleNamespac
 00000110: 6529 01da 012a 6300 0000 0000 0000 0000  e)...*c.........
 00000120: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00000130: 5201 0000 6500 5a01 6400 5a02 6503 6401  R...e.Z.d.Z.e.d.
+00000130: 6001 0000 6500 5a01 6400 5a02 6503 6401  `...e.Z.d.Z.e.d.
 00000140: 6402 8400 8301 5a04 6503 6403 6404 8400  d.....Z.e.d.d...
 00000150: 8301 5a05 6503 6405 6406 8400 8301 5a06  ..Z.e.d.d.....Z.
 00000160: 6503 6407 6408 8400 8301 5a07 6503 6409  e.d.d.....Z.e.d.
-00000170: 640a 8400 8301 5a08 6503 643b 640d 640e  d.....Z.e.d;d.d.
+00000170: 640a 8400 8301 5a08 6503 643d 640d 640e  d.....Z.e.d=d.d.
 00000180: 8401 8301 5a09 6503 640f 6410 8400 8301  ....Z.e.d.d.....
-00000190: 5a0a 6503 643c 6414 6415 8401 8301 5a0b  Z.e.d<d.d.....Z.
-000001a0: 6503 643d 6417 6418 8401 8301 5a0c 6503  e.d=d.d.....Z.e.
-000001b0: 643e 6419 641a 8401 8301 5a0d 6503 641b  d>d.d.....Z.e.d.
+00000190: 5a0a 6503 643e 6414 6415 8401 8301 5a0b  Z.e.d>d.d.....Z.
+000001a0: 6503 643f 6417 6418 8401 8301 5a0c 6503  e.d?d.d.....Z.e.
+000001b0: 6440 6419 641a 8401 8301 5a0d 6503 641b  d@d.d.....Z.e.d.
 000001c0: 641c 8400 8301 5a0e 6503 641d 641e 8400  d.....Z.e.d.d...
 000001d0: 8301 5a0f 6503 641f 6420 8400 8301 5a10  ..Z.e.d.d ....Z.
-000001e0: 6503 643f 6421 6422 8401 8301 5a11 6503  e.d?d!d"....Z.e.
+000001e0: 6503 6441 6421 6422 8401 8301 5a11 6503  e.dAd!d"....Z.e.
 000001f0: 6423 6424 8400 8301 5a12 6503 6425 6426  d#d$....Z.e.d%d&
 00000200: 8400 8301 5a13 6503 6427 6428 8400 8301  ....Z.e.d'd(....
-00000210: 5a14 6503 643e 6429 642a 8401 8301 5a15  Z.e.d>d)d*....Z.
-00000220: 6503 642b 642c 8400 8301 5a16 6517 6440  e.d+d,....Z.e.d@
+00000210: 5a14 6503 6440 6429 642a 8401 8301 5a15  Z.e.d@d)d*....Z.
+00000220: 6503 642b 642c 8400 8301 5a16 6517 6442  e.d+d,....Z.e.dB
 00000230: 642d 642e 8401 8301 5a18 6503 642f 6430  d-d.....Z.e.d/d0
 00000240: 8400 8301 5a19 6503 6431 6432 8400 8301  ....Z.e.d1d2....
 00000250: 5a1a 6503 6433 6434 8400 8301 5a1b 6503  Z.e.d3d4....Z.e.
 00000260: 6435 6436 8400 8301 5a1c 6503 6437 6438  d5d6....Z.e.d7d8
 00000270: 8400 8301 5a1d 6503 6439 643a 8400 8301  ....Z.e.d9d:....
-00000280: 5a1e 6411 5300 2941 da05 5574 696c 7363  Z.d.S.)A..Utilsc
-00000290: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000002a0: 0900 0000 4300 0000 7352 0000 007a 1c7c  ....C...sR...z.|
-000002b0: 0064 0176 0072 097c 00a0 00a1 007d 0074  .d.v.r.|.....}.t
-000002c0: 01a0 027c 00a1 017d 0074 037c 0074 0483  ...|...}.t.|.t..
-000002d0: 0272 1a74 057c 0083 017d 0057 007c 0053  .r.t.|...}.W.|.S
-000002e0: 0057 007c 0053 0004 0074 0674 0766 0279  .W.|.S...t.t.f.y
-000002f0: 2801 0001 0001 0059 007c 0053 0077 0029  (......Y.|.S.w.)
-00000300: 024e 2902 da04 7472 7565 da05 6661 6c73  .N)...true..fals
-00000310: 6529 08da 0574 6974 6c65 da03 6173 74da  e)...title..ast.
-00000320: 0c6c 6974 6572 616c 5f65 7661 6cda 0a69  .literal_eval..i
-00000330: 7369 6e73 7461 6e63 65da 0574 7570 6c65  sinstance..tuple
-00000340: da04 6c69 7374 da0a 5661 6c75 6545 7272  ..list..ValueErr
-00000350: 6f72 da0b 5379 6e74 6178 4572 726f 7229  or..SyntaxError)
-00000360: 01da 0178 a900 7214 0000 00fa 502f 5573  ...x..r.....P/Us
-00000370: 6572 732f 6c70 7865 6831 302f 446f 6375  ers/lpxeh10/Docu
-00000380: 6d65 6e74 732f 5265 706f 7369 746f 7269  ments/Repositori
-00000390: 6573 2f66 4d52 495f 524f 495f 616e 616c  es/fMRI_ROI_anal
-000003a0: 7973 6973 5f74 6f6f 6c2f 6652 4154 2f75  ysis_tool/fRAT/u
-000003b0: 7469 6c73 2f75 7469 6c73 2e70 79da 2363  tils/utils.py.#c
-000003c0: 6f6e 7665 7274 5f74 6f6d 6c5f 696e 7075  onvert_toml_inpu
-000003d0: 745f 746f 5f70 7974 686f 6e5f 6f62 6a65  t_to_python_obje
-000003e0: 6374 1800 0000 731a 0000 0002 0208 0108  ct....s.........
-000003f0: 010a 020a 020a 0104 0502 fa04 0610 fd02  ................
-00000400: 0104 0202 fd7a 2955 7469 6c73 2e63 6f6e  .....z)Utils.con
-00000410: 7665 7274 5f74 6f6d 6c5f 696e 7075 745f  vert_toml_input_
-00000420: 746f 5f70 7974 686f 6e5f 6f62 6a65 6374  to_python_object
-00000430: 6300 0000 0000 0000 0000 0000 0006 0000  c...............
-00000440: 000a 0000 0043 0000 0073 cc00 0000 7400  .....C...s....t.
-00000450: 6a01 6401 6402 6403 6404 6405 8d04 7d00  j.d.d.d.d.d...}.
-00000460: 7c00 6a02 6406 6407 6408 6409 8d03 0100  |.j.d.d.d.d.....
-00000470: 7403 640a 6400 8502 1900 7d01 7c01 4400  t.d.d.....}.|.D.
-00000480: 5d46 7d02 7404 7c02 8301 4400 5d3f 7d03  ]F}.t.|...D.]?}.
-00000490: 7404 7c02 8301 7c03 1900 640b 1900 640c  t.|...|...d...d.
-000004a0: 6b02 722c 711f 7a0e 7404 7c02 8301 7c03  k.r,q.z.t.|...|.
-000004b0: 1900 640d 1900 a005 640e 640f a102 7d04  ..d.....d.d...}.
-000004c0: 5700 6e09 0400 7406 7943 0100 0100 0100  W.n...t.yC......
-000004d0: 5900 711f 7700 7c04 6410 6b02 7253 6411  Y.q.w.|.d.k.rSd.
-000004e0: 7404 7c02 8301 7c03 1900 6412 1900 9b00  t.|...|...d.....
-000004f0: 9d02 7d04 7c00 6a02 6413 7c03 9b00 9d02  ..}.|.j.d.|.....
-00000500: 7c03 7c04 6409 8d03 0100 711f 7119 7c00  |.|.d.....q.q.|.
-00000510: a007 a100 7d05 7c05 5300 2914 4e7a 0766  ....}.|.S.).Nz.f
-00000520: 5241 542e 7079 7a14 2528 7072 6f67 2973  RAT.pyz.%(prog)s
-00000530: 205b 6172 6775 6d65 6e74 735d 7a44 436f   [arguments]zDCo
-00000540: 6e76 6572 7420 766f 7865 6c77 6973 6520  nvert voxelwise 
-00000550: 7374 6174 6973 7469 6373 2074 6f20 7265  statistics to re
-00000560: 6769 6f6e 7769 7365 2073 7461 7469 7374  gionwise statist
-00000570: 6963 7320 666f 7220 664d 5249 2064 6174  ics for fMRI dat
-00000580: 612e 6188 0100 0053 7570 706c 7969 6e67  a.a....Supplying
-00000590: 2061 7267 756d 656e 7473 2069 6e20 7468   arguments in th
-000005a0: 6973 2077 6179 2069 7320 666f 7220 6164  is way is for ad
-000005b0: 7661 6e63 6564 2075 7365 7273 206f 6e6c  vanced users onl
-000005c0: 792e 2049 7420 6973 2072 6563 6f6d 6d65  y. It is recomme
-000005d0: 6e64 6564 2074 6861 7420 7365 7474 696e  nded that settin
-000005e0: 6773 2061 7265 2063 6861 6e67 6564 2075  gs are changed u
-000005f0: 7369 6e67 2074 6865 2047 5549 206f 7220  sing the GUI or 
-00000600: 6279 2065 6469 7469 6e67 2074 6865 2066  by editing the f
-00000610: 5241 545f 636f 6e66 6967 2e74 6f6d 6c20  RAT_config.toml 
-00000620: 6669 6c65 2e20 4172 6775 6d65 6e74 7320  file. Arguments 
-00000630: 7368 6f75 6c64 2062 6520 6769 7665 6e20  should be given 
-00000640: 696e 2074 6f6d 6c20 666f 726d 6174 2e20  in toml format. 
-00000650: 466f 7220 6578 616d 706c 653a 2074 7275  For example: tru
-00000660: 6520 7368 6f75 6c64 2062 6520 7573 6564  e should be used
-00000670: 2069 6e73 7465 6164 206f 6620 5472 7565   instead of True
-00000680: 2061 6e64 2073 7472 696e 6773 2073 686f   and strings sho
-00000690: 756c 6420 6265 2069 6e20 7175 6f74 6174  uld be in quotat
-000006a0: 696f 6e20 6d61 726b 732e 2057 6865 7265  ion marks. Where
-000006b0: 2061 2063 6f6d 6d61 2d73 6570 6172 6174   a comma-separat
-000006c0: 6564 206c 6973 7420 6973 2073 7570 706f  ed list is suppo
-000006d0: 7365 6420 746f 2062 6520 6769 7665 6e2c  sed to be given,
-000006e0: 2074 6869 7320 7368 6f75 6c64 2062 6520   this should be 
-000006f0: 696e 2074 6865 2066 6f72 6d61 743a 205b  in the format: [
-00000700: 226d 6222 2c20 2273 656e 7365 225d 2e29  "mb", "sense"].)
-00000710: 04da 0470 726f 67da 0575 7361 6765 da0b  ...prog..usage..
-00000720: 6465 7363 7269 7074 696f 6eda 0665 7069  description..epi
-00000730: 6c6f 677a 0c2d 2d6d 616b 655f 7461 626c  logz.--make_tabl
-00000740: 65da 0a6d 616b 655f 7461 626c 657a a874  e..make_tablez.t
-00000750: 7275 6520 6f72 2066 616c 7365 2e20 5573  rue or false. Us
-00000760: 6520 7468 6973 2066 6c61 6720 746f 2063  e this flag to c
-00000770: 7265 6174 6520 6120 6373 7620 6669 6c65  reate a csv file
-00000780: 2074 6f20 7374 6f72 6520 7061 7261 6d65   to store parame
-00000790: 7465 7220 696e 666f 726d 6174 696f 6e20  ter information 
-000007a0: 6162 6f75 7420 6669 6c65 732e 2052 6563  about files. Rec
-000007b0: 6f6d 6d65 6e64 6564 2074 6861 7420 7468  ommended that th
-000007c0: 6973 2066 696c 6520 6973 2063 7265 6174  is file is creat
-000007d0: 6564 2061 6e64 2066 696c 6c65 6420 696e  ed and filled in
-000007e0: 2062 6566 6f72 6520 6652 4154 2065 7865   before fRAT exe
-000007f0: 6375 7469 6f6e 2e29 02da 0464 6573 74da  cution.)...dest.
-00000800: 0468 656c 70e9 0100 0000 da04 7479 7065  .help.......type
-00000810: da06 4275 7474 6f6e da0b 4465 7363 7269  ..Button..Descri
-00000820: 7074 696f 6efa 0125 7a02 2525 da00 7a13  ption..%z.%%..z.
-00000830: 5265 636f 6d6d 656e 6465 6420 7661 6c75  Recommended valu
-00000840: 653a 20da 0b52 6563 6f6d 6d65 6e64 6564  e: ..Recommended
-00000850: 7a02 2d2d 2908 da08 6172 6770 6172 7365  z.--)...argparse
-00000860: da0e 4172 6775 6d65 6e74 5061 7273 6572  ..ArgumentParser
-00000870: da0c 6164 645f 6172 6775 6d65 6e74 da05  ..add_argument..
-00000880: 7061 6765 73da 0465 7661 6cda 0772 6570  pages..eval..rep
-00000890: 6c61 6365 da08 4b65 7945 7272 6f72 da0a  lace..KeyError..
-000008a0: 7061 7273 655f 6172 6773 2906 da06 7061  parse_args)...pa
-000008b0: 7273 6572 5a0e 6172 675f 6361 7465 676f  rserZ.arg_catego
-000008c0: 7269 6573 da08 6361 7465 676f 7279 da03  ries..category..
-000008d0: 6172 67da 0968 656c 705f 7465 7874 da04  arg..help_text..
-000008e0: 6172 6773 7214 0000 0072 1400 0000 7215  argsr....r....r.
-000008f0: 0000 00da 0961 7267 7061 7273 6572 2800  .....argparser(.
-00000900: 0000 732e 0000 0008 0302 0102 0206 fd08  ..s.............
-00000910: 0c02 0106 ff0c 0508 020c 0114 0102 0202  ................
-00000920: 021c 010c 0104 0102 ff08 0316 0118 0202  ................
-00000930: f308 1004 027a 0f55 7469 6c73 2e61 7267  .....z.Utils.arg
-00000940: 7061 7273 6572 6301 0000 0000 0000 0000  parserc.........
-00000950: 0000 0005 0000 0006 0000 0047 0000 0073  ...........G...s
-00000960: 5200 0000 6700 7d02 7c01 4400 5d22 7d03  R...g.}.|.D.]"}.
-00000970: 7c03 6401 1900 6402 6b02 7211 7c03 a000  |.d...d.k.r.|...
-00000980: 6402 a101 0100 6403 6404 8400 7401 7c00  d.....d.d...t.|.
-00000990: 9b00 6405 7c03 9b00 9d03 8301 4400 8301  ..d.|.......D...
-000009a0: 7d04 7c04 7226 7c02 a002 7c04 a101 0100  }.|.r&|...|.....
-000009b0: 7104 7c02 5300 2906 4e72 0100 0000 da01  q.|.S.).Nr......
-000009c0: 2e63 0100 0000 0000 0000 0000 0000 0200  .c..............
-000009d0: 0000 0500 0000 5300 0000 7318 0000 0067  ......S...s....g
-000009e0: 007c 005d 087d 0174 006a 01a0 027c 01a1  .|.].}.t.j...|..
-000009f0: 0191 0271 0253 0072 1400 0000 2903 da02  ...q.S.r....)...
-00000a00: 6f73 da04 7061 7468 da08 6261 7365 6e61  os..path..basena
-00000a10: 6d65 2902 da02 2e30 da01 6672 1400 0000  me)....0..fr....
-00000a20: 7214 0000 0072 1500 0000 da0a 3c6c 6973  r....r......<lis
-00000a30: 7463 6f6d 703e 5a00 0000 7302 0000 0018  tcomp>Z...s.....
-00000a40: 007a 2455 7469 6c73 2e66 696e 645f 6669  .z$Utils.find_fi
-00000a50: 6c65 732e 3c6c 6f63 616c 733e 2e3c 6c69  les.<locals>.<li
-00000a60: 7374 636f 6d70 3e7a 032f 2a2e 2903 da06  stcomp>z./*.)...
-00000a70: 6c73 7472 6970 7202 0000 00da 0665 7874  lstripr......ext
-00000a80: 656e 6429 05da 0964 6972 6563 746f 7279  end)...directory
-00000a90: da0a 6578 7465 6e73 696f 6e73 da05 6669  ..extensions..fi
-00000aa0: 6c65 73da 0965 7874 656e 7369 6f6e 5a0b  les..extensionZ.
-00000ab0: 7468 6573 655f 6669 6c65 7372 1400 0000  these_filesr....
-00000ac0: 7214 0000 0072 1500 0000 da0a 6669 6e64  r....r......find
-00000ad0: 5f66 696c 6573 5300 0000 7312 0000 0004  _filesS...s.....
-00000ae0: 0208 010c 010a 011c 0204 020a 0102 8004  ................
-00000af0: 027a 1055 7469 6c73 2e66 696e 645f 6669  .z.Utils.find_fi
-00000b00: 6c65 7363 0100 0000 0000 0000 0000 0000  lesc............
-00000b10: 0300 0000 0400 0000 4300 0000 732c 0000  ........C...s,..
-00000b20: 0069 007d 017c 006a 0044 005d 0e7d 027c  .i.}.|.j.D.].}.|
-00000b30: 007c 0219 00a0 01a1 00a0 02a1 00a0 03a1  .|..............
-00000b40: 007c 017c 023c 0071 057c 0153 00a9 014e  .|.|.<.q.|.S...N
-00000b50: 2904 da07 636f 6c75 6d6e 73da 0664 726f  )...columns..dro
-00000b60: 706e 61da 0874 6f5f 6e75 6d70 79da 0674  pna..to_numpy..t
-00000b70: 6f6c 6973 7429 03da 0964 6174 6166 7261  olist)...datafra
-00000b80: 6d65 da07 726f 6964 6963 74da 0663 6f6c  me..roidict..col
-00000b90: 756d 6e72 1400 0000 7214 0000 0072 1500  umnr....r....r..
-00000ba0: 0000 da11 6461 7461 6672 616d 655f 746f  ....dataframe_to
-00000bb0: 5f64 6963 7461 0000 0073 0800 0000 0402  _dicta...s......
-00000bc0: 0a01 1a01 0402 7a17 5574 696c 732e 6461  ......z.Utils.da
-00000bd0: 7461 6672 616d 655f 746f 5f64 6963 7463  taframe_to_dictc
-00000be0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000bf0: 0400 0000 4300 0000 7314 0000 0074 006a  ....C...s....t.j
-00000c00: 016a 027c 0064 0164 028d 02a0 03a1 0053  .j.|.d.d.......S
-00000c10: 0029 034e da05 696e 6465 7829 01da 066f  .).N..index)...o
-00000c20: 7269 656e 7429 04da 0270 64da 0944 6174  rient)...pd..Dat
-00000c30: 6146 7261 6d65 da09 6672 6f6d 5f64 6963  aFrame..from_dic
-00000c40: 74da 0974 7261 6e73 706f 7365 2901 7247  t..transpose).rG
-00000c50: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00000c60: 0000 da11 6469 6374 5f74 6f5f 6461 7461  ....dict_to_data
-00000c70: 6672 616d 6569 0000 00f3 0200 0000 1402  framei..........
-00000c80: 7a17 5574 696c 732e 6469 6374 5f74 6f5f  z.Utils.dict_to_
-00000c90: 6461 7461 6672 616d 6572 2300 0000 4663  dataframer#...Fc
-00000ca0: 0200 0000 0000 0000 0000 0000 0400 0000  ................
-00000cb0: 0300 0000 4300 0000 735c 0000 0074 0083  ....C...s\...t..
-00000cc0: 007d 027c 02a0 01a1 0001 0074 026a 037c  .}.|.......t.j.|
-00000cd0: 0064 018d 017d 037c 02a0 04a1 0001 007c  .d...}.|.......|
-00000ce0: 0373 1774 0564 0283 0182 017c 0172 1e74  .s.t.d.....|.r.t
-00000cf0: 06a0 077c 03a1 0101 0074 0864 0075 0073  ...|.....t.d.u.s
-00000d00: 2574 086a 0972 2c74 0a64 037c 039b 009d  %t.j.r,t.d.|....
-00000d10: 0283 0101 007c 0353 0029 044e 2901 720b  .....|.S.).N).r.
-00000d20: 0000 007a 134e 6f20 666f 6c64 6572 2073  ...z.No folder s
-00000d30: 656c 6563 7465 642e 7a14 5365 6c65 6374  elected.z.Select
-00000d40: 6564 2064 6972 6563 746f 7279 3a20 290b  ed directory: ).
-00000d50: 7204 0000 00da 0877 6974 6864 7261 7772  r......withdrawr
-00000d60: 0500 0000 5a0c 6173 6b64 6972 6563 746f  ....Z.askdirecto
-00000d70: 7279 da07 6465 7374 726f 79da 1146 696c  ry..destroy..Fil
-00000d80: 654e 6f74 466f 756e 6445 7272 6f72 7234  eNotFoundErrorr4
-00000d90: 0000 00da 0563 6864 6972 da06 636f 6e66  .....chdir..conf
-00000da0: 6967 da07 7665 7262 6f73 65da 0570 7269  ig..verbose..pri
-00000db0: 6e74 2904 720b 0000 0072 5500 0000 da04  nt).r....rU.....
-00000dc0: 726f 6f74 723c 0000 0072 1400 0000 7214  rootr<...r....r.
-00000dd0: 0000 0072 1500 0000 da0c 6669 6c65 5f62  ...r......file_b
-00000de0: 726f 7773 6572 6d00 0000 7316 0000 0006  rowserm...s.....
-00000df0: 0208 010c 0208 0204 0208 0104 020a 010e  ................
-00000e00: 020e 0104 027a 1255 7469 6c73 2e66 696c  .....z.Utils.fil
-00000e10: 655f 6272 6f77 7365 7263 0200 0000 0000  e_browserc......
-00000e20: 0000 0000 0000 0400 0000 0500 0000 4700  ..............G.
-00000e30: 0000 732c 0000 007c 0244 005d 117d 037c  ..s,...|.D.].}.|
-00000e40: 0172 0a74 007c 0383 0101 007c 00a0 0174  .r.t.|.....|...t
-00000e50: 027c 0383 0164 0117 00a1 0101 0071 0264  .|...d.......q.d
-00000e60: 0053 0029 024e da01 0a29 0372 5800 0000  .S.).N...).rX...
-00000e70: da05 7772 6974 65da 0373 7472 2904 da0b  ..write..str)...
-00000e80: 6669 6c65 5f6f 626a 6563 745a 1170 7269  file_objectZ.pri
-00000e90: 6e74 5f74 6f5f 7465 726d 696e 616c 7231  nt_to_terminalr1
-00000ea0: 0000 00da 046c 696e 6572 1400 0000 7214  .....liner....r.
-00000eb0: 0000 0072 1500 0000 da0e 7072 696e 745f  ...r......print_
-00000ec0: 616e 645f 7361 7665 8100 0000 730a 0000  and_save....s...
-00000ed0: 0008 0204 0108 0114 0104 fd7a 1455 7469  ...........z.Uti
-00000ee0: 6c73 2e70 7269 6e74 5f61 6e64 5f73 6176  ls.print_and_sav
-00000ef0: 654e da03 616c 6cda 0a63 6f6e 6669 675f  eN..all..config_
-00000f00: 6c6f 6763 0600 0000 0000 0000 0000 0000  logc............
-00000f10: 0a00 0000 0900 0000 4300 0000 7320 0100  ........C...s ..
-00000f20: 0074 007c 009b 0064 017c 059b 0064 029d  .t.|...d.|...d..
-00000f30: 0464 0383 028f 7b7d 0674 007c 019b 0064  .d....{}.t.|...d
-00000f40: 017c 029b 009d 0364 0483 028f 587d 077c  .|.....d....X}.|
-00000f50: 06a0 0164 0574 029b 0064 067c 029b 0064  ...d.t...d.|...d
-00000f60: 079d 05a1 0101 007c 0372 347c 0344 005d  .......|.r4|.D.]
-00000f70: 077d 087c 06a0 017c 08a1 0101 0071 277c  .}.|...|.....q'|
-00000f80: 06a0 0164 08a1 0101 007c 06a0 0164 08a1  ...d.....|...d..
-00000f90: 0101 0064 007d 097c 0744 005d 297d 087c  ...d.}.|.D.])}.|
-00000fa0: 08a0 0364 09a1 0172 537c 08a0 0364 0aa1  ...d...rS|...d..
-00000fb0: 0173 537c 08a0 0464 0964 0ba1 0264 0c64  .sS|...d.d...d.d
-00000fc0: 0d85 0219 007d 097c 0464 0e6b 0272 5d7c  .....}.|.d.k.r]|
-00000fd0: 06a0 017c 08a1 0101 0071 3d7c 097c 0476  ...|.....q=|.|.v
-00000fe0: 0072 667c 06a0 017c 08a1 0101 0071 3d57  .rf|...|.....q=W
-00000ff0: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
-00001000: 7177 0101 0001 0001 0059 0001 0057 0064  qw.......Y...W.d
-00001010: 0004 0004 0083 0301 0064 0053 0057 0064  .........d.S.W.d
-00001020: 0004 0004 0083 0301 0064 0053 0031 0073  .........d.S.1.s
-00001030: 8977 0101 0001 0001 0059 0001 0064 0053  .w.......Y...d.S
-00001040: 0029 0f4e fa01 2f7a 052e 746f 6d6c da01  .).N../z..toml..
-00001050: 77da 0172 7a20 2320 4765 6e65 7261 6c20  w..rz # General 
-00001060: 696e 666f 726d 6174 696f 6e0a 7665 7273  information.vers
-00001070: 696f 6e20 3d20 7a15 0a63 6f6e 6669 675f  ion = z..config_
-00001080: 6669 6c65 5f75 7365 6420 3d20 277a 0227  file_used = 'z.'
-00001090: 0a72 5b00 0000 fa01 237a 0223 2372 2300  .r[.....#z.##r#.
-000010a0: 0000 721e 0000 00e9 ffff ffff 7261 0000  ..r.........ra..
-000010b0: 0029 05da 046f 7065 6e72 5c00 0000 da07  .)...openr\.....
-000010c0: 7665 7273 696f 6eda 0a73 7461 7274 7377  version..startsw
-000010d0: 6974 6872 2a00 0000 290a 5a06 6e65 7764  ithr*...).Z.newd
-000010e0: 6972 da0b 636f 6e66 6967 5f70 6174 68da  ir..config_path.
-000010f0: 0f63 6f6e 6669 675f 6669 6c65 6e61 6d65  .config_filename
-00001100: da0f 6164 6469 7469 6f6e 616c 5f69 6e66  ..additional_inf
-00001110: 6fda 1172 656c 6576 616e 745f 7365 6374  o..relevant_sect
-00001120: 696f 6e73 da0f 6e65 775f 636f 6e66 6967  ions..new_config
-00001130: 5f6e 616d 6572 3800 0000 7265 0000 0072  _namer8...re...r
-00001140: 5f00 0000 5a0f 6375 7272 656e 745f 7365  _...Z.current_se
-00001150: 6374 696f 6e72 1400 0000 7214 0000 0072  ctionr....r....r
-00001160: 1500 0000 da0b 7361 7665 5f63 6f6e 6669  ......save_confi
-00001170: 6788 0000 0073 2c00 0000 2e02 0601 0201  g....s,.........
-00001180: 04ff 0202 0afe 0404 0801 0c01 0a02 0a02  ................
-00001190: 0402 0801 1401 1401 0802 0c01 0801 0a01  ................
-000011a0: 0280 02f9 50f2 7a11 5574 696c 732e 7361  ....P.z.Utils.sa
-000011b0: 7665 5f63 6f6e 6669 6754 6306 0000 0000  ve_configTc.....
-000011c0: 0000 0000 0000 0007 0000 0006 0000 0043  ...............C
-000011d0: 0000 0073 9c00 0000 7c01 a000 6401 a101  ...s....|...d...
-000011e0: 7309 7c01 6401 3700 7d01 7c02 a000 6401  s.|.d.7.}.|...d.
-000011f0: a101 7312 7c02 6401 3700 7d02 7c05 7217  ..s.|.d.7.}.|.r.
-00001200: 6402 7d06 6e02 7c00 7d06 7c03 723e 7c04  d.}.n.|.}.|.r>|.
-00001210: 722e 7401 a002 7c01 9b00 7c00 9b00 9d02  r.t...|...|.....
-00001220: 7c02 9b00 6403 7c06 9b00 9d03 a102 0100  |...d.|.........
-00001230: 6400 5300 7401 a002 7c01 9b00 7c00 9b00  d.S.t...|...|...
-00001240: 9d02 7c02 9b00 7c06 9b00 9d02 a102 0100  ..|...|.........
-00001250: 6400 5300 7403 a004 7c01 9b00 7c00 9b00  d.S.t...|...|...
-00001260: 9d02 7c02 9b00 7c06 9b00 9d02 a102 0100  ..|...|.........
-00001270: 6400 5300 2904 4e72 6300 0000 7a0f 7061  d.S.).Nrc...z.pa
-00001280: 7261 6d56 616c 7565 732e 6373 765a 0563  ramValues.csvZ.c
-00001290: 6f70 795f 2905 da08 656e 6473 7769 7468  opy_)...endswith
-000012a0: da06 7368 7574 696c da04 636f 7079 7234  ..shutil..copyr4
-000012b0: 0000 00da 0672 656e 616d 6529 07da 086f  .....rename)...o
-000012c0: 6c64 5f6e 616d 655a 0c6f 7269 6769 6e61  ld_nameZ.origina
-000012d0: 6c5f 6469 725a 076e 6577 5f64 6972 7273  l_dirZ.new_dirrs
-000012e0: 0000 00da 0b72 656e 616d 655f 636f 7079  .....rename_copy
-000012f0: da0e 7061 7261 6d65 7465 725f 6669 6c65  ..parameter_file
-00001300: da08 6e65 775f 6e61 6d65 7214 0000 0072  ..new_namer....r
-00001310: 1400 0000 7215 0000 00da 096d 6f76 655f  ....r......move_
-00001320: 6669 6c65 a100 0000 7318 0000 000a 0208  file....s.......
-00001330: 010a 0208 0104 0206 0104 0204 0204 0122  ..............."
-00001340: 0120 0220 027a 0f55 7469 6c73 2e6d 6f76  . . .z.Utils.mov
-00001350: 655f 6669 6c65 6302 0000 0000 0000 0000  e_filec.........
-00001360: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00001370: 4600 0000 7c01 7214 7400 6a01 a002 7c00  F...|.r.t.j...|.
-00001380: a101 7214 7403 a004 7c00 a101 0100 7405  ..r.t...|.....t.
-00001390: a006 7c00 a101 0100 6400 5300 7400 6a01  ..|.....d.S.t.j.
-000013a0: a002 7c00 a101 7321 7405 a006 7c00 a101  ..|...s!t...|...
-000013b0: 0100 6400 5300 6400 5300 7241 0000 0029  ..d.S.d.S.rA...)
-000013c0: 0772 3400 0000 7235 0000 00da 0665 7869  .r4...r5.....exi
-000013d0: 7374 7372 7200 0000 da06 726d 7472 6565  stsrr.....rmtree
-000013e0: 7208 0000 00da 066d 6b5f 6469 7229 0272  r......mk_dir).r
-000013f0: 3500 0000 da0a 6465 6c65 7465 5f6f 6c64  5.....delete_old
-00001400: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00001410: 1263 6865 636b 5f61 6e64 5f6d 616b 655f  .check_and_make_
-00001420: 6469 72b6 0000 0073 0c00 0000 1002 0a01  dir....s........
-00001430: 0e01 0c02 0e01 04ff 7a18 5574 696c 732e  ........z.Utils.
-00001440: 6368 6563 6b5f 616e 645f 6d61 6b65 5f64  check_and_make_d
-00001450: 6972 6303 0000 0000 0000 0000 0000 0007  irc.............
-00001460: 0000 0008 0000 0003 0000 0073 4201 0000  ...........sB...
-00001470: 7c02 6401 6b02 7269 6700 7d03 7400 6402  |.d.k.rig.}.t.d.
-00001480: 8301 0100 7401 8800 8301 4400 5d0d 5c02  ....t.....D.].\.
-00001490: 7d04 7d05 7400 6403 6a02 7c04 7c05 6404  }.}.t.d.j.|.|.d.
-000014a0: 8d02 8301 0100 710e 7c03 7368 7400 6405  ......q.|.sht.d.
-000014b0: 7c01 9b00 6406 9d03 8301 0100 7403 6407  |...d.......t.d.
-000014c0: 8301 7d06 7c06 a004 a100 6408 6b02 723a  ..}.|.....d.k.r:
-000014d0: 7405 7406 6409 7407 8800 8301 8302 8301  t.t.d.t.........
-000014e0: 7d03 6e2c 7407 7c06 8301 6409 6b04 7263  }.n,t.|...d.k.rc
-000014f0: 640a 640b 8400 7c06 a008 640c a101 4400  d.d...|...d...D.
-00001500: 8301 7d03 7a09 7405 7409 740a 7c03 8302  ..}.z.t.t.t.|...
-00001510: 8301 7d03 5700 6e12 0400 740b 7962 0100  ..}.W.n...t.yb..
-00001520: 0100 0100 7400 640d 8301 0100 6700 7d03  ....t.d.....g.}.
-00001530: 5900 6e04 7700 6700 7d03 7196 7c03 721e  Y.n.w.g.}.q.|.r.
-00001540: 6e2d 740c 7c02 7405 8302 7287 740c 7c02  n-t.|.t...r.t.|.
-00001550: 6409 1900 740d 8302 7287 7c02 6409 1900  d...t...r.|.d...
-00001560: a004 a100 6408 6b02 7287 7405 7406 6409  ....d.k.r.t.t.d.
-00001570: 7407 8800 8301 8302 8301 7d03 6e0f 7c02  t.........}.n.|.
-00001580: 7d03 740c 7c03 740a 8302 7292 7c03 6701  }.t.|.t...r.|.g.
-00001590: 7d03 6e04 7405 7c03 8301 7d03 8700 6601  }.n.t.|...}...f.
-000015a0: 640e 640b 8408 7c03 4400 8301 7d03 7c03  d.d...|.D...}.|.
-000015b0: 5300 290f 4eda 0752 756e 7469 6d65 725b  S.).N..Runtimer[
-000015c0: 0000 007a 107b 726f 695f 6e75 6d7d 3a20  ...z.{roi_num}: 
-000015d0: 7b72 6f69 7d29 02da 0772 6f69 5f6e 756d  {roi})...roi_num
-000015e0: da03 726f 697a 050a 2d2d 2d20 7a0d 2063  ..roiz..--- z. c
-000015f0: 7265 6174 696f 6e20 2d2d 2d7a b854 7970  reation ---z.Typ
-00001600: 6520 6120 636f 6d6d 612d 7365 7061 7261  e a comma-separa
-00001610: 7465 6420 6c69 7374 206f 6620 7468 6520  ted list of the 
-00001620: 524f 4973 2028 6c69 7374 6564 2061 626f  ROIs (listed abo
-00001630: 7665 2920 796f 7520 7761 6e74 2074 6f20  ve) you want to 
-00001640: 7072 6f64 7563 6520 6120 6669 6775 7265  produce a figure
-00001650: 2066 6f72 2c20 2765 2e67 2e20 322c 2031   for, 'e.g. 2, 1
-00001660: 352c 2037 2c20 3233 2720 6f72 2027 616c  5, 7, 23' or 'al
-00001670: 6c27 2066 6f72 2061 6c6c 2072 6f69 732e  l' for all rois.
-00001680: 200a 416c 7465 726e 6174 6976 656c 7920   .Alternatively 
-00001690: 7072 6573 7320 656e 7465 7220 7477 6963  press enter twic
-000016a0: 6520 746f 2073 6b69 7020 7468 6973 2073  e to skip this s
-000016b0: 7465 703a 2072 6100 0000 7201 0000 0063  tep: ra...r....c
-000016c0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000016d0: 0400 0000 5300 0000 f314 0000 0067 007c  ....S........g.|
-000016e0: 005d 067d 017c 01a0 00a1 0091 0271 0253  .].}.|.......q.S
-000016f0: 0072 1400 0000 2901 da05 7374 7269 70a9  .r....)...strip.
-00001700: 0272 3700 0000 7213 0000 0072 1400 0000  .r7...r....r....
-00001710: 7214 0000 0072 1500 0000 7239 0000 00d2  r....r....r9....
-00001720: 0000 00f3 0200 0000 1400 7a2a 5574 696c  ..........z*Util
-00001730: 732e 6669 6e64 5f63 686f 7365 6e5f 726f  s.find_chosen_ro
-00001740: 6973 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  is.<locals>.<lis
-00001750: 7463 6f6d 703e fa01 2c7a 2c43 6f6d 6d61  tcomp>..,z,Comma
-00001760: 2d73 6570 6172 6174 6564 206c 6973 7420  -separated list 
-00001770: 636f 6e74 6169 6e73 206e 6f6e 2069 6e74  contains non int
-00001780: 6567 6572 732e 0a63 0100 0000 0000 0000  egers..c........
-00001790: 0000 0000 0200 0000 0400 0000 1300 0000  ................
-000017a0: 7314 0000 0067 007c 005d 067d 0188 007c  s....g.|.].}...|
-000017b0: 0119 0091 0271 0253 0072 1400 0000 7214  .....q.S.r....r.
-000017c0: 0000 0029 0272 3700 0000 5a0a 726f 695f  ...).r7...Z.roi_
-000017d0: 6e75 6d62 6572 a901 da08 616c 6c5f 726f  number....all_ro
-000017e0: 6973 7214 0000 0072 1500 0000 7239 0000  isr....r....r9..
-000017f0: 00ea 0000 0072 8500 0000 290e 7258 0000  .....r....).rX..
-00001800: 00da 0965 6e75 6d65 7261 7465 da06 666f  ...enumerate..fo
-00001810: 726d 6174 da05 696e 7075 74da 056c 6f77  rmat..input..low
-00001820: 6572 7210 0000 00da 0572 616e 6765 da03  err......range..
-00001830: 6c65 6eda 0573 706c 6974 da03 6d61 70da  len..split..map.
-00001840: 0369 6e74 7211 0000 0072 0e00 0000 725d  .intr....r....r]
-00001850: 0000 0029 0772 8800 0000 da09 6675 6e63  ...).r......func
-00001860: 5f6e 616d 655a 1163 6f6e 6669 675f 7265  _nameZ.config_re
-00001870: 6769 6f6e 5f76 6172 5a0b 6368 6f73 656e  gion_varZ.chosen
-00001880: 5f72 6f69 7372 8000 0000 7281 0000 005a  _roisr....r....Z
-00001890: 0772 6f69 5f61 6e73 7214 0000 0072 8700  .roi_ansr....r..
-000018a0: 0000 7215 0000 00da 1066 696e 645f 6368  ..r......find_ch
-000018b0: 6f73 656e 5f72 6f69 73bf 0000 0073 4400  osen_rois....sD.
-000018c0: 0000 0802 0401 0801 1002 1401 0402 1001  ................
-000018d0: 0201 0201 04ff 0c04 1401 0c02 1401 0202  ................
-000018e0: 1201 0c01 0801 0801 02fe 0405 0201 04ec  ................
-000018f0: 0280 1817 0e01 02ff 1402 0402 0a02 0801  ................
-00001900: 0802 1202 0402 7a16 5574 696c 732e 6669  ......z.Utils.fi
-00001910: 6e64 5f63 686f 7365 6e5f 726f 6973 6302  nd_chosen_roisc.
-00001920: 0000 0000 0000 0000 0000 0004 0000 0008  ................
-00001930: 0000 0043 0000 0073 7e00 0000 7400 a001  ...C...s~...t...
-00001940: a100 7d02 6401 7d03 7a1f 7c01 6402 6b02  ..}.d.}.z.|.d.k.
-00001950: 7216 7c00 9b00 6403 9d02 7d03 7400 a002  r.|...d...}.t...
-00001960: 7c03 a101 7d02 6e0e 7c01 6404 6b02 7224  |...}.n.|.d.k.r$
-00001970: 7c00 9b00 6405 9d02 7d03 7400 a002 7c03  |...d...}.t...|.
-00001980: a101 7d02 5700 6e10 0400 7403 7935 0100  ..}.W.n...t.y5..
-00001990: 0100 0100 7404 6406 7405 6a06 9b00 6407  ....t.d.t.j...d.
-000019a0: 9d03 8301 8201 7700 7c02 a007 6408 a101  ......w.|...d...
-000019b0: 7d02 7c02 7c03 6602 5300 2909 4e72 2300  }.|.|.f.S.).Nr#.
-000019c0: 0000 fa10 5365 7373 696f 6e20 6176 6572  ....Session aver
-000019d0: 6167 6564 7a4a 2f4f 7665 7261 6c6c 2f53  agedzJ/Overall/S
-000019e0: 756d 6d61 7269 7365 645f 7265 7375 6c74  ummarised_result
-000019f0: 732f 5365 7373 696f 6e5f 6176 6572 6167  s/Session_averag
-00001a00: 6564 5f72 6573 756c 7473 2f63 6f6d 6269  ed_results/combi
-00001a10: 6e65 645f 7265 7375 6c74 732e 6a73 6f6e  ned_results.json
-00001a20: fa14 5061 7274 6963 6970 616e 7420 6176  ..Participant av
-00001a30: 6572 6167 6564 7a4e 2f4f 7665 7261 6c6c  eragedzN/Overall
-00001a40: 2f53 756d 6d61 7269 7365 645f 7265 7375  /Summarised_resu
-00001a50: 6c74 732f 5061 7274 6963 6970 616e 745f  lts/Participant_
-00001a60: 6176 6572 6167 6564 5f72 6573 756c 7473  averaged_results
-00001a70: 2f63 6f6d 6269 6e65 645f 7265 7375 6c74  /combined_result
-00001a80: 732e 6a73 6f6e 7a23 636f 6d62 696e 6564  s.jsonz#combined
-00001a90: 5f72 6573 756c 7473 2e6a 736f 6e20 6e6f  _results.json no
-00001aa0: 7420 666f 756e 6420 696e 207a 0820 666f  t found in z. fo
-00001ab0: 6c64 6572 2e72 4a00 0000 2908 724c 0000  lder.rJ...).rL..
-00001ac0: 0072 4d00 0000 da09 7265 6164 5f6a 736f  .rM.....read_jso
-00001ad0: 6e72 1100 0000 da09 4578 6365 7074 696f  nr......Exceptio
-00001ae0: 6e72 5600 0000 da0e 6176 6572 6167 696e  nrV.....averagin
-00001af0: 675f 7479 7065 da0b 736f 7274 5f76 616c  g_type..sort_val
-00001b00: 7565 7329 04da 0666 6f6c 6465 7272 9800  ues)...folderr..
-00001b10: 0000 da02 6466 7235 0000 0072 1400 0000  ....dfr5...r....
-00001b20: 7214 0000 0072 1500 0000 da15 7265 6164  r....r......read
-00001b30: 5f63 6f6d 6269 6e65 645f 7265 7375 6c74  _combined_result
-00001b40: 73ee 0000 0073 1e00 0000 0802 0401 0202  s....s..........
-00001b50: 0801 0a01 0c01 0802 0a01 0a01 0480 0c02  ................
-00001b60: 1201 02ff 0a03 0802 7a1b 5574 696c 732e  ........z.Utils.
-00001b70: 7265 6164 5f63 6f6d 6269 6e65 645f 7265  read_combined_re
-00001b80: 7375 6c74 7363 0100 0000 0000 0000 0000  sultsc..........
-00001b90: 0000 0500 0000 0900 0000 0300 0000 73c2  ..............s.
-00001ba0: 0000 0064 0164 0284 007c 006a 0044 0083  ...d.d...|.j.D..
-00001bb0: 017c 005f 0074 0164 0364 0484 0074 027c  .|._.t.d.d...t.|
-00001bc0: 006a 0083 0144 0083 0164 0583 027d 0174  .j...D...d...}.t
-00001bd0: 0164 0664 0484 0074 027c 006a 0083 0144  .d.d...t.|.j...D
-00001be0: 0083 0164 0583 027d 027c 0273 2e74 0364  ...d...}.|.s.t.d
-00001bf0: 0774 046a 059b 0064 089d 0383 0182 0167  .t.j...d.......g
-00001c00: 007d 0374 046a 0644 005d 2889 0074 0187  .}.t.j.D.](..t..
-00001c10: 0066 0164 0964 0484 0874 027c 006a 0083  .f.d.d...t.|.j..
-00001c20: 0144 0083 0164 0583 027d 047c 0472 4c7c  .D...d...}.|.rL|
-00001c30: 03a0 077c 04a1 0101 0071 3374 0864 0a88  ...|.....q3t.d..
-00001c40: 009b 0064 0b74 046a 059b 0064 0c74 046a  ...d.t.j...d.t.j
-00001c50: 059b 0064 0d9d 0783 0182 017c 017c 037c  ...d.......|.|.|
-00001c60: 0266 0353 0029 0e4e 6301 0000 0000 0000  .f.S.).Nc.......
-00001c70: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00001c80: 0072 8200 0000 7214 0000 00a9 0172 8c00  .r....r......r..
-00001c90: 0000 7284 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00001ca0: 0072 1500 0000 7239 0000 0005 0100 0072  .r....r9.......r
-00001cb0: 8500 0000 7a2a 5574 696c 732e 6669 6e64  ....z*Utils.find
-00001cc0: 5f63 6f6c 756d 6e5f 6c6f 6373 2e3c 6c6f  _column_locs.<lo
-00001cd0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00001ce0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00001cf0: 0003 0000 0073 0000 00f3 2000 0000 8100  .....s.... .....
-00001d00: 7c00 5d0b 5c02 7d01 7d02 6400 7c02 7600  |.].\.}.}.d.|.v.
-00001d10: 7202 7c01 5600 0100 7102 6401 5300 2902  r.|.V...q.d.S.).
-00001d20: 7a0b 6967 6e6f 7265 2066 696c 654e 7214  z.ignore fileNr.
-00001d30: 0000 00a9 0372 3700 0000 da07 636f 756e  .....r7.....coun
-00001d40: 7465 7272 4800 0000 7214 0000 0072 1400  terrH...r....r..
-00001d50: 0000 7215 0000 00da 093c 6765 6e65 7870  ..r......<genexp
-00001d60: 723e 0701 0000 7304 0000 0002 801e 007a  r>....s........z
-00001d70: 2955 7469 6c73 2e66 696e 645f 636f 6c75  )Utils.find_colu
-00001d80: 6d6e 5f6c 6f63 732e 3c6c 6f63 616c 733e  mn_locs.<locals>
-00001d90: 2e3c 6765 6e65 7870 723e 4663 0100 0000  .<genexpr>Fc....
-00001da0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00001db0: 7300 0000 729e 0000 0029 02da 0862 6173  s...r....)...bas
-00001dc0: 656c 696e 654e 7214 0000 0072 9f00 0000  elineNr....r....
-00001dd0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00001de0: a100 0000 0a01 0000 7308 0000 0002 800a  ........s.......
-00001df0: 0006 010e ff7a 1c4e 6f20 6261 7365 6c69  .....z.No baseli
-00001e00: 6e65 2063 6f6c 756d 6e20 666f 756e 6420  ne column found 
-00001e10: 696e 2072 3300 0000 6301 0000 0000 0000  in r3...c.......
-00001e20: 0000 0000 0003 0000 0003 0000 0033 0000  .............3..
-00001e30: 0073 2400 0000 8100 7c00 5d0d 5c02 7d01  .s$.....|.].\.}.
-00001e40: 7d02 8800 a000 a100 7c02 6b02 7202 7c01  }.......|.k.r.|.
-00001e50: 5600 0100 7102 6400 5300 7241 0000 0072  V...q.d.S.rA...r
-00001e60: 9d00 0000 729f 0000 00a9 01da 036b 6579  ....r........key
-00001e70: 7214 0000 0072 1500 0000 72a1 0000 0011  r....r....r.....
-00001e80: 0100 0073 0400 0000 0280 2200 7a05 4b65  ...s......".z.Ke
-00001e90: 7920 227a 0f22 206e 6f74 2066 6f75 6e64  y "z." not found
-00001ea0: 2069 6e20 7a76 2e20 4368 6563 6b20 7468   in zv. Check th
-00001eb0: 6520 4372 6974 6963 616c 2050 6172 616d  e Critical Param
-00001ec0: 6574 6572 7320 6f70 7469 6f6e 2069 6e20  eters option in 
-00001ed0: 7468 6520 5061 7273 696e 6720 6d65 6e75  the Parsing menu
-00001ee0: 2028 7061 7261 6d65 7465 725f 6469 6374   (parameter_dict
-00001ef0: 3120 6966 206e 6f74 2075 7369 6e67 2074  1 if not using t
-00001f00: 6865 2047 5549 2920 636f 7272 6563 746c  he GUI) correctl
-00001f10: 7920 6d61 7463 6820 7468 6520 7a09 2068  y match the z. h
-00001f20: 6561 6465 7273 2e29 0972 4200 0000 da04  eaders.).rB.....
-00001f30: 6e65 7874 7289 0000 00da 094e 616d 6545  nextr......NameE
-00001f40: 7272 6f72 7256 0000 0072 7700 0000 da0e  rrorrV...rw.....
-00001f50: 7061 7261 6d65 7465 725f 6469 6374 da06  parameter_dict..
-00001f60: 6170 7065 6e64 7297 0000 0029 05da 0574  appendr....)...t
-00001f70: 6162 6c65 da11 6967 6e6f 7265 5f63 6f6c  able..ignore_col
-00001f80: 756d 6e5f 6c6f 635a 1362 6173 656c 696e  umn_locZ.baselin
-00001f90: 655f 636f 6c75 6d6e 5f6c 6f63 da14 6372  e_column_loc..cr
-00001fa0: 6974 6963 616c 5f63 6f6c 756d 6e5f 6c6f  itical_column_lo
-00001fb0: 6373 5a0a 636f 6c75 6d6e 5f6c 6f63 7214  csZ.column_locr.
-00001fc0: 0000 0072 a300 0000 7215 0000 00da 1066  ...r....r......f
-00001fd0: 696e 645f 636f 6c75 6d6e 5f6c 6f63 7303  ind_column_locs.
-00001fe0: 0100 0073 2400 0000 1202 1402 0201 04ff  ...s$...........
-00001ff0: 1403 0201 04ff 0402 1201 0402 0a01 1e01  ................
-00002000: 0402 0c01 1202 0402 0afe 0a04 7a16 5574  ............z.Ut
-00002010: 696c 732e 6669 6e64 5f63 6f6c 756d 6e5f  ils.find_column_
-00002020: 6c6f 6373 6301 0000 0000 0000 0000 0000  locsc...........
-00002030: 0004 0000 0008 0000 0043 0000 0073 8200  .........C...s..
-00002040: 0000 7c00 7205 7c00 7d01 6e04 7400 a001  ..|.r.|.}.n.t...
-00002050: a100 7d01 7400 6a02 a003 7c01 9b00 6401  ..}.t.j...|...d.
-00002060: 7404 6a05 9b00 9d03 a101 7226 7406 a007  t.j.......r&t...
-00002070: 7c01 9b00 6401 7404 6a05 9b00 9d03 a101  |...d.t.j.......
-00002080: 7d02 6402 7d03 7c02 7c03 6602 5300 7a0f  }.d.}.|.|.f.S.z.
-00002090: 7406 a007 7c01 9b00 6403 9d02 a101 7d02  t...|...d.....}.
-000020a0: 6404 7d03 5700 7c02 7c03 6602 5300 0400  d.}.W.|.|.f.S...
-000020b0: 7408 7940 0100 0100 0100 7409 6405 8301  t.y@......t.d...
-000020c0: 8201 7700 2906 4e72 6300 0000 da0b 6261  ..w.).Nrc.....ba
-000020d0: 7365 5f66 6f6c 6465 727a 152f 636f 7079  se_folderz./copy
-000020e0: 5f70 6172 616d 5661 6c75 6573 2e63 7376  _paramValues.csv
-000020f0: da0d 7265 706f 7274 5f66 6f6c 6465 727a  ..report_folderz
-00002100: b34d 616b 6520 7375 7265 2061 2063 6f70  .Make sure a cop
-00002110: 7920 6f66 2070 6172 616d 5661 6c75 6573  y of paramValues
-00002120: 2e63 7376 2069 7320 696e 2074 6865 2063  .csv is in the c
-00002130: 686f 7365 6e20 666f 6c64 6572 2e20 0a41  hosen folder. .A
-00002140: 6c73 6f20 6d61 6b65 2073 7572 6520 7468  lso make sure th
-00002150: 6520 7365 6c65 6374 6564 2066 6f6c 6465  e selected folde
-00002160: 7220 636f 6e74 6169 6e73 2061 6c6c 2074  r contains all t
-00002170: 6865 2070 6172 7469 6369 7061 6e74 2064  he participant d
-00002180: 6972 6563 746f 7269 6573 2069 6e20 7468  irectories in th
-00002190: 6520 6e65 6365 7373 6172 7920 4249 4453  e necessary BIDS
-000021a0: 2066 6f72 6d61 7420 652e 672e 2073 7562   format e.g. sub
-000021b0: 2d30 312e 290a 7234 0000 00da 0667 6574  -01.).r4.....get
-000021c0: 6377 6472 3500 0000 da06 6973 6669 6c65  cwdr5.....isfile
-000021d0: 7256 0000 0072 7700 0000 724c 0000 00da  rV...rw...rL....
-000021e0: 0872 6561 645f 6373 7672 5400 0000 7297  .read_csvrT...r.
-000021f0: 0000 0029 0472 3c00 0000 729a 0000 0072  ...).r<...r....r
-00002200: a900 0000 da0b 666f 6c64 6572 5f74 7970  ......folder_typ
-00002210: 6572 1400 0000 7214 0000 0072 1500 0000  er....r....r....
-00002220: da15 6c6f 6164 5f70 6172 616d 5661 6c75  ..load_paramValu
-00002230: 6573 5f66 696c 651c 0100 0073 1c00 0000  es_file....s....
-00002240: 0402 0601 0802 1802 1601 0401 080c 02f7  ................
-00002250: 1001 0601 0807 0cfb 0801 02ff 7a1b 5574  ............z.Ut
-00002260: 696c 732e 6c6f 6164 5f70 6172 616d 5661  ils.load_paramVa
-00002270: 6c75 6573 5f66 696c 6563 0100 0000 0000  lues_filec......
-00002280: 0000 0000 0000 0100 0000 0800 0000 4300  ..............C.
-00002290: 0000 7326 0000 007a 0874 00a0 017c 00a1  ..s&...z.t...|..
-000022a0: 0101 0057 0064 0053 0004 0074 0279 1201  ...W.d.S...t.y..
-000022b0: 0001 0001 0059 0064 0053 0077 0072 4100  .....Y.d.S.w.rA.
-000022c0: 0000 2903 7234 0000 00da 056d 6b64 6972  ..).r4.....mkdir
-000022d0: da0f 4669 6c65 4578 6973 7473 4572 726f  ..FileExistsErro
-000022e0: 7229 0172 3500 0000 7214 0000 0072 1400  r).r5...r....r..
-000022f0: 0000 7215 0000 0072 7c00 0000 3301 0000  ..r....r|...3...
-00002300: 730a 0000 0002 0210 010c 0106 0102 ff7a  s..............z
-00002310: 0c55 7469 6c73 2e6d 6b5f 6469 7263 0000  .Utils.mk_dirc..
-00002320: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00002330: 0000 4700 0000 731e 0000 0074 007c 0064  ..G...s....t.|.d
-00002340: 0119 007c 0064 0219 0083 027c 0064 0364  ...|.d.....|.d.d
-00002350: 0085 0219 008e 0053 0029 044e 7201 0000  .......S.).Nr...
-00002360: 0072 1e00 0000 e902 0000 0029 01da 0767  .r.........)...g
-00002370: 6574 6174 7472 a901 da04 6172 6776 7214  etattr....argvr.
-00002380: 0000 0072 1400 0000 7215 0000 00da 1769  ...r....r......i
-00002390: 6e73 7461 6e63 655f 6d65 7468 6f64 5f68  nstance_method_h
-000023a0: 616e 646c 6572 3a01 0000 7302 0000 001e  andler:...s.....
-000023b0: 027a 1d55 7469 6c73 2e69 6e73 7461 6e63  .z.Utils.instanc
-000023c0: 655f 6d65 7468 6f64 5f68 616e 646c 6572  e_method_handler
-000023d0: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-000023e0: 0004 0000 0047 0000 0073 1400 0000 7c00  .....G...s....|.
-000023f0: 6401 1900 7c00 6402 6400 8502 1900 8e00  d...|.d.d.......
-00002400: 5300 2903 4e72 0100 0000 721e 0000 0072  S.).Nr....r....r
-00002410: 1400 0000 72b8 0000 0072 1400 0000 7214  ....r....r....r.
-00002420: 0000 0072 1500 0000 da14 636c 6173 735f  ...r......class_
-00002430: 6d65 7468 6f64 5f68 616e 646c 6572 3e01  method_handler>.
-00002440: 0000 7251 0000 007a 1a55 7469 6c73 2e63  ..rQ...z.Utils.c
-00002450: 6c61 7373 5f6d 6574 686f 645f 6861 6e64  lass_method_hand
-00002460: 6c65 7263 0100 0000 0000 0000 0000 0000  lerc............
-00002470: 0300 0000 0400 0000 4300 0000 734e 0000  ........C...sN..
-00002480: 0074 006a 0164 016b 0272 0a74 02a0 03a1  .t.j.d.k.r.t....
-00002490: 007d 016e 0574 0474 006a 0183 017d 0174  .}.n.t.t.j...}.t
-000024a0: 02a0 0564 02a1 017d 0274 006a 0672 217c  ...d...}.t.j.r!|
-000024b0: 0073 2174 0764 037c 019b 0064 049d 0383  .s!t.d.|...d....
-000024c0: 0101 007c 026a 087c 0164 058d 0153 0029  ...|.j.|.d...S.)
-000024d0: 064e da03 6d61 78da 0a66 6f72 6b73 6572  .N..max..forkser
-000024e0: 7665 727a 200a 5374 6172 7469 6e67 2070  verz .Starting p
-000024f0: 726f 6365 7373 696e 6720 706f 6f6c 2075  rocessing pool u
-00002500: 7369 6e67 207a 0720 636f 7265 732e 2901  sing z. cores.).
-00002510: da09 7072 6f63 6573 7365 7329 0972 5600  ..processes).rV.
-00002520: 0000 5a0e 6d61 785f 636f 7265 5f75 7361  ..Z.max_core_usa
-00002530: 6765 da02 6d70 da09 6370 755f 636f 756e  ge..mp..cpu_coun
-00002540: 7472 9100 0000 da0b 6765 745f 636f 6e74  tr......get_cont
-00002550: 6578 7472 5700 0000 7258 0000 00da 0450  extrW...rX.....P
-00002560: 6f6f 6c29 03da 0772 6573 7461 7274 da07  ool)...restart..
-00002570: 776f 726b 6572 73da 0363 7478 7214 0000  workers..ctxr...
-00002580: 0072 1400 0000 7215 0000 00da 1573 7461  .r....r......sta
-00002590: 7274 5f70 726f 6365 7373 696e 675f 706f  rt_processing_po
-000025a0: 6f6c 4201 0000 730e 0000 000a 020a 010a  olB...s.........
-000025b0: 020a 020a 0210 010c 027a 1b55 7469 6c73  .........z.Utils
-000025c0: 2e73 7461 7274 5f70 726f 6365 7373 696e  .start_processin
-000025d0: 675f 706f 6f6c 6302 0000 0000 0000 0000  g_poolc.........
-000025e0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-000025f0: 2400 0000 7c00 a000 a100 0100 7c00 a001  $...|.......|...
-00002600: a100 0100 7c01 7210 7402 6a03 6401 6402  ....|.r.t.j.d.d.
-00002610: 8d01 7d00 7c00 5300 2903 4e54 2901 72c3  ..}.|.S.).NT).r.
-00002620: 0000 0029 04da 0563 6c6f 7365 da04 6a6f  ...)...close..jo
-00002630: 696e 7208 0000 0072 c600 0000 2902 da04  inr....r....)...
-00002640: 706f 6f6c 72c3 0000 0072 1400 0000 7214  poolr....r....r.
-00002650: 0000 0072 1500 0000 da14 6a6f 696e 5f70  ...r......join_p
-00002660: 726f 6365 7373 696e 675f 706f 6f6c 5001  rocessing_poolP.
-00002670: 0000 730a 0000 0008 0208 0104 020c 0104  ..s.............
-00002680: 027a 1a55 7469 6c73 2e6a 6f69 6e5f 7072  .z.Utils.join_pr
-00002690: 6f63 6573 7369 6e67 5f70 6f6f 6c63 0500  ocessing_poolc..
-000026a0: 0000 0000 0000 0000 0000 0800 0000 0a00  ................
-000026b0: 0000 4300 0000 7318 0100 0074 007c 019b  ..C...s....t.|..
-000026c0: 0064 017c 029b 009d 0364 0283 028f 787d  .d.|.....d....x}
-000026d0: 057a 677c 05a0 01a1 007d 0674 02a0 0364  .zg|.....}.t...d
-000026e0: 03a0 047c 06a1 01a1 017d 067c 0644 005d  ...|.....}.|.D.]
-000026f0: 0c7d 077c 067c 0719 0064 046b 0272 2664  .}.|.|...d.k.r&d
-00002700: 007c 067c 073c 0071 1a7c 0372 2974 0564  .|.|.<.q.|.r)t.d
-00002710: 1069 007c 06a4 018e 0161 0674 076a 08a0  .i.|.....a.t.j..
-00002720: 097c 01a1 0164 0519 0064 066b 0272 5667  .|...d...d.k.rVg
-00002730: 0064 07a2 0167 0064 08a2 0164 099c 0274  .d...g.d...d...t
-00002740: 065f 0a64 0a64 0b84 0074 0b74 0c74 066a  ._.d.d...t.t.t.j
-00002750: 0d83 0183 0144 0083 0174 065f 0e74 0fa0  .....D...t._.t..
-00002760: 1074 06a1 0101 007c 0264 0c6b 0272 697c  .t.....|.d.k.ri|
-00002770: 0474 065f 117c 0474 065f 1264 0d74 065f  .t._.|.t._.d.t._
-00002780: 1364 0e74 065f 1464 0e74 065f 1574 0657  .d.t._.d.t._.t.W
-00002790: 0057 0002 0064 0004 0004 0083 0301 0053  .W...d.........S
-000027a0: 0004 0074 026a 166a 1774 1866 0279 8101  ...t.j.j.t.f.y..
-000027b0: 0001 0001 0074 1964 0f83 0182 0177 0031  .....t.d.....w.1
-000027c0: 0073 8577 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
-000027d0: 0053 0029 114e 7263 0000 0072 6500 0000  .S.).Nrc...re...
-000027e0: 7223 0000 00da 044e 6f6e 6572 6700 0000  r#.....Nonerg...
-000027f0: 5a0c 726f 695f 616e 616c 7973 6973 290b  Z.roi_analysis).
-00002800: 7a0c 546f 7461 6c20 766f 7865 6c73 7a0f  z.Total voxelsz.
-00002810: 4578 636c 7564 6564 2076 6f78 656c 737a  Excluded voxelsz
-00002820: 1a41 7665 7261 6765 2076 6f78 656c 7320  .Average voxels 
-00002830: 7065 7220 7365 7373 696f 6eda 044d 6561  per session..Mea
-00002840: 6eda 0753 7464 5f64 6576 da13 436f 6e66  n..Std_dev..Conf
-00002850: 6964 656e 6365 5f69 6e74 6572 7661 6cda  idence_interval.
-00002860: 064d 6564 6961 6eda 074d 696e 696d 756d  .Median..Minimum
-00002870: da07 4d61 7869 6d75 6dda 0c50 6172 7469  ..Maximum..Parti
-00002880: 6369 7061 6e74 73da 0853 6573 7369 6f6e  cipants..Session
-00002890: 7329 0a5a 0c56 6f78 656c 5f61 6d6f 756e  s).Z.Voxel_amoun
-000028a0: 74da 1645 7863 6c75 6465 645f 766f 7865  t..Excluded_voxe
-000028b0: 6c73 5f61 6d6f 756e 745a 0e41 7665 7261  ls_amountZ.Avera
-000028c0: 6765 5f76 6f78 656c 7372 cc00 0000 5a12  ge_voxelsr....Z.
-000028d0: 5374 616e 6461 7264 5f64 6576 6961 7469  Standard_deviati
-000028e0: 6f6e 72ce 0000 0072 cf00 0000 72d0 0000  onr....r....r...
-000028f0: 0072 d100 0000 72d3 0000 0029 0272 9500  .r....r....).r..
-00002900: 0000 7294 0000 0063 0100 0000 0000 0000  ..r....c........
-00002910: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-00002920: 731e 0000 0069 007c 005d 0b7d 0174 006a  s....i.|.].}.t.j
-00002930: 017c 0119 0074 006a 027c 0119 0093 0271  .|...t.j.|.....q
-00002940: 0253 0072 1400 0000 2903 7256 0000 00da  .S.r....).rV....
-00002950: 0f70 6172 616d 6574 6572 5f64 6963 7431  .parameter_dict1
-00002960: da0f 7061 7261 6d65 7465 725f 6469 6374  ..parameter_dict
-00002970: 3229 0272 3700 0000 da01 6972 1400 0000  2).r7.....ir....
-00002980: 7214 0000 0072 1500 0000 da0a 3c64 6963  r....r......<dic
-00002990: 7463 6f6d 703e 8401 0000 730a 0000 0006  tcomp>....s.....
-000029a0: 0002 0108 ff08 0106 ff7a 2555 7469 6c73  .........z%Utils
-000029b0: 2e6c 6f61 645f 636f 6e66 6967 2e3c 6c6f  .load_config.<lo
-000029c0: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-000029d0: 7a10 7465 7374 5f63 6f6e 6669 672e 746f  z.test_config.to
-000029e0: 6d6c 5a0f 7465 7374 5f52 4f49 5f72 6570  mlZ.test_ROI_rep
-000029f0: 6f72 745a 0974 6573 745f 6d61 7073 7a35  ortZ.test_mapsz5
-00002a00: 436f 6e66 6967 2066 696c 6520 6e6f 7420  Config file not 
-00002a10: 696e 2063 6f72 7265 6374 2066 6f72 6d61  in correct forma
-00002a20: 7420 6f72 206d 6973 7369 6e67 2065 6e74  t or missing ent
-00002a30: 7269 6573 2e72 1400 0000 291a 7268 0000  ries.r....).rh..
-00002a40: 00da 0972 6561 646c 696e 6573 da04 746f  ...readlines..to
-00002a50: 6d6c da05 6c6f 6164 7372 c800 0000 7206  ml..loadsr....r.
-00002a60: 0000 0072 5600 0000 7234 0000 0072 3500  ...rV...r4...r5.
-00002a70: 0000 728f 0000 00da 1173 7461 7469 7374  ..r......statist
-00002a80: 6963 5f6f 7074 696f 6e73 728d 0000 0072  ic_optionsr....r
-00002a90: 8e00 0000 72d5 0000 0072 a700 0000 7208  ....r....r....r.
-00002aa0: 0000 00da 1463 6c65 616e 5f63 6f6e 6669  .....clean_confi
-00002ab0: 675f 6f70 7469 6f6e 73da 0e62 7261 696e  g_options..brain
-00002ac0: 5f66 696c 655f 6c6f 6372 ad00 0000 da0d  _file_locr......
-00002ad0: 6f75 7470 7574 5f66 6f6c 6465 725a 126f  output_folderZ.o
-00002ae0: 7574 7075 745f 666f 6c64 6572 5f6e 616d  utput_folder_nam
-00002af0: 65da 0f73 7461 745f 6d61 705f 666f 6c64  e..stat_map_fold
-00002b00: 6572 da07 6465 636f 6465 72da 0f54 6f6d  er..decoder..Tom
-00002b10: 6c44 6563 6f64 6545 7272 6f72 da0e 4174  lDecodeError..At
-00002b20: 7472 6962 7574 6545 7272 6f72 7297 0000  tributeErrorr...
-00002b30: 0029 08da 0363 6c73 726b 0000 00da 0866  .)...clsrk.....f
-00002b40: 696c 656e 616d 65da 0473 6176 6572 3500  ilename..saver5.
-00002b50: 0000 da08 746f 6d6c 6669 6c65 da05 7061  ....tomlfile..pa
-00002b60: 7273 6572 a400 0000 7214 0000 0072 1400  rser....r....r..
-00002b70: 0000 7215 0000 00da 0b6c 6f61 645f 636f  ..r......load_co
-00002b80: 6e66 6967 5a01 0000 733c 0000 0016 0202  nfigZ...s<......
-00002b90: 0108 0110 0108 020c 0108 0102 8004 020e  ................
-00002ba0: 0314 0206 0206 0c08 f306 190c 0108 ff0a  ................
-00002bb0: 0308 0206 0206 0106 0106 0106 0104 0210  ................
-00002bc0: cb14 3708 0102 ff14 c97a 1155 7469 6c73  ..7......z.Utils
-00002bd0: 2e6c 6f61 645f 636f 6e66 6967 6301 0000  .load_configc...
-00002be0: 0000 0000 0000 0000 0003 0000 0007 0000  ................
-00002bf0: 0043 0000 0073 6e00 0000 6700 6401 a201  .C...sn...g.d...
-00002c00: 7d01 7400 7c00 6a01 8301 7402 7501 7212  }.t.|.j...t.u.r.
-00002c10: 7c01 a003 7c00 6a01 a101 7c00 5f01 6700  |...|.j...|._.g.
-00002c20: 6402 a201 7d02 7400 7c00 6a04 8301 7402  d...}.t.|.j...t.
-00002c30: 7501 7235 6403 7405 6404 7406 a007 6405  u.r5d.t.d.t...d.
-00002c40: 7c00 6a04 a102 6406 1900 9b00 9d02 8301  |.j...d.........
-00002c50: 1800 7c00 5f08 7c02 a003 7c00 6a04 a101  ..|._.|...|.j...
-00002c60: 7c00 5f04 7c00 5300 2907 4e29 0d7a 1343  |._.|.S.).N).z.C
-00002c70: 6572 6562 656c 6c75 6d2d 4d4e 4966 6c69  erebellum-MNIfli
-00002c80: 7274 7a13 4365 7265 6265 6c6c 756d 2d4d  rtz.Cerebellum-M
-00002c90: 4e49 666e 6972 747a 1248 6172 7661 7264  NIfnirtz.Harvard
-00002ca0: 4f78 666f 7264 2d63 6f72 747a 1148 6172  Oxford-cortz.Har
-00002cb0: 7661 7264 4f78 666f 7264 2d73 7562 7a0f  vardOxford-subz.
-00002cc0: 4a48 552d 4943 424d 2d6c 6162 656c 737a  JHU-ICBM-labelsz
-00002cd0: 0f4a 4855 2d49 4342 4d2d 7472 6163 7473  .JHU-ICBM-tracts
-00002ce0: 5a07 6a75 656c 6963 68da 034d 4e49 7a0c  Z.juelich..MNIz.
-00002cf0: 534d 4154 542d 6c61 6265 6c73 da03 5354  SMATT-labels..ST
-00002d00: 4e7a 1373 7472 6961 7475 6d2d 7374 7275  Nz.striatum-stru
-00002d10: 6374 7572 616c 7a10 5461 6c61 6972 6163  cturalz.Talairac
-00002d20: 682d 6c61 6265 6c73 da08 5468 616c 616d  h-labels..Thalam
-00002d30: 7573 2906 7a09 3830 252c 2031 2e32 387a  us).z.80%, 1.28z
-00002d40: 0938 3525 2c20 312e 3434 7a09 3930 252c  .85%, 1.44z.90%,
-00002d50: 2031 2e36 347a 0939 3525 2c20 312e 3936   1.64z.95%, 1.96
-00002d60: 7a09 3938 252c 2032 2e33 337a 0939 3925  z.98%, 2.33z.99%
-00002d70: 2c20 322e 3538 721e 0000 007a 0230 2e72  , 2.58r....z.0.r
-00002d80: 2200 0000 7201 0000 0029 0972 1f00 0000  "...r....).r....
-00002d90: da0c 6174 6c61 735f 6e75 6d62 6572 7291  ..atlas_numberr.
-00002da0: 0000 0072 4a00 0000 da11 636f 6e66 5f6c  ...rJ.....conf_l
-00002db0: 6576 656c 5f6e 756d 6265 72da 0566 6c6f  evel_number..flo
-00002dc0: 6174 da02 7265 728f 0000 00da 0f62 6f6f  at..rer......boo
-00002dd0: 7473 7472 6170 5f61 6c70 6861 2903 7256  tstrap_alpha).rV
-00002de0: 0000 00da 0d61 746c 6173 5f6f 7074 696f  .....atlas_optio
-00002df0: 6e73 5a12 636f 6e66 5f6c 6576 656c 5f6f  nsZ.conf_level_o
-00002e00: 7074 696f 6e73 7214 0000 0072 1400 0000  ptionsr....r....
-00002e10: 7215 0000 0072 dd00 0000 9601 0000 7310  r....r........s.
-00002e20: 0000 0008 020e 050e 0108 020e 0222 010e  ............."..
-00002e30: 0104 027a 1a55 7469 6c73 2e63 6c65 616e  ...z.Utils.clean
-00002e40: 5f63 6f6e 6669 675f 6f70 7469 6f6e 7363  _config_optionsc
-00002e50: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00002e60: 0300 0000 4300 0000 7320 0000 0074 00a0  ....C...s ...t..
-00002e70: 017c 00a1 017d 017c 016a 027d 027c 01a0  .|...}.|.j.}.|..
-00002e80: 03a1 007d 017c 017c 0266 0253 0072 4100  ...}.|.|.f.S.rA.
-00002e90: 0000 2904 da03 6e69 62da 046c 6f61 64da  ..)...nib..load.
-00002ea0: 0668 6561 6465 72da 0967 6574 5f66 6461  .header..get_fda
-00002eb0: 7461 2903 da09 6669 6c65 5f70 6174 68da  ta)...file_path.
-00002ec0: 0464 6174 6172 f500 0000 7214 0000 0072  .datar....r....r
-00002ed0: 1400 0000 7215 0000 00da 0a6c 6f61 645f  ....r......load_
-00002ee0: 6272 6169 6ea8 0100 0073 0800 0000 0a02  brain....s......
-00002ef0: 0602 0801 0802 7a10 5574 696c 732e 6c6f  ......z.Utils.lo
-00002f00: 6164 5f62 7261 696e 6301 0000 0000 0000  ad_brainc.......
-00002f10: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00002f20: 0073 2200 0000 6700 6401 a201 7d01 7c01  .s"...g.d...}.|.
-00002f30: 4400 5d08 7d02 7c00 a000 7c02 6402 a102  D.].}.|...|.d...
-00002f40: 7d00 7106 7c00 5300 2903 4e29 047a 072e  }.q.|.S.).N).z..
-00002f50: 6e69 692e 677a 7a04 2e6e 6969 7a04 2e68  nii.gzz..niiz..h
-00002f60: 6472 7a05 2e6a 736f 6e72 2300 0000 2901  drz..jsonr#...).
-00002f70: 722a 0000 0029 0372 3500 0000 723d 0000  r*...).r5...r=..
-00002f80: 0072 3f00 0000 7214 0000 0072 1400 0000  .r?...r....r....
-00002f90: 7215 0000 00da 0973 7472 6970 5f65 7874  r......strip_ext
-00002fa0: b101 0000 7308 0000 0008 0208 020e 0104  ....s...........
-00002fb0: 027a 0f55 7469 6c73 2e73 7472 6970 5f65  .z.Utils.strip_e
-00002fc0: 7874 6301 0000 0000 0000 0000 0000 0003  xtc.............
-00002fd0: 0000 0004 0000 0043 0000 0073 5c00 0000  .......C...s\...
-00002fe0: 6401 6402 8400 7400 7c00 9b00 6403 9d02  d.d...t.|...d...
-00002ff0: 8301 4400 8301 7d01 6404 6402 8400 7c01  ..D...}.d.d...|.
-00003000: 4400 8301 7d02 7401 7c01 8301 6405 6b02  D...}.t.|...d.k.
-00003010: 721d 7402 6406 8301 8201 7403 6a04 722a  r.t.d.....t.j.r*
-00003020: 7405 6407 7401 7c01 8301 9b00 6408 9d03  t.d.t.|.....d...
-00003030: 8301 0100 7c01 7c02 6602 5300 2909 4e63  ....|.|.f.S.).Nc
-00003040: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00003050: 0600 0000 5300 0000 731c 0000 0067 007c  ....S...s....g.|
-00003060: 005d 0a7d 0174 00a0 0164 007c 01a1 0272  .].}.t...d.|...r
-00003070: 027c 0191 0271 0253 0029 017a 0b73 7562  .|...q.S.).z.sub
-00003080: 2d5b 302d 395d 2b24 2902 72f0 0000 00da  -[0-9]+$).r.....
-00003090: 0673 6561 7263 6829 0272 3700 0000 da05  .search).r7.....
-000030a0: 6469 7265 6372 1400 0000 7214 0000 0072  direcr....r....r
-000030b0: 1500 0000 7239 0000 00bd 0100 0073 0200  ....r9.......s..
-000030c0: 0000 1c00 7a2f 5574 696c 732e 6669 6e64  ....z/Utils.find
-000030d0: 5f70 6172 7469 6369 7061 6e74 5f64 6972  _participant_dir
-000030e0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-000030f0: 636f 6d70 3e7a 022f 2a63 0100 0000 0000  comp>z./*c......
-00003100: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-00003110: 0000 731a 0000 0067 007c 005d 097d 017c  ..s....g.|.].}.|
-00003120: 01a0 0064 00a1 0164 0119 0091 0271 0253  ...d...d.....q.S
-00003130: 0029 0272 6300 0000 7267 0000 0029 0172  .).rc...rg...).r
-00003140: 8f00 0000 2902 7237 0000 00da 0b70 6172  ....).r7.....par
-00003150: 7469 6369 7061 6e74 7214 0000 0072 1400  ticipantr....r..
-00003160: 0000 7215 0000 0072 3900 0000 be01 0000  ..r....r9.......
-00003170: 7302 0000 001a 0072 0100 0000 7a9e 5061  s......r....z.Pa
-00003180: 7274 6963 6970 616e 7420 6469 7265 6374  rticipant direct
-00003190: 6f72 6965 7320 6e6f 7420 666f 756e 642e  ories not found.
-000031a0: 0a4d 616b 6520 7375 7265 2070 6172 7469  .Make sure parti
-000031b0: 6369 7061 6e74 2064 6972 6563 746f 7269  cipant directori
-000031c0: 6573 2061 7265 206c 6162 656c 6c65 6420  es are labelled 
-000031d0: 652e 672e 2073 7562 2d30 3120 616e 6420  e.g. sub-01 and 
-000031e0: 7468 6520 7365 6c65 6374 6564 2064 6972  the selected dir
-000031f0: 6563 746f 7279 2063 6f6e 7461 696e 7320  ectory contains 
-00003200: 616c 6c20 7061 7274 6963 6970 616e 7420  all participant 
-00003210: 6469 7265 6374 6f72 6965 732e 7a06 466f  directories.z.Fo
-00003220: 756e 6420 7a15 2070 6172 7469 6369 7061  und z. participa
-00003230: 6e74 2066 6f6c 6465 7273 2e29 0672 0200  nt folders.).r..
-00003240: 0000 728e 0000 0072 5400 0000 7256 0000  ..r....rT...rV..
-00003250: 0072 5700 0000 7258 0000 0029 0372 3c00  .rW...rX...).r<.
-00003260: 0000 5a11 7061 7274 6963 6970 616e 745f  ..Z.participant_
-00003270: 7061 7468 73da 1170 6172 7469 6369 7061  paths..participa
-00003280: 6e74 5f6e 616d 6573 7214 0000 0072 1400  nt_namesr....r..
-00003290: 0000 7215 0000 00da 1566 696e 645f 7061  ..r......find_pa
-000032a0: 7274 6963 6970 616e 745f 6469 7273 ba01  rticipant_dirs..
-000032b0: 0000 730e 0000 0018 030e 010c 0208 0106  ..s.............
-000032c0: 0314 0108 027a 1b55 7469 6c73 2e66 696e  .....z.Utils.fin
-000032d0: 645f 7061 7274 6963 6970 616e 745f 6469  d_participant_di
-000032e0: 7273 6301 0000 0000 0000 0000 0000 0004  rsc.............
-000032f0: 0000 0008 0000 0043 0000 0073 a400 0000  .......C...s....
-00003300: 7c00 6100 6401 7d01 6402 7d02 7401 6403  |.a.d.}.d.}.t.d.
-00003310: 7c00 9b00 6404 7402 7c01 8301 9b00 6405  |...d.t.|.....d.
-00003320: 7402 7c02 8301 9b00 6406 9d07 8301 0100  t.|.....d.......
-00003330: 7403 6a04 6400 6407 8502 1900 7c01 7c02  t.j.d.d.....|.|.
-00003340: 6602 6b03 7250 7402 7403 6a04 6408 1900  f.k.rPt.t.j.d...
-00003350: 8301 9b00 6405 7402 7403 6a04 6409 1900  ....d.t.t.j.d...
-00003360: 8301 9b00 6405 7402 7403 6a04 6407 1900  ....d.t.t.j.d...
-00003370: 8301 9b00 9d05 7d03 7401 640a 7c03 9b00  ......}.t.d.|...
-00003380: 640b 7402 7c01 8301 9b00 6405 7402 7c02  d.t.|.....d.t.|.
-00003390: 8301 9b00 640c 9d07 8301 0100 6400 5300  ....d.......d.S.
-000033a0: 6400 5300 290d 4ee9 0300 0000 e90a 0000  d.S.).N.........
-000033b0: 007a 060a 6652 4154 207a 2520 6973 2064  .z..fRAT z% is d
-000033c0: 6576 656c 6f70 6564 2061 6e64 2074 6573  eveloped and tes
-000033d0: 7465 6420 7769 7468 2050 7974 686f 6e20  ted with Python 
-000033e0: 7233 0000 007a 022e 0a72 b600 0000 7201  r3...z...r....r.
-000033f0: 0000 0072 1e00 0000 7a15 494e 464f 3a20  ...r....z.INFO: 
-00003400: 5079 7468 6f6e 2076 6572 7369 6f6e 207a  Python version z
-00003410: 2b20 6973 2075 6e74 6573 7465 642e 2043  + is untested. C
-00003420: 6f6e 7369 6465 7220 6368 616e 6769 6e67  onsider changing
-00003430: 2074 6f20 7665 7273 696f 6e20 7a22 2069   to version z" i
-00003440: 6620 7468 6572 6520 6172 6520 6572 726f  f there are erro
-00003450: 7273 2072 756e 6e69 6e67 2066 5241 542e  rs running fRAT.
-00003460: 2905 7269 0000 0072 5800 0000 725d 0000  ).ri...rX...r]..
-00003470: 00da 0373 7973 da0c 7665 7273 696f 6e5f  ...sys..version_
-00003480: 696e 666f 2904 5a0c 6672 6174 5f76 6572  info).Z.frat_ver
-00003490: 7369 6f6e 5a0c 6578 7065 6374 5f6d 616a  sionZ.expect_maj
-000034a0: 6f72 5a0c 6578 7065 6374 5f6d 696e 6f72  orZ.expect_minor
-000034b0: 5a0f 6375 7272 656e 745f 7665 7273 696f  Z.current_versio
-000034c0: 6e72 1400 0000 7214 0000 0072 1500 0000  nr....r....r....
-000034d0: da0c 6368 6563 6b76 6572 7369 6f6e c901  ..checkversion..
-000034e0: 0000 7318 0000 0004 0304 0304 0124 0216  ..s..........$..
-000034f0: 0132 010a 0106 0104 ff06 010e ff04 fe7a  .2.............z
-00003500: 1255 7469 6c73 2e63 6865 636b 7665 7273  .Utils.checkvers
-00003510: 696f 6e63 0200 0000 0000 0000 0000 0000  ionc............
-00003520: 0400 0000 0800 0000 4300 0000 73ae 0000  ........C...s...
-00003530: 007c 0064 016b 0272 097c 016a 0072 0964  .|.d.k.r.|.j.r.d
-00003540: 0053 007c 016a 0172 2364 0264 036c 026d  .S.|.j.r#d.d.l.m
-00003550: 037d 0201 0074 04a0 05a1 009b 0064 047c  .}...t.......d.|
-00003560: 026a 069b 009d 037d 0374 04a0 077c 03a1  .j.....}.t...|..
-00003570: 0101 007c 0353 007c 016a 0864 0576 0072  ...|.S.|.j.d.v.r
-00003580: 3574 0964 0683 0101 0074 0a6a 0b64 0764  5t.d.....t.j.d.d
-00003590: 0864 098d 027d 037c 0353 007c 016a 087d  .d...}.|.S.|.j.}
-000035a0: 037a 0774 04a0 077c 03a1 0101 0057 006e  .z.t...|.....W.n
-000035b0: 0b04 0074 0c79 4a01 0001 0001 0074 0c64  ...t.yJ......t.d
-000035c0: 0a83 0182 0177 007c 016a 0d72 5574 0964  .....w.|.j.rUt.d
-000035d0: 0b7c 039b 009d 0283 0101 007c 0353 0029  .|.........|.S.)
-000035e0: 0c4e da0a 5374 6174 6973 7469 6373 721e  .N..Statisticsr.
-000035f0: 0000 0029 01da 1145 6e76 6972 6f6e 6d65  ...)...Environme
-00003600: 6e74 5f53 6574 7570 7263 0000 0029 0272  nt_Setuprc...).r
-00003610: 2300 0000 fa01 207a 2853 656c 6563 7420  #..... z(Select 
-00003620: 7468 6520 6469 7265 6374 6f72 7920 6f75  the directory ou
-00003630: 7470 7574 2062 7920 7468 6520 6652 4154  tput by the fRAT
-00003640: 2e7a 2753 656c 6563 7420 7468 6520 6469  .z'Select the di
-00003650: 7265 6374 6f72 7920 6f75 7470 7574 2062  rectory output b
-00003660: 7920 7468 6520 6652 4154 5429 0272 0b00  y the fRATT).r..
-00003670: 0000 7255 0000 007a 4e4f 7574 7075 7420  ..rU...zNOutput 
-00003680: 666f 6c64 6572 206c 6f63 6174 696f 6e20  folder location 
-00003690: 2866 5241 5420 6f75 7470 7574 2066 6f6c  (fRAT output fol
-000036a0: 6465 7220 6c6f 6361 7469 6f6e 2920 6973  der location) is
-000036b0: 206e 6f74 2061 2076 616c 6964 2064 6972   not a valid dir
-000036c0: 6563 746f 7279 2e7a 194f 7574 7075 7420  ectory.z.Output 
-000036d0: 666f 6c64 6572 2073 656c 6563 7469 6f6e  folder selection
-000036e0: 3a20 290e da0c 7275 6e5f 706c 6f74 7469  : )...run_plotti
-000036f0: 6e67 da0c 7275 6e5f 616e 616c 7973 6973  ng..run_analysis
-00003700: da08 616e 616c 7973 6973 7206 0100 0072  ..analysisr....r
-00003710: 3400 0000 72af 0000 00da 0d73 6176 655f  4...r......save_
-00003720: 6c6f 6361 7469 6f6e 7255 0000 005a 1472  locationrU...Z.r
-00003730: 6570 6f72 745f 6f75 7470 7574 5f66 6f6c  eport_output_fol
-00003740: 6465 7272 5800 0000 7208 0000 0072 5a00  derrX...r....rZ.
-00003750: 0000 7254 0000 0072 5700 0000 2904 5a0c  ..rT...rW...).Z.
-00003760: 6375 7272 656e 745f 7374 6570 7256 0000  current_steprV..
-00003770: 0072 0601 0000 5a0e 6a73 6f6e 5f64 6972  .r....Z.json_dir
-00003780: 6563 746f 7279 7214 0000 0072 1400 0000  ectoryr....r....
-00003790: 7215 0000 00da 1963 6864 6972 5f74 6f5f  r......chdir_to_
-000037a0: 6f75 7470 7574 5f64 6972 6563 746f 7279  output_directory
-000037b0: d801 0000 732c 0000 000e 0204 0106 020c  ....s,..........
-000037c0: 0114 010a 0204 120a f008 010e 0104 0e06  ................
-000037d0: f502 020e 010c 0102 0102 0104 ff02 ff06  ................
-000037e0: 040e 0104 027a 1f55 7469 6c73 2e63 6864  .....z.Utils.chd
-000037f0: 6972 5f74 6f5f 6f75 7470 7574 5f64 6972  ir_to_output_dir
-00003800: 6563 746f 7279 2902 7223 0000 0046 2903  ectory).r#...F).
-00003810: 4e72 6100 0000 7262 0000 0029 0346 5446  Nra...rb...).FTF
-00003820: 2901 4629 0172 2300 0000 2902 544e 291f  ).F).r#...).TN).
-00003830: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00003840: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00003850: 6d65 5f5f da0c 7374 6174 6963 6d65 7468  me__..staticmeth
-00003860: 6f64 7216 0000 0072 3200 0000 7240 0000  odr....r2...r@..
-00003870: 0072 4900 0000 7250 0000 0072 5a00 0000  .rI...rP...rZ...
-00003880: 7260 0000 0072 7000 0000 7279 0000 0072  r`...rp...ry...r
-00003890: 7e00 0000 7293 0000 0072 9c00 0000 72ac  ~...r....r....r.
-000038a0: 0000 0072 b300 0000 727c 0000 0072 ba00  ...r....r|...r..
-000038b0: 0000 72bb 0000 0072 c600 0000 72ca 0000  ..r....r....r...
-000038c0: 00da 0b63 6c61 7373 6d65 7468 6f64 72e9  ...classmethodr.
-000038d0: 0000 0072 dd00 0000 72f9 0000 0072 fa00  ...r....r....r..
-000038e0: 0000 72ff 0000 0072 0401 0000 720c 0100  ..r....r....r...
-000038f0: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
-00003900: 7215 0000 0072 0800 0000 1700 0000 736a  r....r........sj
-00003910: 0000 0008 0002 010a 0102 0f0a 0102 2a0a  ..............*.
-00003920: 0102 0d0a 0102 070a 0102 030c 0102 130a  ................
-00003930: 0102 060c 0102 180c 0102 140c 0102 080a  ................
-00003940: 0102 2e0a 0102 140a 0102 180c 0102 160a  ................
-00003950: 0102 060a 0102 030a 0102 030c 0102 0d0a  ................
-00003960: 0102 090c 0102 3b0a 0102 110a 0102 080a  ......;.........
-00003970: 0102 080a 0102 0e0a 0102 0e0e 0172 0800  .............r..
-00003980: 0000 2919 7225 0000 0072 0c00 0000 7234  ..).r%...r....r4
-00003990: 0000 0072 f000 0000 7272 0000 0072 0201  ...r....rr...r..
-000039a0: 0000 7202 0000 00da 0770 6174 686c 6962  ..r......pathlib
-000039b0: 7203 0000 00da 0774 6b69 6e74 6572 7204  r......tkinterr.
-000039c0: 0000 0072 0500 0000 da05 7479 7065 7372  ...r......typesr
-000039d0: 0600 0000 da0c 6d75 6c74 6970 726f 6365  ......multiproce
-000039e0: 7373 72bf 0000 00da 076e 6962 6162 656c  ssr......nibabel
-000039f0: 72f3 0000 00da 0670 616e 6461 7372 4c00  r......pandasrL.
-00003a00: 0000 72da 0000 00da 1c66 5241 542e 7574  ..r......fRAT.ut
-00003a10: 696c 732e 6652 4154 5f63 6f6e 6669 675f  ils.fRAT_config_
-00003a20: 7365 7475 7072 5600 0000 7269 0000 0072  setuprV...ri...r
-00003a30: 0800 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
-00003a40: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
-00003a50: 653e 0100 0000 7324 0000 0008 0008 0108  e>....s$........
-00003a60: 0108 0108 0108 010c 010c 0110 010c 0108  ................
-00003a70: 0208 0108 0108 0108 0204 0204 0112 03    ...............
+00000280: 5a1e 6503 6443 643b 643c 8401 8301 5a1f  Z.e.dCd;d<....Z.
+00000290: 6411 5300 2944 da05 5574 696c 7363 0100  d.S.)D..Utilsc..
+000002a0: 0000 0000 0000 0000 0000 0100 0000 0900  ................
+000002b0: 0000 4300 0000 7352 0000 007a 1c7c 0064  ..C...sR...z.|.d
+000002c0: 0176 0072 097c 00a0 00a1 007d 0074 01a0  .v.r.|.....}.t..
+000002d0: 027c 00a1 017d 0074 037c 0074 0483 0272  .|...}.t.|.t...r
+000002e0: 1a74 057c 0083 017d 0057 007c 0053 0057  .t.|...}.W.|.S.W
+000002f0: 007c 0053 0004 0074 0674 0766 0279 2801  .|.S...t.t.f.y(.
+00000300: 0001 0001 0059 007c 0053 0077 0029 024e  .....Y.|.S.w.).N
+00000310: 2902 da04 7472 7565 da05 6661 6c73 6529  )...true..false)
+00000320: 08da 0574 6974 6c65 da03 6173 74da 0c6c  ...title..ast..l
+00000330: 6974 6572 616c 5f65 7661 6cda 0a69 7369  iteral_eval..isi
+00000340: 6e73 7461 6e63 65da 0574 7570 6c65 da04  nstance..tuple..
+00000350: 6c69 7374 da0a 5661 6c75 6545 7272 6f72  list..ValueError
+00000360: da0b 5379 6e74 6178 4572 726f 7229 01da  ..SyntaxError)..
+00000370: 0178 a900 7214 0000 00fa 502f 5573 6572  .x..r.....P/User
+00000380: 732f 6c70 7865 6831 302f 446f 6375 6d65  s/lpxeh10/Docume
+00000390: 6e74 732f 5265 706f 7369 746f 7269 6573  nts/Repositories
+000003a0: 2f66 4d52 495f 524f 495f 616e 616c 7973  /fMRI_ROI_analys
+000003b0: 6973 5f74 6f6f 6c2f 6652 4154 2f75 7469  is_tool/fRAT/uti
+000003c0: 6c73 2f75 7469 6c73 2e70 79da 2363 6f6e  ls/utils.py.#con
+000003d0: 7665 7274 5f74 6f6d 6c5f 696e 7075 745f  vert_toml_input_
+000003e0: 746f 5f70 7974 686f 6e5f 6f62 6a65 6374  to_python_object
+000003f0: 1800 0000 731a 0000 0002 0208 0108 010a  ....s...........
+00000400: 020a 020a 0104 0502 fa04 0610 fd02 0104  ................
+00000410: 0202 fd7a 2955 7469 6c73 2e63 6f6e 7665  ...z)Utils.conve
+00000420: 7274 5f74 6f6d 6c5f 696e 7075 745f 746f  rt_toml_input_to
+00000430: 5f70 7974 686f 6e5f 6f62 6a65 6374 6300  _python_objectc.
+00000440: 0000 0000 0000 0000 0000 0006 0000 000a  ................
+00000450: 0000 0043 0000 0073 cc00 0000 7400 6a01  ...C...s....t.j.
+00000460: 6401 6402 6403 6404 6405 8d04 7d00 7c00  d.d.d.d.d...}.|.
+00000470: 6a02 6406 6407 6408 6409 8d03 0100 7403  j.d.d.d.d.....t.
+00000480: 640a 6400 8502 1900 7d01 7c01 4400 5d46  d.d.....}.|.D.]F
+00000490: 7d02 7404 7c02 8301 4400 5d3f 7d03 7404  }.t.|...D.]?}.t.
+000004a0: 7c02 8301 7c03 1900 640b 1900 640c 6b02  |...|...d...d.k.
+000004b0: 722c 711f 7a0e 7404 7c02 8301 7c03 1900  r,q.z.t.|...|...
+000004c0: 640d 1900 a005 640e 640f a102 7d04 5700  d.....d.d...}.W.
+000004d0: 6e09 0400 7406 7943 0100 0100 0100 5900  n...t.yC......Y.
+000004e0: 711f 7700 7c04 6410 6b02 7253 6411 7404  q.w.|.d.k.rSd.t.
+000004f0: 7c02 8301 7c03 1900 6412 1900 9b00 9d02  |...|...d.......
+00000500: 7d04 7c00 6a02 6413 7c03 9b00 9d02 7c03  }.|.j.d.|.....|.
+00000510: 7c04 6409 8d03 0100 711f 7119 7c00 a007  |.d.....q.q.|...
+00000520: a100 7d05 7c05 5300 2914 4e7a 0766 5241  ..}.|.S.).Nz.fRA
+00000530: 542e 7079 7a14 2528 7072 6f67 2973 205b  T.pyz.%(prog)s [
+00000540: 6172 6775 6d65 6e74 735d 7a44 436f 6e76  arguments]zDConv
+00000550: 6572 7420 766f 7865 6c77 6973 6520 7374  ert voxelwise st
+00000560: 6174 6973 7469 6373 2074 6f20 7265 6769  atistics to regi
+00000570: 6f6e 7769 7365 2073 7461 7469 7374 6963  onwise statistic
+00000580: 7320 666f 7220 664d 5249 2064 6174 612e  s for fMRI data.
+00000590: 6188 0100 0053 7570 706c 7969 6e67 2061  a....Supplying a
+000005a0: 7267 756d 656e 7473 2069 6e20 7468 6973  rguments in this
+000005b0: 2077 6179 2069 7320 666f 7220 6164 7661   way is for adva
+000005c0: 6e63 6564 2075 7365 7273 206f 6e6c 792e  nced users only.
+000005d0: 2049 7420 6973 2072 6563 6f6d 6d65 6e64   It is recommend
+000005e0: 6564 2074 6861 7420 7365 7474 696e 6773  ed that settings
+000005f0: 2061 7265 2063 6861 6e67 6564 2075 7369   are changed usi
+00000600: 6e67 2074 6865 2047 5549 206f 7220 6279  ng the GUI or by
+00000610: 2065 6469 7469 6e67 2074 6865 2066 5241   editing the fRA
+00000620: 545f 636f 6e66 6967 2e74 6f6d 6c20 6669  T_config.toml fi
+00000630: 6c65 2e20 4172 6775 6d65 6e74 7320 7368  le. Arguments sh
+00000640: 6f75 6c64 2062 6520 6769 7665 6e20 696e  ould be given in
+00000650: 2074 6f6d 6c20 666f 726d 6174 2e20 466f   toml format. Fo
+00000660: 7220 6578 616d 706c 653a 2074 7275 6520  r example: true 
+00000670: 7368 6f75 6c64 2062 6520 7573 6564 2069  should be used i
+00000680: 6e73 7465 6164 206f 6620 5472 7565 2061  nstead of True a
+00000690: 6e64 2073 7472 696e 6773 2073 686f 756c  nd strings shoul
+000006a0: 6420 6265 2069 6e20 7175 6f74 6174 696f  d be in quotatio
+000006b0: 6e20 6d61 726b 732e 2057 6865 7265 2061  n marks. Where a
+000006c0: 2063 6f6d 6d61 2d73 6570 6172 6174 6564   comma-separated
+000006d0: 206c 6973 7420 6973 2073 7570 706f 7365   list is suppose
+000006e0: 6420 746f 2062 6520 6769 7665 6e2c 2074  d to be given, t
+000006f0: 6869 7320 7368 6f75 6c64 2062 6520 696e  his should be in
+00000700: 2074 6865 2066 6f72 6d61 743a 205b 226d   the format: ["m
+00000710: 6222 2c20 2273 656e 7365 225d 2e29 04da  b", "sense"].)..
+00000720: 0470 726f 67da 0575 7361 6765 da0b 6465  .prog..usage..de
+00000730: 7363 7269 7074 696f 6eda 0665 7069 6c6f  scription..epilo
+00000740: 677a 0c2d 2d6d 616b 655f 7461 626c 65da  gz.--make_table.
+00000750: 0a6d 616b 655f 7461 626c 657a a874 7275  .make_tablez.tru
+00000760: 6520 6f72 2066 616c 7365 2e20 5573 6520  e or false. Use 
+00000770: 7468 6973 2066 6c61 6720 746f 2063 7265  this flag to cre
+00000780: 6174 6520 6120 6373 7620 6669 6c65 2074  ate a csv file t
+00000790: 6f20 7374 6f72 6520 7061 7261 6d65 7465  o store paramete
+000007a0: 7220 696e 666f 726d 6174 696f 6e20 6162  r information ab
+000007b0: 6f75 7420 6669 6c65 732e 2052 6563 6f6d  out files. Recom
+000007c0: 6d65 6e64 6564 2074 6861 7420 7468 6973  mended that this
+000007d0: 2066 696c 6520 6973 2063 7265 6174 6564   file is created
+000007e0: 2061 6e64 2066 696c 6c65 6420 696e 2062   and filled in b
+000007f0: 6566 6f72 6520 6652 4154 2065 7865 6375  efore fRAT execu
+00000800: 7469 6f6e 2e29 02da 0464 6573 74da 0468  tion.)...dest..h
+00000810: 656c 70e9 0100 0000 da04 7479 7065 da06  elp.......type..
+00000820: 4275 7474 6f6e da0b 4465 7363 7269 7074  Button..Descript
+00000830: 696f 6efa 0125 7a02 2525 da00 7a13 5265  ion..%z.%%..z.Re
+00000840: 636f 6d6d 656e 6465 6420 7661 6c75 653a  commended value:
+00000850: 20da 0b52 6563 6f6d 6d65 6e64 6564 7a02   ..Recommendedz.
+00000860: 2d2d 2908 da08 6172 6770 6172 7365 da0e  --)...argparse..
+00000870: 4172 6775 6d65 6e74 5061 7273 6572 da0c  ArgumentParser..
+00000880: 6164 645f 6172 6775 6d65 6e74 da05 7061  add_argument..pa
+00000890: 6765 73da 0465 7661 6cda 0772 6570 6c61  ges..eval..repla
+000008a0: 6365 da08 4b65 7945 7272 6f72 da0a 7061  ce..KeyError..pa
+000008b0: 7273 655f 6172 6773 2906 da06 7061 7273  rse_args)...pars
+000008c0: 6572 5a0e 6172 675f 6361 7465 676f 7269  erZ.arg_categori
+000008d0: 6573 da08 6361 7465 676f 7279 da03 6172  es..category..ar
+000008e0: 67da 0968 656c 705f 7465 7874 da04 6172  g..help_text..ar
+000008f0: 6773 7214 0000 0072 1400 0000 7215 0000  gsr....r....r...
+00000900: 00da 0961 7267 7061 7273 6572 2800 0000  ...argparser(...
+00000910: 732e 0000 0008 0302 0102 0206 fd08 0c02  s...............
+00000920: 0106 ff0c 0508 020c 0114 0102 0202 021c  ................
+00000930: 010c 0104 0102 ff08 0316 0118 0202 f308  ................
+00000940: 1004 027a 0f55 7469 6c73 2e61 7267 7061  ...z.Utils.argpa
+00000950: 7273 6572 6301 0000 0000 0000 0000 0000  rserc...........
+00000960: 0005 0000 0006 0000 0047 0000 0073 5200  .........G...sR.
+00000970: 0000 6700 7d02 7c01 4400 5d22 7d03 7c03  ..g.}.|.D.]"}.|.
+00000980: 6401 1900 6402 6b02 7211 7c03 a000 6402  d...d.k.r.|...d.
+00000990: a101 0100 6403 6404 8400 7401 7c00 9b00  ....d.d...t.|...
+000009a0: 6405 7c03 9b00 9d03 8301 4400 8301 7d04  d.|.......D...}.
+000009b0: 7c04 7226 7c02 a002 7c04 a101 0100 7104  |.r&|...|.....q.
+000009c0: 7c02 5300 2906 4e72 0100 0000 da01 2e63  |.S.).Nr.......c
+000009d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000009e0: 0500 0000 5300 0000 7318 0000 0067 007c  ....S...s....g.|
+000009f0: 005d 087d 0174 006a 01a0 027c 01a1 0191  .].}.t.j...|....
+00000a00: 0271 0253 0072 1400 0000 2903 da02 6f73  .q.S.r....)...os
+00000a10: da04 7061 7468 da08 6261 7365 6e61 6d65  ..path..basename
+00000a20: 2902 da02 2e30 da01 6672 1400 0000 7214  )....0..fr....r.
+00000a30: 0000 0072 1500 0000 da0a 3c6c 6973 7463  ...r......<listc
+00000a40: 6f6d 703e 5a00 0000 7302 0000 0018 007a  omp>Z...s......z
+00000a50: 2455 7469 6c73 2e66 696e 645f 6669 6c65  $Utils.find_file
+00000a60: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+00000a70: 636f 6d70 3e7a 032f 2a2e 2903 da06 6c73  comp>z./*.)...ls
+00000a80: 7472 6970 7202 0000 00da 0665 7874 656e  tripr......exten
+00000a90: 6429 05da 0964 6972 6563 746f 7279 da0a  d)...directory..
+00000aa0: 6578 7465 6e73 696f 6e73 da05 6669 6c65  extensions..file
+00000ab0: 73da 0965 7874 656e 7369 6f6e 5a0b 7468  s..extensionZ.th
+00000ac0: 6573 655f 6669 6c65 7372 1400 0000 7214  ese_filesr....r.
+00000ad0: 0000 0072 1500 0000 da0a 6669 6e64 5f66  ...r......find_f
+00000ae0: 696c 6573 5300 0000 7312 0000 0004 0208  ilesS...s.......
+00000af0: 010c 010a 011c 0204 020a 0102 8004 027a  ...............z
+00000b00: 1055 7469 6c73 2e66 696e 645f 6669 6c65  .Utils.find_file
+00000b10: 7363 0100 0000 0000 0000 0000 0000 0300  sc..............
+00000b20: 0000 0400 0000 4300 0000 732c 0000 0069  ......C...s,...i
+00000b30: 007d 017c 006a 0044 005d 0e7d 027c 007c  .}.|.j.D.].}.|.|
+00000b40: 0219 00a0 01a1 00a0 02a1 00a0 03a1 007c  ...............|
+00000b50: 017c 023c 0071 057c 0153 00a9 014e 2904  .|.<.q.|.S...N).
+00000b60: da07 636f 6c75 6d6e 73da 0664 726f 706e  ..columns..dropn
+00000b70: 61da 0874 6f5f 6e75 6d70 79da 0674 6f6c  a..to_numpy..tol
+00000b80: 6973 7429 03da 0964 6174 6166 7261 6d65  ist)...dataframe
+00000b90: da07 726f 6964 6963 74da 0663 6f6c 756d  ..roidict..colum
+00000ba0: 6e72 1400 0000 7214 0000 0072 1500 0000  nr....r....r....
+00000bb0: da11 6461 7461 6672 616d 655f 746f 5f64  ..dataframe_to_d
+00000bc0: 6963 7461 0000 0073 0800 0000 0402 0a01  icta...s........
+00000bd0: 1a01 0402 7a17 5574 696c 732e 6461 7461  ....z.Utils.data
+00000be0: 6672 616d 655f 746f 5f64 6963 7463 0100  frame_to_dictc..
+00000bf0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000c00: 0000 4300 0000 7314 0000 0074 006a 016a  ..C...s....t.j.j
+00000c10: 027c 0064 0164 028d 02a0 03a1 0053 0029  .|.d.d.......S.)
+00000c20: 034e da05 696e 6465 7829 01da 066f 7269  .N..index)...ori
+00000c30: 656e 7429 04da 0270 64da 0944 6174 6146  ent)...pd..DataF
+00000c40: 7261 6d65 da09 6672 6f6d 5f64 6963 74da  rame..from_dict.
+00000c50: 0974 7261 6e73 706f 7365 2901 7247 0000  .transpose).rG..
+00000c60: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000c70: da11 6469 6374 5f74 6f5f 6461 7461 6672  ..dict_to_datafr
+00000c80: 616d 6569 0000 00f3 0200 0000 1402 7a17  amei..........z.
+00000c90: 5574 696c 732e 6469 6374 5f74 6f5f 6461  Utils.dict_to_da
+00000ca0: 7461 6672 616d 6572 2300 0000 4663 0200  taframer#...Fc..
+00000cb0: 0000 0000 0000 0000 0000 0400 0000 0300  ................
+00000cc0: 0000 4300 0000 735c 0000 0074 0083 007d  ..C...s\...t...}
+00000cd0: 027c 02a0 01a1 0001 0074 026a 037c 0064  .|.......t.j.|.d
+00000ce0: 018d 017d 037c 02a0 04a1 0001 007c 0373  ...}.|.......|.s
+00000cf0: 1774 0564 0283 0182 017c 0172 1e74 06a0  .t.d.....|.r.t..
+00000d00: 077c 03a1 0101 0074 0864 0075 0073 2574  .|.....t.d.u.s%t
+00000d10: 086a 0972 2c74 0a64 037c 039b 009d 0283  .j.r,t.d.|......
+00000d20: 0101 007c 0353 0029 044e 2901 720b 0000  ...|.S.).N).r...
+00000d30: 007a 134e 6f20 666f 6c64 6572 2073 656c  .z.No folder sel
+00000d40: 6563 7465 642e 7a14 5365 6c65 6374 6564  ected.z.Selected
+00000d50: 2064 6972 6563 746f 7279 3a20 290b 7204   directory: ).r.
+00000d60: 0000 00da 0877 6974 6864 7261 7772 0500  .....withdrawr..
+00000d70: 0000 5a0c 6173 6b64 6972 6563 746f 7279  ..Z.askdirectory
+00000d80: da07 6465 7374 726f 79da 1146 696c 654e  ..destroy..FileN
+00000d90: 6f74 466f 756e 6445 7272 6f72 7234 0000  otFoundErrorr4..
+00000da0: 00da 0563 6864 6972 da06 636f 6e66 6967  ...chdir..config
+00000db0: da07 7665 7262 6f73 65da 0570 7269 6e74  ..verbose..print
+00000dc0: 2904 720b 0000 0072 5500 0000 da04 726f  ).r....rU.....ro
+00000dd0: 6f74 723c 0000 0072 1400 0000 7214 0000  otr<...r....r...
+00000de0: 0072 1500 0000 da0c 6669 6c65 5f62 726f  .r......file_bro
+00000df0: 7773 6572 6d00 0000 7316 0000 0006 0208  wserm...s.......
+00000e00: 010c 0208 0204 0208 0104 020a 010e 020e  ................
+00000e10: 0104 027a 1255 7469 6c73 2e66 696c 655f  ...z.Utils.file_
+00000e20: 6272 6f77 7365 7263 0200 0000 0000 0000  browserc........
+00000e30: 0000 0000 0400 0000 0500 0000 4700 0000  ............G...
+00000e40: 732c 0000 007c 0244 005d 117d 037c 0172  s,...|.D.].}.|.r
+00000e50: 0a74 007c 0383 0101 007c 00a0 0174 027c  .t.|.....|...t.|
+00000e60: 0383 0164 0117 00a1 0101 0071 0264 0053  ...d.......q.d.S
+00000e70: 0029 024e da01 0a29 0372 5800 0000 da05  .).N...).rX.....
+00000e80: 7772 6974 65da 0373 7472 2904 da0b 6669  write..str)...fi
+00000e90: 6c65 5f6f 626a 6563 745a 1170 7269 6e74  le_objectZ.print
+00000ea0: 5f74 6f5f 7465 726d 696e 616c 7231 0000  _to_terminalr1..
+00000eb0: 00da 046c 696e 6572 1400 0000 7214 0000  ...liner....r...
+00000ec0: 0072 1500 0000 da0e 7072 696e 745f 616e  .r......print_an
+00000ed0: 645f 7361 7665 8100 0000 730a 0000 0008  d_save....s.....
+00000ee0: 0204 0108 0114 0104 fd7a 1455 7469 6c73  .........z.Utils
+00000ef0: 2e70 7269 6e74 5f61 6e64 5f73 6176 654e  .print_and_saveN
+00000f00: da03 616c 6cda 0a63 6f6e 6669 675f 6c6f  ..all..config_lo
+00000f10: 6763 0600 0000 0000 0000 0000 0000 0a00  gc..............
+00000f20: 0000 0900 0000 4300 0000 7320 0100 0074  ......C...s ...t
+00000f30: 007c 009b 0064 017c 059b 0064 029d 0464  .|...d.|...d...d
+00000f40: 0383 028f 7b7d 0674 007c 019b 0064 017c  ....{}.t.|...d.|
+00000f50: 029b 009d 0364 0483 028f 587d 077c 06a0  .....d....X}.|..
+00000f60: 0164 0574 029b 0064 067c 029b 0064 079d  .d.t...d.|...d..
+00000f70: 05a1 0101 007c 0372 347c 0344 005d 077d  .....|.r4|.D.].}
+00000f80: 087c 06a0 017c 08a1 0101 0071 277c 06a0  .|...|.....q'|..
+00000f90: 0164 08a1 0101 007c 06a0 0164 08a1 0101  .d.....|...d....
+00000fa0: 0064 007d 097c 0744 005d 297d 087c 08a0  .d.}.|.D.])}.|..
+00000fb0: 0364 09a1 0172 537c 08a0 0364 0aa1 0173  .d...rS|...d...s
+00000fc0: 537c 08a0 0464 0964 0ba1 0264 0c64 0d85  S|...d.d...d.d..
+00000fd0: 0219 007d 097c 0464 0e6b 0272 5d7c 06a0  ...}.|.d.k.r]|..
+00000fe0: 017c 08a1 0101 0071 3d7c 097c 0476 0072  .|.....q=|.|.v.r
+00000ff0: 667c 06a0 017c 08a1 0101 0071 3d57 0064  f|...|.....q=W.d
+00001000: 0004 0004 0083 0301 006e 1031 0073 7177  .........n.1.sqw
+00001010: 0101 0001 0001 0059 0001 0057 0064 0004  .......Y...W.d..
+00001020: 0004 0083 0301 0064 0053 0057 0064 0004  .......d.S.W.d..
+00001030: 0004 0083 0301 0064 0053 0031 0073 8977  .......d.S.1.s.w
+00001040: 0101 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+00001050: 0f4e fa01 2f7a 052e 746f 6d6c da01 77da  .N../z..toml..w.
+00001060: 0172 7a20 2320 4765 6e65 7261 6c20 696e  .rz # General in
+00001070: 666f 726d 6174 696f 6e0a 7665 7273 696f  formation.versio
+00001080: 6e20 3d20 7a15 0a63 6f6e 6669 675f 6669  n = z..config_fi
+00001090: 6c65 5f75 7365 6420 3d20 277a 0227 0a72  le_used = 'z.'.r
+000010a0: 5b00 0000 fa01 237a 0223 2372 2300 0000  [.....#z.##r#...
+000010b0: 721e 0000 00e9 ffff ffff 7261 0000 0029  r.........ra...)
+000010c0: 05da 046f 7065 6e72 5c00 0000 da07 7665  ...openr\.....ve
+000010d0: 7273 696f 6eda 0a73 7461 7274 7377 6974  rsion..startswit
+000010e0: 6872 2a00 0000 290a 5a06 6e65 7764 6972  hr*...).Z.newdir
+000010f0: da0b 636f 6e66 6967 5f70 6174 68da 0f63  ..config_path..c
+00001100: 6f6e 6669 675f 6669 6c65 6e61 6d65 5a0f  onfig_filenameZ.
+00001110: 6164 6469 7469 6f6e 616c 5f69 6e66 6fda  additional_info.
+00001120: 1172 656c 6576 616e 745f 7365 6374 696f  .relevant_sectio
+00001130: 6e73 da0f 6e65 775f 636f 6e66 6967 5f6e  ns..new_config_n
+00001140: 616d 6572 3800 0000 7265 0000 0072 5f00  amer8...re...r_.
+00001150: 0000 5a0f 6375 7272 656e 745f 7365 6374  ..Z.current_sect
+00001160: 696f 6e72 1400 0000 7214 0000 0072 1500  ionr....r....r..
+00001170: 0000 da0b 7361 7665 5f63 6f6e 6669 6788  ....save_config.
+00001180: 0000 0073 2c00 0000 2e02 0601 0201 04ff  ...s,...........
+00001190: 0202 0afe 0404 0801 0c01 0a02 0a02 0402  ................
+000011a0: 0801 1401 1401 0802 0c01 0801 0a01 0280  ................
+000011b0: 02f9 50f2 7a11 5574 696c 732e 7361 7665  ..P.z.Utils.save
+000011c0: 5f63 6f6e 6669 6754 6306 0000 0000 0000  _configTc.......
+000011d0: 0000 0000 0007 0000 0006 0000 0043 0000  .............C..
+000011e0: 0073 9c00 0000 7c01 a000 6401 a101 7309  .s....|...d...s.
+000011f0: 7c01 6401 3700 7d01 7c02 a000 6401 a101  |.d.7.}.|...d...
+00001200: 7312 7c02 6401 3700 7d02 7c05 7217 6402  s.|.d.7.}.|.r.d.
+00001210: 7d06 6e02 7c00 7d06 7c03 723e 7c04 722e  }.n.|.}.|.r>|.r.
+00001220: 7401 a002 7c01 9b00 7c00 9b00 9d02 7c02  t...|...|.....|.
+00001230: 9b00 6403 7c06 9b00 9d03 a102 0100 6400  ..d.|.........d.
+00001240: 5300 7401 a002 7c01 9b00 7c00 9b00 9d02  S.t...|...|.....
+00001250: 7c02 9b00 7c06 9b00 9d02 a102 0100 6400  |...|.........d.
+00001260: 5300 7403 a004 7c01 9b00 7c00 9b00 9d02  S.t...|...|.....
+00001270: 7c02 9b00 7c06 9b00 9d02 a102 0100 6400  |...|.........d.
+00001280: 5300 2904 4e72 6300 0000 7a0f 7061 7261  S.).Nrc...z.para
+00001290: 6d56 616c 7565 732e 6373 765a 0563 6f70  mValues.csvZ.cop
+000012a0: 795f 2905 da08 656e 6473 7769 7468 da06  y_)...endswith..
+000012b0: 7368 7574 696c da04 636f 7079 7234 0000  shutil..copyr4..
+000012c0: 00da 0672 656e 616d 6529 07da 086f 6c64  ...rename)...old
+000012d0: 5f6e 616d 655a 0c6f 7269 6769 6e61 6c5f  _nameZ.original_
+000012e0: 6469 725a 076e 6577 5f64 6972 7272 0000  dirZ.new_dirrr..
+000012f0: 00da 0b72 656e 616d 655f 636f 7079 da0e  ...rename_copy..
+00001300: 7061 7261 6d65 7465 725f 6669 6c65 da08  parameter_file..
+00001310: 6e65 775f 6e61 6d65 7214 0000 0072 1400  new_namer....r..
+00001320: 0000 7215 0000 00da 096d 6f76 655f 6669  ..r......move_fi
+00001330: 6c65 a100 0000 7318 0000 000a 0208 010a  le....s.........
+00001340: 0208 0104 0206 0104 0204 0204 0122 0120  .............". 
+00001350: 0220 027a 0f55 7469 6c73 2e6d 6f76 655f  . .z.Utils.move_
+00001360: 6669 6c65 6302 0000 0000 0000 0000 0000  filec...........
+00001370: 0002 0000 0003 0000 0043 0000 0073 4600  .........C...sF.
+00001380: 0000 7c01 7214 7400 6a01 a002 7c00 a101  ..|.r.t.j...|...
+00001390: 7214 7403 a004 7c00 a101 0100 7405 a006  r.t...|.....t...
+000013a0: 7c00 a101 0100 6400 5300 7400 6a01 a002  |.....d.S.t.j...
+000013b0: 7c00 a101 7321 7405 a006 7c00 a101 0100  |...s!t...|.....
+000013c0: 6400 5300 6400 5300 7241 0000 0029 0772  d.S.d.S.rA...).r
+000013d0: 3400 0000 7235 0000 00da 0665 7869 7374  4...r5.....exist
+000013e0: 7372 7100 0000 da06 726d 7472 6565 7208  srq.....rmtreer.
+000013f0: 0000 00da 066d 6b5f 6469 7229 0272 3500  .....mk_dir).r5.
+00001400: 0000 da0a 6465 6c65 7465 5f6f 6c64 7214  ....delete_oldr.
+00001410: 0000 0072 1400 0000 7215 0000 00da 1263  ...r....r......c
+00001420: 6865 636b 5f61 6e64 5f6d 616b 655f 6469  heck_and_make_di
+00001430: 72b6 0000 0073 0c00 0000 1002 0a01 0e01  r....s..........
+00001440: 0c02 0e01 04ff 7a18 5574 696c 732e 6368  ......z.Utils.ch
+00001450: 6563 6b5f 616e 645f 6d61 6b65 5f64 6972  eck_and_make_dir
+00001460: 6303 0000 0000 0000 0000 0000 0007 0000  c...............
+00001470: 0008 0000 0003 0000 0073 4201 0000 7c02  .........sB...|.
+00001480: 6401 6b02 7269 6700 7d03 7400 6402 8301  d.k.rig.}.t.d...
+00001490: 0100 7401 8800 8301 4400 5d0d 5c02 7d04  ..t.....D.].\.}.
+000014a0: 7d05 7400 6403 6a02 7c04 7c05 6404 8d02  }.t.d.j.|.|.d...
+000014b0: 8301 0100 710e 7c03 7368 7400 6405 7c01  ....q.|.sht.d.|.
+000014c0: 9b00 6406 9d03 8301 0100 7403 6407 8301  ..d.......t.d...
+000014d0: 7d06 7c06 a004 a100 6408 6b02 723a 7405  }.|.....d.k.r:t.
+000014e0: 7406 6409 7407 8800 8301 8302 8301 7d03  t.d.t.........}.
+000014f0: 6e2c 7407 7c06 8301 6409 6b04 7263 640a  n,t.|...d.k.rcd.
+00001500: 640b 8400 7c06 a008 640c a101 4400 8301  d...|...d...D...
+00001510: 7d03 7a09 7405 7409 740a 7c03 8302 8301  }.z.t.t.t.|.....
+00001520: 7d03 5700 6e12 0400 740b 7962 0100 0100  }.W.n...t.yb....
+00001530: 0100 7400 640d 8301 0100 6700 7d03 5900  ..t.d.....g.}.Y.
+00001540: 6e04 7700 6700 7d03 7196 7c03 721e 6e2d  n.w.g.}.q.|.r.n-
+00001550: 740c 7c02 7405 8302 7287 740c 7c02 6409  t.|.t...r.t.|.d.
+00001560: 1900 740d 8302 7287 7c02 6409 1900 a004  ..t...r.|.d.....
+00001570: a100 6408 6b02 7287 7405 7406 6409 7407  ..d.k.r.t.t.d.t.
+00001580: 8800 8301 8302 8301 7d03 6e0f 7c02 7d03  ........}.n.|.}.
+00001590: 740c 7c03 740a 8302 7292 7c03 6701 7d03  t.|.t...r.|.g.}.
+000015a0: 6e04 7405 7c03 8301 7d03 8700 6601 640e  n.t.|...}...f.d.
+000015b0: 640b 8408 7c03 4400 8301 7d03 7c03 5300  d...|.D...}.|.S.
+000015c0: 290f 4eda 0752 756e 7469 6d65 725b 0000  ).N..Runtimer[..
+000015d0: 007a 107b 726f 695f 6e75 6d7d 3a20 7b72  .z.{roi_num}: {r
+000015e0: 6f69 7d29 02da 0772 6f69 5f6e 756d da03  oi})...roi_num..
+000015f0: 726f 697a 050a 2d2d 2d20 7a0d 2063 7265  roiz..--- z. cre
+00001600: 6174 696f 6e20 2d2d 2d7a b854 7970 6520  ation ---z.Type 
+00001610: 6120 636f 6d6d 612d 7365 7061 7261 7465  a comma-separate
+00001620: 6420 6c69 7374 206f 6620 7468 6520 524f  d list of the RO
+00001630: 4973 2028 6c69 7374 6564 2061 626f 7665  Is (listed above
+00001640: 2920 796f 7520 7761 6e74 2074 6f20 7072  ) you want to pr
+00001650: 6f64 7563 6520 6120 6669 6775 7265 2066  oduce a figure f
+00001660: 6f72 2c20 2765 2e67 2e20 322c 2031 352c  or, 'e.g. 2, 15,
+00001670: 2037 2c20 3233 2720 6f72 2027 616c 6c27   7, 23' or 'all'
+00001680: 2066 6f72 2061 6c6c 2072 6f69 732e 200a   for all rois. .
+00001690: 416c 7465 726e 6174 6976 656c 7920 7072  Alternatively pr
+000016a0: 6573 7320 656e 7465 7220 7477 6963 6520  ess enter twice 
+000016b0: 746f 2073 6b69 7020 7468 6973 2073 7465  to skip this ste
+000016c0: 703a 2072 6100 0000 7201 0000 0063 0100  p: ra...r....c..
+000016d0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000016e0: 0000 5300 0000 f314 0000 0067 007c 005d  ..S........g.|.]
+000016f0: 067d 017c 01a0 00a1 0091 0271 0253 0072  .}.|.......q.S.r
+00001700: 1400 0000 2901 da05 7374 7269 70a9 0272  ....)...strip..r
+00001710: 3700 0000 7213 0000 0072 1400 0000 7214  7...r....r....r.
+00001720: 0000 0072 1500 0000 7239 0000 00d2 0000  ...r....r9......
+00001730: 00f3 0200 0000 1400 7a2a 5574 696c 732e  ........z*Utils.
+00001740: 6669 6e64 5f63 686f 7365 6e5f 726f 6973  find_chosen_rois
+00001750: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00001760: 6f6d 703e fa01 2c7a 2c43 6f6d 6d61 2d73  omp>..,z,Comma-s
+00001770: 6570 6172 6174 6564 206c 6973 7420 636f  eparated list co
+00001780: 6e74 6169 6e73 206e 6f6e 2069 6e74 6567  ntains non integ
+00001790: 6572 732e 0a63 0100 0000 0000 0000 0000  ers..c..........
+000017a0: 0000 0200 0000 0400 0000 1300 0000 7314  ..............s.
+000017b0: 0000 0067 007c 005d 067d 0188 007c 0119  ...g.|.].}...|..
+000017c0: 0091 0271 0253 0072 1400 0000 7214 0000  ...q.S.r....r...
+000017d0: 0029 0272 3700 0000 5a0a 726f 695f 6e75  .).r7...Z.roi_nu
+000017e0: 6d62 6572 a901 da08 616c 6c5f 726f 6973  mber....all_rois
+000017f0: 7214 0000 0072 1500 0000 7239 0000 00ea  r....r....r9....
+00001800: 0000 0072 8400 0000 290e 7258 0000 00da  ...r....).rX....
+00001810: 0965 6e75 6d65 7261 7465 da06 666f 726d  .enumerate..form
+00001820: 6174 da05 696e 7075 74da 056c 6f77 6572  at..input..lower
+00001830: 7210 0000 00da 0572 616e 6765 da03 6c65  r......range..le
+00001840: 6eda 0573 706c 6974 da03 6d61 70da 0369  n..split..map..i
+00001850: 6e74 7211 0000 0072 0e00 0000 725d 0000  ntr....r....r]..
+00001860: 0029 0772 8700 0000 da09 6675 6e63 5f6e  .).r......func_n
+00001870: 616d 655a 1163 6f6e 6669 675f 7265 6769  ameZ.config_regi
+00001880: 6f6e 5f76 6172 5a0b 6368 6f73 656e 5f72  on_varZ.chosen_r
+00001890: 6f69 7372 7f00 0000 7280 0000 005a 0772  oisr....r....Z.r
+000018a0: 6f69 5f61 6e73 7214 0000 0072 8600 0000  oi_ansr....r....
+000018b0: 7215 0000 00da 1066 696e 645f 6368 6f73  r......find_chos
+000018c0: 656e 5f72 6f69 73bf 0000 0073 4400 0000  en_rois....sD...
+000018d0: 0802 0401 0801 1002 1401 0402 1001 0201  ................
+000018e0: 0201 04ff 0c04 1401 0c02 1401 0202 1201  ................
+000018f0: 0c01 0801 0801 02fe 0405 0201 04ec 0280  ................
+00001900: 1817 0e01 02ff 1402 0402 0a02 0801 0802  ................
+00001910: 1202 0402 7a16 5574 696c 732e 6669 6e64  ....z.Utils.find
+00001920: 5f63 686f 7365 6e5f 726f 6973 6302 0000  _chosen_roisc...
+00001930: 0000 0000 0000 0000 0004 0000 0008 0000  ................
+00001940: 0043 0000 0073 7e00 0000 7400 a001 a100  .C...s~...t.....
+00001950: 7d02 6401 7d03 7a1f 7c01 6402 6b02 7216  }.d.}.z.|.d.k.r.
+00001960: 7c00 9b00 6403 9d02 7d03 7400 a002 7c03  |...d...}.t...|.
+00001970: a101 7d02 6e0e 7c01 6404 6b02 7224 7c00  ..}.n.|.d.k.r$|.
+00001980: 9b00 6405 9d02 7d03 7400 a002 7c03 a101  ..d...}.t...|...
+00001990: 7d02 5700 6e10 0400 7403 7935 0100 0100  }.W.n...t.y5....
+000019a0: 0100 7404 6406 7405 6a06 9b00 6407 9d03  ..t.d.t.j...d...
+000019b0: 8301 8201 7700 7c02 a007 6408 a101 7d02  ....w.|...d...}.
+000019c0: 7c02 7c03 6602 5300 2909 4e72 2300 0000  |.|.f.S.).Nr#...
+000019d0: fa10 5365 7373 696f 6e20 6176 6572 6167  ..Session averag
+000019e0: 6564 7a4a 2f4f 7665 7261 6c6c 2f53 756d  edzJ/Overall/Sum
+000019f0: 6d61 7269 7365 645f 7265 7375 6c74 732f  marised_results/
+00001a00: 5365 7373 696f 6e5f 6176 6572 6167 6564  Session_averaged
+00001a10: 5f72 6573 756c 7473 2f63 6f6d 6269 6e65  _results/combine
+00001a20: 645f 7265 7375 6c74 732e 6a73 6f6e fa14  d_results.json..
+00001a30: 5061 7274 6963 6970 616e 7420 6176 6572  Participant aver
+00001a40: 6167 6564 7a4e 2f4f 7665 7261 6c6c 2f53  agedzN/Overall/S
+00001a50: 756d 6d61 7269 7365 645f 7265 7375 6c74  ummarised_result
+00001a60: 732f 5061 7274 6963 6970 616e 745f 6176  s/Participant_av
+00001a70: 6572 6167 6564 5f72 6573 756c 7473 2f63  eraged_results/c
+00001a80: 6f6d 6269 6e65 645f 7265 7375 6c74 732e  ombined_results.
+00001a90: 6a73 6f6e 7a23 636f 6d62 696e 6564 5f72  jsonz#combined_r
+00001aa0: 6573 756c 7473 2e6a 736f 6e20 6e6f 7420  esults.json not 
+00001ab0: 666f 756e 6420 696e 207a 0820 666f 6c64  found in z. fold
+00001ac0: 6572 2e72 4a00 0000 2908 724c 0000 0072  er.rJ...).rL...r
+00001ad0: 4d00 0000 da09 7265 6164 5f6a 736f 6e72  M.....read_jsonr
+00001ae0: 1100 0000 da09 4578 6365 7074 696f 6e72  ......Exceptionr
+00001af0: 5600 0000 da0e 6176 6572 6167 696e 675f  V.....averaging_
+00001b00: 7479 7065 da0b 736f 7274 5f76 616c 7565  type..sort_value
+00001b10: 7329 04da 0666 6f6c 6465 7272 9700 0000  s)...folderr....
+00001b20: da02 6466 7235 0000 0072 1400 0000 7214  ..dfr5...r....r.
+00001b30: 0000 0072 1500 0000 da15 7265 6164 5f63  ...r......read_c
+00001b40: 6f6d 6269 6e65 645f 7265 7375 6c74 73ee  ombined_results.
+00001b50: 0000 0073 1e00 0000 0802 0401 0202 0801  ...s............
+00001b60: 0a01 0c01 0802 0a01 0a01 0480 0c02 1201  ................
+00001b70: 02ff 0a03 0802 7a1b 5574 696c 732e 7265  ......z.Utils.re
+00001b80: 6164 5f63 6f6d 6269 6e65 645f 7265 7375  ad_combined_resu
+00001b90: 6c74 7363 0100 0000 0000 0000 0000 0000  ltsc............
+00001ba0: 0500 0000 0900 0000 0300 0000 73c2 0000  ............s...
+00001bb0: 0064 0164 0284 007c 006a 0044 0083 017c  .d.d...|.j.D...|
+00001bc0: 005f 0074 0164 0364 0484 0074 027c 006a  ._.t.d.d...t.|.j
+00001bd0: 0083 0144 0083 0164 0583 027d 0174 0164  ...D...d...}.t.d
+00001be0: 0664 0484 0074 027c 006a 0083 0144 0083  .d...t.|.j...D..
+00001bf0: 0164 0583 027d 027c 0273 2e74 0364 0774  .d...}.|.s.t.d.t
+00001c00: 046a 059b 0064 089d 0383 0182 0167 007d  .j...d.......g.}
+00001c10: 0374 046a 0644 005d 2889 0074 0187 0066  .t.j.D.](..t...f
+00001c20: 0164 0964 0484 0874 027c 006a 0083 0144  .d.d...t.|.j...D
+00001c30: 0083 0164 0583 027d 047c 0472 4c7c 03a0  ...d...}.|.rL|..
+00001c40: 077c 04a1 0101 0071 3374 0864 0a88 009b  .|.....q3t.d....
+00001c50: 0064 0b74 046a 059b 0064 0c74 046a 059b  .d.t.j...d.t.j..
+00001c60: 0064 0d9d 0783 0182 017c 017c 037c 0266  .d.......|.|.|.f
+00001c70: 0353 0029 0e4e 6301 0000 0000 0000 0000  .S.).Nc.........
+00001c80: 0000 0002 0000 0004 0000 0053 0000 0072  ...........S...r
+00001c90: 8100 0000 7214 0000 00a9 0172 8b00 0000  ....r......r....
+00001ca0: 7283 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00001cb0: 1500 0000 7239 0000 0005 0100 0072 8400  ....r9.......r..
+00001cc0: 0000 7a2a 5574 696c 732e 6669 6e64 5f63  ..z*Utils.find_c
+00001cd0: 6f6c 756d 6e5f 6c6f 6373 2e3c 6c6f 6361  olumn_locs.<loca
+00001ce0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 6301  ls>.<listcomp>c.
+00001cf0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
+00001d00: 0000 0073 0000 00f3 2000 0000 8100 7c00  ...s.... .....|.
+00001d10: 5d0b 5c02 7d01 7d02 6400 7c02 7600 7202  ].\.}.}.d.|.v.r.
+00001d20: 7c01 5600 0100 7102 6401 5300 2902 7a0b  |.V...q.d.S.).z.
+00001d30: 6967 6e6f 7265 2066 696c 654e 7214 0000  ignore fileNr...
+00001d40: 00a9 0372 3700 0000 da07 636f 756e 7465  ...r7.....counte
+00001d50: 7272 4800 0000 7214 0000 0072 1400 0000  rrH...r....r....
+00001d60: 7215 0000 00da 093c 6765 6e65 7870 723e  r......<genexpr>
+00001d70: 0701 0000 7304 0000 0002 801e 007a 2955  ....s........z)U
+00001d80: 7469 6c73 2e66 696e 645f 636f 6c75 6d6e  tils.find_column
+00001d90: 5f6c 6f63 732e 3c6c 6f63 616c 733e 2e3c  _locs.<locals>.<
+00001da0: 6765 6e65 7870 723e 4663 0100 0000 0000  genexpr>Fc......
+00001db0: 0000 0000 0000 0300 0000 0300 0000 7300  ..............s.
+00001dc0: 0000 729d 0000 0029 02da 0862 6173 656c  ..r....)...basel
+00001dd0: 696e 654e 7214 0000 0072 9e00 0000 7214  ineNr....r....r.
+00001de0: 0000 0072 1400 0000 7215 0000 0072 a000  ...r....r....r..
+00001df0: 0000 0a01 0000 7308 0000 0002 800a 0006  ......s.........
+00001e00: 010e ff7a 1c4e 6f20 6261 7365 6c69 6e65  ...z.No baseline
+00001e10: 2063 6f6c 756d 6e20 666f 756e 6420 696e   column found in
+00001e20: 2072 3300 0000 6301 0000 0000 0000 0000   r3...c.........
+00001e30: 0000 0003 0000 0003 0000 0033 0000 0073  ...........3...s
+00001e40: 2400 0000 8100 7c00 5d0d 5c02 7d01 7d02  $.....|.].\.}.}.
+00001e50: 8800 a000 a100 7c02 6b02 7202 7c01 5600  ......|.k.r.|.V.
+00001e60: 0100 7102 6400 5300 7241 0000 0072 9c00  ..q.d.S.rA...r..
+00001e70: 0000 729e 0000 00a9 01da 036b 6579 7214  ..r........keyr.
+00001e80: 0000 0072 1500 0000 72a0 0000 0011 0100  ...r....r.......
+00001e90: 0073 0400 0000 0280 2200 7a05 4b65 7920  .s......".z.Key 
+00001ea0: 227a 0f22 206e 6f74 2066 6f75 6e64 2069  "z." not found i
+00001eb0: 6e20 7a76 2e20 4368 6563 6b20 7468 6520  n zv. Check the 
+00001ec0: 4372 6974 6963 616c 2050 6172 616d 6574  Critical Paramet
+00001ed0: 6572 7320 6f70 7469 6f6e 2069 6e20 7468  ers option in th
+00001ee0: 6520 5061 7273 696e 6720 6d65 6e75 2028  e Parsing menu (
+00001ef0: 7061 7261 6d65 7465 725f 6469 6374 3120  parameter_dict1 
+00001f00: 6966 206e 6f74 2075 7369 6e67 2074 6865  if not using the
+00001f10: 2047 5549 2920 636f 7272 6563 746c 7920   GUI) correctly 
+00001f20: 6d61 7463 6820 7468 6520 7a09 2068 6561  match the z. hea
+00001f30: 6465 7273 2e29 0972 4200 0000 da04 6e65  ders.).rB.....ne
+00001f40: 7874 7288 0000 00da 094e 616d 6545 7272  xtr......NameErr
+00001f50: 6f72 7256 0000 0072 7600 0000 da0e 7061  orrV...rv.....pa
+00001f60: 7261 6d65 7465 725f 6469 6374 da06 6170  rameter_dict..ap
+00001f70: 7065 6e64 7296 0000 0029 05da 0574 6162  pendr....)...tab
+00001f80: 6c65 da11 6967 6e6f 7265 5f63 6f6c 756d  le..ignore_colum
+00001f90: 6e5f 6c6f 635a 1362 6173 656c 696e 655f  n_locZ.baseline_
+00001fa0: 636f 6c75 6d6e 5f6c 6f63 da14 6372 6974  column_loc..crit
+00001fb0: 6963 616c 5f63 6f6c 756d 6e5f 6c6f 6373  ical_column_locs
+00001fc0: 5a0a 636f 6c75 6d6e 5f6c 6f63 7214 0000  Z.column_locr...
+00001fd0: 0072 a200 0000 7215 0000 00da 1066 696e  .r....r......fin
+00001fe0: 645f 636f 6c75 6d6e 5f6c 6f63 7303 0100  d_column_locs...
+00001ff0: 0073 2400 0000 1202 1402 0201 04ff 1403  .s$.............
+00002000: 0201 04ff 0402 1201 0402 0a01 1e01 0402  ................
+00002010: 0c01 1202 0402 0afe 0a04 7a16 5574 696c  ..........z.Util
+00002020: 732e 6669 6e64 5f63 6f6c 756d 6e5f 6c6f  s.find_column_lo
+00002030: 6373 6301 0000 0000 0000 0000 0000 0004  csc.............
+00002040: 0000 0008 0000 0043 0000 0073 8200 0000  .......C...s....
+00002050: 7c00 7205 7c00 7d01 6e04 7400 a001 a100  |.r.|.}.n.t.....
+00002060: 7d01 7400 6a02 a003 7c01 9b00 6401 7404  }.t.j...|...d.t.
+00002070: 6a05 9b00 9d03 a101 7226 7406 a007 7c01  j.......r&t...|.
+00002080: 9b00 6401 7404 6a05 9b00 9d03 a101 7d02  ..d.t.j.......}.
+00002090: 6402 7d03 7c02 7c03 6602 5300 7a0f 7406  d.}.|.|.f.S.z.t.
+000020a0: a007 7c01 9b00 6403 9d02 a101 7d02 6404  ..|...d.....}.d.
+000020b0: 7d03 5700 7c02 7c03 6602 5300 0400 7408  }.W.|.|.f.S...t.
+000020c0: 7940 0100 0100 0100 7409 6405 8301 8201  y@......t.d.....
+000020d0: 7700 2906 4e72 6300 0000 da0b 6261 7365  w.).Nrc.....base
+000020e0: 5f66 6f6c 6465 727a 152f 636f 7079 5f70  _folderz./copy_p
+000020f0: 6172 616d 5661 6c75 6573 2e63 7376 da0d  aramValues.csv..
+00002100: 7265 706f 7274 5f66 6f6c 6465 727a b34d  report_folderz.M
+00002110: 616b 6520 7375 7265 2061 2063 6f70 7920  ake sure a copy 
+00002120: 6f66 2070 6172 616d 5661 6c75 6573 2e63  of paramValues.c
+00002130: 7376 2069 7320 696e 2074 6865 2063 686f  sv is in the cho
+00002140: 7365 6e20 666f 6c64 6572 2e20 0a41 6c73  sen folder. .Als
+00002150: 6f20 6d61 6b65 2073 7572 6520 7468 6520  o make sure the 
+00002160: 7365 6c65 6374 6564 2066 6f6c 6465 7220  selected folder 
+00002170: 636f 6e74 6169 6e73 2061 6c6c 2074 6865  contains all the
+00002180: 2070 6172 7469 6369 7061 6e74 2064 6972   participant dir
+00002190: 6563 746f 7269 6573 2069 6e20 7468 6520  ectories in the 
+000021a0: 6e65 6365 7373 6172 7920 4249 4453 2066  necessary BIDS f
+000021b0: 6f72 6d61 7420 652e 672e 2073 7562 2d30  ormat e.g. sub-0
+000021c0: 312e 290a 7234 0000 00da 0667 6574 6377  1.).r4.....getcw
+000021d0: 6472 3500 0000 da06 6973 6669 6c65 7256  dr5.....isfilerV
+000021e0: 0000 0072 7600 0000 724c 0000 00da 0872  ...rv...rL.....r
+000021f0: 6561 645f 6373 7672 5400 0000 7296 0000  ead_csvrT...r...
+00002200: 0029 0472 3c00 0000 7299 0000 0072 a800  .).r<...r....r..
+00002210: 0000 da0b 666f 6c64 6572 5f74 7970 6572  ....folder_typer
+00002220: 1400 0000 7214 0000 0072 1500 0000 da15  ....r....r......
+00002230: 6c6f 6164 5f70 6172 616d 5661 6c75 6573  load_paramValues
+00002240: 5f66 696c 651c 0100 0073 1c00 0000 0402  _file....s......
+00002250: 0601 0802 1802 1601 0401 080c 02f7 1001  ................
+00002260: 0601 0807 0cfb 0801 02ff 7a1b 5574 696c  ..........z.Util
+00002270: 732e 6c6f 6164 5f70 6172 616d 5661 6c75  s.load_paramValu
+00002280: 6573 5f66 696c 6563 0100 0000 0000 0000  es_filec........
+00002290: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
+000022a0: 7326 0000 007a 0874 00a0 017c 00a1 0101  s&...z.t...|....
+000022b0: 0057 0064 0053 0004 0074 0279 1201 0001  .W.d.S...t.y....
+000022c0: 0001 0059 0064 0053 0077 0072 4100 0000  ...Y.d.S.w.rA...
+000022d0: 2903 7234 0000 00da 056d 6b64 6972 da0f  ).r4.....mkdir..
+000022e0: 4669 6c65 4578 6973 7473 4572 726f 7229  FileExistsError)
+000022f0: 0172 3500 0000 7214 0000 0072 1400 0000  .r5...r....r....
+00002300: 7215 0000 0072 7b00 0000 3301 0000 730a  r....r{...3...s.
+00002310: 0000 0002 0210 010c 0106 0102 ff7a 0c55  .............z.U
+00002320: 7469 6c73 2e6d 6b5f 6469 7263 0000 0000  tils.mk_dirc....
+00002330: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00002340: 4700 0000 731e 0000 0074 007c 0064 0119  G...s....t.|.d..
+00002350: 007c 0064 0219 0083 027c 0064 0364 0085  .|.d.....|.d.d..
+00002360: 0219 008e 0053 0029 044e 7201 0000 0072  .....S.).Nr....r
+00002370: 1e00 0000 e902 0000 0029 01da 0767 6574  .........)...get
+00002380: 6174 7472 a901 da04 6172 6776 7214 0000  attr....argvr...
+00002390: 0072 1400 0000 7215 0000 00da 1769 6e73  .r....r......ins
+000023a0: 7461 6e63 655f 6d65 7468 6f64 5f68 616e  tance_method_han
+000023b0: 646c 6572 3a01 0000 7302 0000 001e 027a  dler:...s......z
+000023c0: 1d55 7469 6c73 2e69 6e73 7461 6e63 655f  .Utils.instance_
+000023d0: 6d65 7468 6f64 5f68 616e 646c 6572 6300  method_handlerc.
+000023e0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+000023f0: 0000 0047 0000 0073 1400 0000 7c00 6401  ...G...s....|.d.
+00002400: 1900 7c00 6402 6400 8502 1900 8e00 5300  ..|.d.d.......S.
+00002410: 2903 4e72 0100 0000 721e 0000 0072 1400  ).Nr....r....r..
+00002420: 0000 72b7 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00002430: 0072 1500 0000 da14 636c 6173 735f 6d65  .r......class_me
+00002440: 7468 6f64 5f68 616e 646c 6572 3e01 0000  thod_handler>...
+00002450: 7251 0000 007a 1a55 7469 6c73 2e63 6c61  rQ...z.Utils.cla
+00002460: 7373 5f6d 6574 686f 645f 6861 6e64 6c65  ss_method_handle
+00002470: 7263 0100 0000 0000 0000 0000 0000 0300  rc..............
+00002480: 0000 0400 0000 4300 0000 734e 0000 0074  ......C...sN...t
+00002490: 006a 0164 016b 0272 0a74 02a0 03a1 007d  .j.d.k.r.t.....}
+000024a0: 016e 0574 0474 006a 0183 017d 0174 02a0  .n.t.t.j...}.t..
+000024b0: 0564 02a1 017d 0274 006a 0672 217c 0073  .d...}.t.j.r!|.s
+000024c0: 2174 0764 037c 019b 0064 049d 0383 0101  !t.d.|...d......
+000024d0: 007c 026a 087c 0164 058d 0153 0029 064e  .|.j.|.d...S.).N
+000024e0: da03 6d61 78da 0a66 6f72 6b73 6572 7665  ..max..forkserve
+000024f0: 727a 200a 5374 6172 7469 6e67 2070 726f  rz .Starting pro
+00002500: 6365 7373 696e 6720 706f 6f6c 2075 7369  cessing pool usi
+00002510: 6e67 207a 0720 636f 7265 732e 2901 da09  ng z. cores.)...
+00002520: 7072 6f63 6573 7365 7329 0972 5600 0000  processes).rV...
+00002530: 5a0e 6d61 785f 636f 7265 5f75 7361 6765  Z.max_core_usage
+00002540: da02 6d70 da09 6370 755f 636f 756e 7472  ..mp..cpu_countr
+00002550: 9000 0000 da0b 6765 745f 636f 6e74 6578  ......get_contex
+00002560: 7472 5700 0000 7258 0000 00da 0450 6f6f  trW...rX.....Poo
+00002570: 6c29 03da 0772 6573 7461 7274 da07 776f  l)...restart..wo
+00002580: 726b 6572 73da 0363 7478 7214 0000 0072  rkers..ctxr....r
+00002590: 1400 0000 7215 0000 00da 1573 7461 7274  ....r......start
+000025a0: 5f70 726f 6365 7373 696e 675f 706f 6f6c  _processing_pool
+000025b0: 4201 0000 730e 0000 000a 020a 010a 020a  B...s...........
+000025c0: 020a 0210 010c 027a 1b55 7469 6c73 2e73  .......z.Utils.s
+000025d0: 7461 7274 5f70 726f 6365 7373 696e 675f  tart_processing_
+000025e0: 706f 6f6c 6302 0000 0000 0000 0000 0000  poolc...........
+000025f0: 0002 0000 0003 0000 0043 0000 0073 2400  .........C...s$.
+00002600: 0000 7c00 a000 a100 0100 7c00 a001 a100  ..|.......|.....
+00002610: 0100 7c01 7210 7402 6a03 6401 6402 8d01  ..|.r.t.j.d.d...
+00002620: 7d00 7c00 5300 2903 4e54 2901 72c2 0000  }.|.S.).NT).r...
+00002630: 0029 04da 0563 6c6f 7365 da04 6a6f 696e  .)...close..join
+00002640: 7208 0000 0072 c500 0000 2902 da04 706f  r....r....)...po
+00002650: 6f6c 72c2 0000 0072 1400 0000 7214 0000  olr....r....r...
+00002660: 0072 1500 0000 da14 6a6f 696e 5f70 726f  .r......join_pro
+00002670: 6365 7373 696e 675f 706f 6f6c 5001 0000  cessing_poolP...
+00002680: 730a 0000 0008 0208 0104 020c 0104 027a  s..............z
+00002690: 1a55 7469 6c73 2e6a 6f69 6e5f 7072 6f63  .Utils.join_proc
+000026a0: 6573 7369 6e67 5f70 6f6f 6c63 0500 0000  essing_poolc....
+000026b0: 0000 0000 0000 0000 0800 0000 0a00 0000  ................
+000026c0: 4300 0000 7318 0100 0074 007c 019b 0064  C...s....t.|...d
+000026d0: 017c 029b 009d 0364 0283 028f 787d 057a  .|.....d....x}.z
+000026e0: 677c 05a0 01a1 007d 0674 02a0 0364 03a0  g|.....}.t...d..
+000026f0: 047c 06a1 01a1 017d 067c 0644 005d 0c7d  .|.....}.|.D.].}
+00002700: 077c 067c 0719 0064 046b 0272 2664 007c  .|.|...d.k.r&d.|
+00002710: 067c 073c 0071 1a7c 0372 2974 0564 1069  .|.<.q.|.r)t.d.i
+00002720: 007c 06a4 018e 0161 0674 076a 08a0 097c  .|.....a.t.j...|
+00002730: 01a1 0164 0519 0064 066b 0272 5667 0064  ...d...d.k.rVg.d
+00002740: 07a2 0167 0064 08a2 0164 099c 0274 065f  ...g.d...d...t._
+00002750: 0a64 0a64 0b84 0074 0b74 0c74 066a 0d83  .d.d...t.t.t.j..
+00002760: 0183 0144 0083 0174 065f 0e74 0fa0 1074  ...D...t._.t...t
+00002770: 06a1 0101 007c 0264 0c6b 0272 697c 0474  .....|.d.k.ri|.t
+00002780: 065f 117c 0474 065f 1264 0d74 065f 1364  ._.|.t._.d.t._.d
+00002790: 0e74 065f 1464 0e74 065f 1574 0657 0057  .t._.d.t._.t.W.W
+000027a0: 0002 0064 0004 0004 0083 0301 0053 0004  ...d.........S..
+000027b0: 0074 026a 166a 1774 1866 0279 8101 0001  .t.j.j.t.f.y....
+000027c0: 0001 0074 1964 0f83 0182 0177 0031 0073  ...t.d.....w.1.s
+000027d0: 8577 0101 0001 0001 0059 0001 0064 0053  .w.......Y...d.S
+000027e0: 0029 114e 7263 0000 0072 6500 0000 7223  .).Nrc...re...r#
+000027f0: 0000 00da 044e 6f6e 6572 6700 0000 5a0c  .....Nonerg...Z.
+00002800: 726f 695f 616e 616c 7973 6973 290b 7a0c  roi_analysis).z.
+00002810: 546f 7461 6c20 766f 7865 6c73 7a0f 4578  Total voxelsz.Ex
+00002820: 636c 7564 6564 2076 6f78 656c 737a 1a41  cluded voxelsz.A
+00002830: 7665 7261 6765 2076 6f78 656c 7320 7065  verage voxels pe
+00002840: 7220 7365 7373 696f 6eda 044d 6561 6eda  r session..Mean.
+00002850: 0753 7464 5f64 6576 da13 436f 6e66 6964  .Std_dev..Confid
+00002860: 656e 6365 5f69 6e74 6572 7661 6cda 064d  ence_interval..M
+00002870: 6564 6961 6eda 074d 696e 696d 756d da07  edian..Minimum..
+00002880: 4d61 7869 6d75 6dda 0c50 6172 7469 6369  Maximum..Partici
+00002890: 7061 6e74 73da 0853 6573 7369 6f6e 7329  pants..Sessions)
+000028a0: 0a5a 0c56 6f78 656c 5f61 6d6f 756e 74da  .Z.Voxel_amount.
+000028b0: 1645 7863 6c75 6465 645f 766f 7865 6c73  .Excluded_voxels
+000028c0: 5f61 6d6f 756e 745a 0e41 7665 7261 6765  _amountZ.Average
+000028d0: 5f76 6f78 656c 7372 cb00 0000 5a12 5374  _voxelsr....Z.St
+000028e0: 616e 6461 7264 5f64 6576 6961 7469 6f6e  andard_deviation
+000028f0: 72cd 0000 0072 ce00 0000 72cf 0000 0072  r....r....r....r
+00002900: d000 0000 72d2 0000 0029 0272 9400 0000  ....r....).r....
+00002910: 7293 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00002920: 0000 0200 0000 0500 0000 5300 0000 731e  ..........S...s.
+00002930: 0000 0069 007c 005d 0b7d 0174 006a 017c  ...i.|.].}.t.j.|
+00002940: 0119 0074 006a 027c 0119 0093 0271 0253  ...t.j.|.....q.S
+00002950: 0072 1400 0000 2903 7256 0000 00da 0f70  .r....).rV.....p
+00002960: 6172 616d 6574 6572 5f64 6963 7431 da0f  arameter_dict1..
+00002970: 7061 7261 6d65 7465 725f 6469 6374 3229  parameter_dict2)
+00002980: 0272 3700 0000 da01 6972 1400 0000 7214  .r7.....ir....r.
+00002990: 0000 0072 1500 0000 da0a 3c64 6963 7463  ...r......<dictc
+000029a0: 6f6d 703e 8401 0000 730a 0000 0006 0002  omp>....s.......
+000029b0: 0108 ff08 0106 ff7a 2555 7469 6c73 2e6c  .......z%Utils.l
+000029c0: 6f61 645f 636f 6e66 6967 2e3c 6c6f 6361  oad_config.<loca
+000029d0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7a10  ls>.<dictcomp>z.
+000029e0: 7465 7374 5f63 6f6e 6669 672e 746f 6d6c  test_config.toml
+000029f0: 5a0f 7465 7374 5f52 4f49 5f72 6570 6f72  Z.test_ROI_repor
+00002a00: 745a 0974 6573 745f 6d61 7073 7a35 436f  tZ.test_mapsz5Co
+00002a10: 6e66 6967 2066 696c 6520 6e6f 7420 696e  nfig file not in
+00002a20: 2063 6f72 7265 6374 2066 6f72 6d61 7420   correct format 
+00002a30: 6f72 206d 6973 7369 6e67 2065 6e74 7269  or missing entri
+00002a40: 6573 2e72 1400 0000 291a 7268 0000 00da  es.r....).rh....
+00002a50: 0972 6561 646c 696e 6573 da04 746f 6d6c  .readlines..toml
+00002a60: da05 6c6f 6164 7372 c700 0000 7206 0000  ..loadsr....r...
+00002a70: 0072 5600 0000 7234 0000 0072 3500 0000  .rV...r4...r5...
+00002a80: 728e 0000 00da 1173 7461 7469 7374 6963  r......statistic
+00002a90: 5f6f 7074 696f 6e73 728c 0000 0072 8d00  _optionsr....r..
+00002aa0: 0000 72d4 0000 0072 a600 0000 7208 0000  ..r....r....r...
+00002ab0: 00da 1463 6c65 616e 5f63 6f6e 6669 675f  ...clean_config_
+00002ac0: 6f70 7469 6f6e 73da 0e62 7261 696e 5f66  options..brain_f
+00002ad0: 696c 655f 6c6f 6372 ac00 0000 da0d 6f75  ile_locr......ou
+00002ae0: 7470 7574 5f66 6f6c 6465 725a 126f 7574  tput_folderZ.out
+00002af0: 7075 745f 666f 6c64 6572 5f6e 616d 65da  put_folder_name.
+00002b00: 0f73 7461 745f 6d61 705f 666f 6c64 6572  .stat_map_folder
+00002b10: da07 6465 636f 6465 72da 0f54 6f6d 6c44  ..decoder..TomlD
+00002b20: 6563 6f64 6545 7272 6f72 da0e 4174 7472  ecodeError..Attr
+00002b30: 6962 7574 6545 7272 6f72 7296 0000 0029  ibuteErrorr....)
+00002b40: 08da 0363 6c73 726b 0000 00da 0866 696c  ...clsrk.....fil
+00002b50: 656e 616d 65da 0473 6176 6572 3500 0000  ename..saver5...
+00002b60: da08 746f 6d6c 6669 6c65 da05 7061 7273  ..tomlfile..pars
+00002b70: 6572 a300 0000 7214 0000 0072 1400 0000  er....r....r....
+00002b80: 7215 0000 00da 0b6c 6f61 645f 636f 6e66  r......load_conf
+00002b90: 6967 5a01 0000 733c 0000 0016 0202 0108  igZ...s<........
+00002ba0: 0110 0108 020c 0108 0102 8004 020e 0314  ................
+00002bb0: 0206 0206 0c08 f306 190c 0108 ff0a 0308  ................
+00002bc0: 0206 0206 0106 0106 0106 0104 0210 cb14  ................
+00002bd0: 3708 0102 ff14 c97a 1155 7469 6c73 2e6c  7......z.Utils.l
+00002be0: 6f61 645f 636f 6e66 6967 6301 0000 0000  oad_configc.....
+00002bf0: 0000 0000 0000 0003 0000 0007 0000 0043  ...............C
+00002c00: 0000 0073 6e00 0000 6700 6401 a201 7d01  ...sn...g.d...}.
+00002c10: 7400 7c00 6a01 8301 7402 7501 7212 7c01  t.|.j...t.u.r.|.
+00002c20: a003 7c00 6a01 a101 7c00 5f01 6700 6402  ..|.j...|._.g.d.
+00002c30: a201 7d02 7400 7c00 6a04 8301 7402 7501  ..}.t.|.j...t.u.
+00002c40: 7235 6403 7405 6404 7406 a007 6405 7c00  r5d.t.d.t...d.|.
+00002c50: 6a04 a102 6406 1900 9b00 9d02 8301 1800  j...d...........
+00002c60: 7c00 5f08 7c02 a003 7c00 6a04 a101 7c00  |._.|...|.j...|.
+00002c70: 5f04 7c00 5300 2907 4e29 0d7a 1343 6572  _.|.S.).N).z.Cer
+00002c80: 6562 656c 6c75 6d2d 4d4e 4966 6c69 7274  ebellum-MNIflirt
+00002c90: 7a13 4365 7265 6265 6c6c 756d 2d4d 4e49  z.Cerebellum-MNI
+00002ca0: 666e 6972 747a 1248 6172 7661 7264 4f78  fnirtz.HarvardOx
+00002cb0: 666f 7264 2d63 6f72 747a 1148 6172 7661  ford-cortz.Harva
+00002cc0: 7264 4f78 666f 7264 2d73 7562 7a0f 4a48  rdOxford-subz.JH
+00002cd0: 552d 4943 424d 2d6c 6162 656c 737a 0f4a  U-ICBM-labelsz.J
+00002ce0: 4855 2d49 4342 4d2d 7472 6163 7473 5a07  HU-ICBM-tractsZ.
+00002cf0: 6a75 656c 6963 68da 034d 4e49 7a0c 534d  juelich..MNIz.SM
+00002d00: 4154 542d 6c61 6265 6c73 da03 5354 4e7a  ATT-labels..STNz
+00002d10: 1373 7472 6961 7475 6d2d 7374 7275 6374  .striatum-struct
+00002d20: 7572 616c 7a10 5461 6c61 6972 6163 682d  uralz.Talairach-
+00002d30: 6c61 6265 6c73 da08 5468 616c 616d 7573  labels..Thalamus
+00002d40: 2906 7a09 3830 252c 2031 2e32 387a 0938  ).z.80%, 1.28z.8
+00002d50: 3525 2c20 312e 3434 7a09 3930 252c 2031  5%, 1.44z.90%, 1
+00002d60: 2e36 347a 0939 3525 2c20 312e 3936 7a09  .64z.95%, 1.96z.
+00002d70: 3938 252c 2032 2e33 337a 0939 3925 2c20  98%, 2.33z.99%, 
+00002d80: 322e 3538 721e 0000 007a 0230 2e72 2200  2.58r....z.0.r".
+00002d90: 0000 7201 0000 0029 0972 1f00 0000 da0c  ..r....).r......
+00002da0: 6174 6c61 735f 6e75 6d62 6572 7290 0000  atlas_numberr...
+00002db0: 0072 4a00 0000 da11 636f 6e66 5f6c 6576  .rJ.....conf_lev
+00002dc0: 656c 5f6e 756d 6265 72da 0566 6c6f 6174  el_number..float
+00002dd0: da02 7265 728e 0000 00da 0f62 6f6f 7473  ..rer......boots
+00002de0: 7472 6170 5f61 6c70 6861 2903 7256 0000  trap_alpha).rV..
+00002df0: 00da 0d61 746c 6173 5f6f 7074 696f 6e73  ...atlas_options
+00002e00: 5a12 636f 6e66 5f6c 6576 656c 5f6f 7074  Z.conf_level_opt
+00002e10: 696f 6e73 7214 0000 0072 1400 0000 7215  ionsr....r....r.
+00002e20: 0000 0072 dc00 0000 9601 0000 7310 0000  ...r........s...
+00002e30: 0008 020e 050e 0108 020e 0222 010e 0104  ..........."....
+00002e40: 027a 1a55 7469 6c73 2e63 6c65 616e 5f63  .z.Utils.clean_c
+00002e50: 6f6e 6669 675f 6f70 7469 6f6e 7363 0100  onfig_optionsc..
+00002e60: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00002e70: 0000 4300 0000 7320 0000 0074 00a0 017c  ..C...s ...t...|
+00002e80: 00a1 017d 017c 016a 027d 027c 01a0 03a1  ...}.|.j.}.|....
+00002e90: 007d 017c 017c 0266 0253 0072 4100 0000  .}.|.|.f.S.rA...
+00002ea0: 2904 da03 6e69 62da 046c 6f61 64da 0668  )...nib..load..h
+00002eb0: 6561 6465 72da 0967 6574 5f66 6461 7461  eader..get_fdata
+00002ec0: 2903 da09 6669 6c65 5f70 6174 68da 0464  )...file_path..d
+00002ed0: 6174 6172 f400 0000 7214 0000 0072 1400  atar....r....r..
+00002ee0: 0000 7215 0000 00da 0a6c 6f61 645f 6272  ..r......load_br
+00002ef0: 6169 6ea8 0100 0073 0800 0000 0a02 0602  ain....s........
+00002f00: 0801 0802 7a10 5574 696c 732e 6c6f 6164  ....z.Utils.load
+00002f10: 5f62 7261 696e 6301 0000 0000 0000 0000  _brainc.........
+00002f20: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
+00002f30: 2200 0000 6700 6401 a201 7d01 7c01 4400  "...g.d...}.|.D.
+00002f40: 5d08 7d02 7c00 a000 7c02 6402 a102 7d00  ].}.|...|.d...}.
+00002f50: 7106 7c00 5300 2903 4e29 04fa 072e 6e69  q.|.S.).N)....ni
+00002f60: 692e 677a 7a04 2e6e 6969 7a04 2e68 6472  i.gzz..niiz..hdr
+00002f70: 7a05 2e6a 736f 6e72 2300 0000 2901 722a  z..jsonr#...).r*
+00002f80: 0000 0029 0372 3500 0000 723d 0000 0072  ...).r5...r=...r
+00002f90: 3f00 0000 7214 0000 0072 1400 0000 7215  ?...r....r....r.
+00002fa0: 0000 00da 0973 7472 6970 5f65 7874 b101  .....strip_ext..
+00002fb0: 0000 7308 0000 0008 0208 020e 0104 027a  ..s............z
+00002fc0: 0f55 7469 6c73 2e73 7472 6970 5f65 7874  .Utils.strip_ext
+00002fd0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00002fe0: 0004 0000 0043 0000 0073 5c00 0000 6401  .....C...s\...d.
+00002ff0: 6402 8400 7400 7c00 9b00 6403 9d02 8301  d...t.|...d.....
+00003000: 4400 8301 7d01 6404 6402 8400 7c01 4400  D...}.d.d...|.D.
+00003010: 8301 7d02 7401 7c01 8301 6405 6b02 721d  ..}.t.|...d.k.r.
+00003020: 7402 6406 8301 8201 7403 6a04 722a 7405  t.d.....t.j.r*t.
+00003030: 6407 7401 7c01 8301 9b00 6408 9d03 8301  d.t.|.....d.....
+00003040: 0100 7c01 7c02 6602 5300 2909 4e63 0100  ..|.|.f.S.).Nc..
+00003050: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00003060: 0000 5300 0000 731c 0000 0067 007c 005d  ..S...s....g.|.]
+00003070: 0a7d 0174 00a0 0164 007c 01a1 0272 027c  .}.t...d.|...r.|
+00003080: 0191 0271 0253 0029 017a 0b73 7562 2d5b  ...q.S.).z.sub-[
+00003090: 302d 395d 2b24 2902 72ef 0000 00da 0673  0-9]+$).r......s
+000030a0: 6561 7263 6829 0272 3700 0000 da05 6469  earch).r7.....di
+000030b0: 7265 6372 1400 0000 7214 0000 0072 1500  recr....r....r..
+000030c0: 0000 7239 0000 00bd 0100 0073 0200 0000  ..r9.......s....
+000030d0: 1c00 7a2f 5574 696c 732e 6669 6e64 5f70  ..z/Utils.find_p
+000030e0: 6172 7469 6369 7061 6e74 5f64 6972 732e  articipant_dirs.
+000030f0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00003100: 6d70 3e7a 022f 2a63 0100 0000 0000 0000  mp>z./*c........
+00003110: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00003120: 731a 0000 0067 007c 005d 097d 017c 01a0  s....g.|.].}.|..
+00003130: 0064 00a1 0164 0119 0091 0271 0253 0029  .d...d.....q.S.)
+00003140: 0272 6300 0000 7267 0000 0029 0172 8e00  .rc...rg...).r..
+00003150: 0000 2902 7237 0000 00da 0b70 6172 7469  ..).r7.....parti
+00003160: 6369 7061 6e74 7214 0000 0072 1400 0000  cipantr....r....
+00003170: 7215 0000 0072 3900 0000 be01 0000 7302  r....r9.......s.
+00003180: 0000 001a 0072 0100 0000 7a9e 5061 7274  .....r....z.Part
+00003190: 6963 6970 616e 7420 6469 7265 6374 6f72  icipant director
+000031a0: 6965 7320 6e6f 7420 666f 756e 642e 0a4d  ies not found..M
+000031b0: 616b 6520 7375 7265 2070 6172 7469 6369  ake sure partici
+000031c0: 7061 6e74 2064 6972 6563 746f 7269 6573  pant directories
+000031d0: 2061 7265 206c 6162 656c 6c65 6420 652e   are labelled e.
+000031e0: 672e 2073 7562 2d30 3120 616e 6420 7468  g. sub-01 and th
+000031f0: 6520 7365 6c65 6374 6564 2064 6972 6563  e selected direc
+00003200: 746f 7279 2063 6f6e 7461 696e 7320 616c  tory contains al
+00003210: 6c20 7061 7274 6963 6970 616e 7420 6469  l participant di
+00003220: 7265 6374 6f72 6965 732e 7a06 466f 756e  rectories.z.Foun
+00003230: 6420 7a15 2070 6172 7469 6369 7061 6e74  d z. participant
+00003240: 2066 6f6c 6465 7273 2e29 0672 0200 0000   folders.).r....
+00003250: 728d 0000 0072 5400 0000 7256 0000 0072  r....rT...rV...r
+00003260: 5700 0000 7258 0000 0029 0372 3c00 0000  W...rX...).r<...
+00003270: 5a11 7061 7274 6963 6970 616e 745f 7061  Z.participant_pa
+00003280: 7468 73da 1170 6172 7469 6369 7061 6e74  ths..participant
+00003290: 5f6e 616d 6573 7214 0000 0072 1400 0000  _namesr....r....
+000032a0: 7215 0000 00da 1566 696e 645f 7061 7274  r......find_part
+000032b0: 6963 6970 616e 745f 6469 7273 ba01 0000  icipant_dirs....
+000032c0: 730e 0000 0018 030e 010c 0208 0106 0314  s...............
+000032d0: 0108 027a 1b55 7469 6c73 2e66 696e 645f  ...z.Utils.find_
+000032e0: 7061 7274 6963 6970 616e 745f 6469 7273  participant_dirs
+000032f0: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00003300: 0008 0000 0043 0000 0073 a400 0000 7c00  .....C...s....|.
+00003310: 6100 6401 7d01 6402 7d02 7401 6403 7c00  a.d.}.d.}.t.d.|.
+00003320: 9b00 6404 7402 7c01 8301 9b00 6405 7402  ..d.t.|.....d.t.
+00003330: 7c02 8301 9b00 6406 9d07 8301 0100 7403  |.....d.......t.
+00003340: 6a04 6400 6407 8502 1900 7c01 7c02 6602  j.d.d.....|.|.f.
+00003350: 6b03 7250 7402 7403 6a04 6408 1900 8301  k.rPt.t.j.d.....
+00003360: 9b00 6405 7402 7403 6a04 6409 1900 8301  ..d.t.t.j.d.....
+00003370: 9b00 6405 7402 7403 6a04 6407 1900 8301  ..d.t.t.j.d.....
+00003380: 9b00 9d05 7d03 7401 640a 7c03 9b00 640b  ....}.t.d.|...d.
+00003390: 7402 7c01 8301 9b00 6405 7402 7c02 8301  t.|.....d.t.|...
+000033a0: 9b00 640c 9d07 8301 0100 6400 5300 6400  ..d.......d.S.d.
+000033b0: 5300 290d 4ee9 0300 0000 e90a 0000 007a  S.).N..........z
+000033c0: 060a 6652 4154 207a 2520 6973 2064 6576  ..fRAT z% is dev
+000033d0: 656c 6f70 6564 2061 6e64 2074 6573 7465  eloped and teste
+000033e0: 6420 7769 7468 2050 7974 686f 6e20 7233  d with Python r3
+000033f0: 0000 007a 022e 0a72 b500 0000 7201 0000  ...z...r....r...
+00003400: 0072 1e00 0000 7a15 494e 464f 3a20 5079  .r....z.INFO: Py
+00003410: 7468 6f6e 2076 6572 7369 6f6e 207a 2b20  thon version z+ 
+00003420: 6973 2075 6e74 6573 7465 642e 2043 6f6e  is untested. Con
+00003430: 7369 6465 7220 6368 616e 6769 6e67 2074  sider changing t
+00003440: 6f20 7665 7273 696f 6e20 7a22 2069 6620  o version z" if 
+00003450: 7468 6572 6520 6172 6520 6572 726f 7273  there are errors
+00003460: 2072 756e 6e69 6e67 2066 5241 542e 2905   running fRAT.).
+00003470: 7269 0000 0072 5800 0000 725d 0000 00da  ri...rX...r]....
+00003480: 0373 7973 da0c 7665 7273 696f 6e5f 696e  .sys..version_in
+00003490: 666f 2904 5a0c 6672 6174 5f76 6572 7369  fo).Z.frat_versi
+000034a0: 6f6e 5a0c 6578 7065 6374 5f6d 616a 6f72  onZ.expect_major
+000034b0: 5a0c 6578 7065 6374 5f6d 696e 6f72 5a0f  Z.expect_minorZ.
+000034c0: 6375 7272 656e 745f 7665 7273 696f 6e72  current_versionr
+000034d0: 1400 0000 7214 0000 0072 1500 0000 da0c  ....r....r......
+000034e0: 6368 6563 6b76 6572 7369 6f6e c901 0000  checkversion....
+000034f0: 7318 0000 0004 0304 0304 0124 0216 0132  s..........$...2
+00003500: 010a 0106 0104 ff06 010e ff04 fe7a 1255  .............z.U
+00003510: 7469 6c73 2e63 6865 636b 7665 7273 696f  tils.checkversio
+00003520: 6e63 0200 0000 0000 0000 0000 0000 0400  nc..............
+00003530: 0000 0800 0000 4300 0000 73ae 0000 007c  ......C...s....|
+00003540: 0064 016b 0272 097c 016a 0072 0964 0053  .d.k.r.|.j.r.d.S
+00003550: 007c 016a 0172 2364 0264 036c 026d 037d  .|.j.r#d.d.l.m.}
+00003560: 0201 0074 04a0 05a1 009b 0064 047c 026a  ...t.......d.|.j
+00003570: 069b 009d 037d 0374 04a0 077c 03a1 0101  .....}.t...|....
+00003580: 007c 0353 007c 016a 0864 0576 0072 3574  .|.S.|.j.d.v.r5t
+00003590: 0964 0683 0101 0074 0a6a 0b64 0764 0864  .d.....t.j.d.d.d
+000035a0: 098d 027d 037c 0353 007c 016a 087d 037a  ...}.|.S.|.j.}.z
+000035b0: 0774 04a0 077c 03a1 0101 0057 006e 0b04  .t...|.....W.n..
+000035c0: 0074 0c79 4a01 0001 0001 0074 0c64 0a83  .t.yJ......t.d..
+000035d0: 0182 0177 007c 016a 0d72 5574 0964 0b7c  ...w.|.j.rUt.d.|
+000035e0: 039b 009d 0283 0101 007c 0353 0029 0c4e  .........|.S.).N
+000035f0: da0a 5374 6174 6973 7469 6373 721e 0000  ..Statisticsr...
+00003600: 0029 01da 1145 6e76 6972 6f6e 6d65 6e74  .)...Environment
+00003610: 5f53 6574 7570 7263 0000 0029 0272 2300  _Setuprc...).r#.
+00003620: 0000 fa01 207a 2853 656c 6563 7420 7468  .... z(Select th
+00003630: 6520 6469 7265 6374 6f72 7920 6f75 7470  e directory outp
+00003640: 7574 2062 7920 7468 6520 6652 4154 2e7a  ut by the fRAT.z
+00003650: 2753 656c 6563 7420 7468 6520 6469 7265  'Select the dire
+00003660: 6374 6f72 7920 6f75 7470 7574 2062 7920  ctory output by 
+00003670: 7468 6520 6652 4154 5429 0272 0b00 0000  the fRATT).r....
+00003680: 7255 0000 007a 4e4f 7574 7075 7420 666f  rU...zNOutput fo
+00003690: 6c64 6572 206c 6f63 6174 696f 6e20 2866  lder location (f
+000036a0: 5241 5420 6f75 7470 7574 2066 6f6c 6465  RAT output folde
+000036b0: 7220 6c6f 6361 7469 6f6e 2920 6973 206e  r location) is n
+000036c0: 6f74 2061 2076 616c 6964 2064 6972 6563  ot a valid direc
+000036d0: 746f 7279 2e7a 194f 7574 7075 7420 666f  tory.z.Output fo
+000036e0: 6c64 6572 2073 656c 6563 7469 6f6e 3a20  lder selection: 
+000036f0: 290e da0c 7275 6e5f 706c 6f74 7469 6e67  )...run_plotting
+00003700: da0c 7275 6e5f 616e 616c 7973 6973 da08  ..run_analysis..
+00003710: 616e 616c 7973 6973 7206 0100 0072 3400  analysisr....r4.
+00003720: 0000 72ae 0000 00da 0d73 6176 655f 6c6f  ..r......save_lo
+00003730: 6361 7469 6f6e 7255 0000 005a 1472 6570  cationrU...Z.rep
+00003740: 6f72 745f 6f75 7470 7574 5f66 6f6c 6465  ort_output_folde
+00003750: 7272 5800 0000 7208 0000 0072 5a00 0000  rrX...r....rZ...
+00003760: 7254 0000 0072 5700 0000 2904 5a0c 6375  rT...rW...).Z.cu
+00003770: 7272 656e 745f 7374 6570 7256 0000 0072  rrent_steprV...r
+00003780: 0601 0000 5a0e 6a73 6f6e 5f64 6972 6563  ....Z.json_direc
+00003790: 746f 7279 7214 0000 0072 1400 0000 7215  toryr....r....r.
+000037a0: 0000 00da 1963 6864 6972 5f74 6f5f 6f75  .....chdir_to_ou
+000037b0: 7470 7574 5f64 6972 6563 746f 7279 d801  tput_directory..
+000037c0: 0000 732c 0000 000e 0204 0106 020c 0114  ..s,............
+000037d0: 010a 0204 120a f008 010e 0104 0e06 f502  ................
+000037e0: 020e 010c 0102 0102 0104 ff02 ff06 040e  ................
+000037f0: 0104 027a 1f55 7469 6c73 2e63 6864 6972  ...z.Utils.chdir
+00003800: 5f74 6f5f 6f75 7470 7574 5f64 6972 6563  _to_output_direc
+00003810: 746f 7279 6305 0000 0000 0000 0000 0000  toryc...........
+00003820: 0006 0000 0008 0000 0043 0000 0073 3e00  .........C...s>.
+00003830: 0000 7400 a001 7c00 6400 7c04 a103 7d05  ..t...|.d.|...}.
+00003840: 7400 a002 7c05 7c03 9b00 6401 7c02 9b00  t...|.|...d.|...
+00003850: 7c01 9b00 6402 9d05 a102 0100 7c03 9b00  |...d.......|...
+00003860: 6401 7c02 9b00 7c01 9b00 6402 9d05 5300  d.|...|...d...S.
+00003870: 2903 4e72 6300 0000 72f9 0000 0029 0372  ).Nrc...r....).r
+00003880: f200 0000 da0a 4e69 6674 6931 5061 6972  ......Nifti1Pair
+00003890: 72e5 0000 0029 0672 f700 0000 da03 6578  r....).r......ex
+000038a0: 745a 0b6e 6f5f 6578 745f 6669 6c65 72de  tZ.no_ext_filer.
+000038b0: 0000 0072 f400 0000 da05 6272 6169 6e72  ...r......brainr
+000038c0: 1400 0000 7214 0000 0072 1500 0000 da0a  ....r....r......
+000038d0: 7361 7665 5f62 7261 696e f501 0000 7306  save_brain....s.
+000038e0: 0000 000e 021c 0114 027a 1055 7469 6c73  .........z.Utils
+000038f0: 2e73 6176 655f 6272 6169 6e29 0272 2300  .save_brain).r#.
+00003900: 0000 4629 034e 7261 0000 0072 6200 0000  ..F).Nra...rb...
+00003910: 2903 4654 4629 0146 2901 7223 0000 0029  ).FTF).F).r#...)
+00003920: 0254 4e72 4100 0000 2920 da08 5f5f 6e61  .TNrA...) ..__na
+00003930: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00003940: da0c 5f5f 7175 616c 6e61 6d65 5f5f da0c  ..__qualname__..
+00003950: 7374 6174 6963 6d65 7468 6f64 7216 0000  staticmethodr...
+00003960: 0072 3200 0000 7240 0000 0072 4900 0000  .r2...r@...rI...
+00003970: 7250 0000 0072 5a00 0000 7260 0000 0072  rP...rZ...r`...r
+00003980: 6f00 0000 7278 0000 0072 7d00 0000 7292  o...rx...r}...r.
+00003990: 0000 0072 9b00 0000 72ab 0000 0072 b200  ...r....r....r..
+000039a0: 0000 727b 0000 0072 b900 0000 72ba 0000  ..r{...r....r...
+000039b0: 0072 c500 0000 72c9 0000 00da 0b63 6c61  .r....r......cla
+000039c0: 7373 6d65 7468 6f64 72e8 0000 0072 dc00  ssmethodr....r..
+000039d0: 0000 72f8 0000 0072 fa00 0000 72ff 0000  ..r....r....r...
+000039e0: 0072 0401 0000 720c 0100 0072 1001 0000  .r....r....r....
+000039f0: 7214 0000 0072 1400 0000 7214 0000 0072  r....r....r....r
+00003a00: 1500 0000 7208 0000 0017 0000 0073 6e00  ....r........sn.
+00003a10: 0000 0800 0201 0a01 020f 0a01 022a 0a01  .............*..
+00003a20: 020d 0a01 0207 0a01 0203 0c01 0213 0a01  ................
+00003a30: 0206 0c01 0218 0c01 0214 0c01 0208 0a01  ................
+00003a40: 022e 0a01 0214 0a01 0218 0c01 0216 0a01  ................
+00003a50: 0206 0a01 0203 0a01 0203 0c01 020d 0a01  ................
+00003a60: 0209 0c01 023b 0a01 0211 0a01 0208 0a01  .....;..........
+00003a70: 0208 0a01 020e 0a01 020e 0a01 021c 1001  ................
+00003a80: 7208 0000 0029 1972 2500 0000 720c 0000  r....).r%...r...
+00003a90: 0072 3400 0000 72ef 0000 0072 7100 0000  .r4...r....rq...
+00003aa0: 7202 0100 0072 0200 0000 da07 7061 7468  r....r......path
+00003ab0: 6c69 6272 0300 0000 da07 746b 696e 7465  libr......tkinte
+00003ac0: 7272 0400 0000 7205 0000 00da 0574 7970  rr....r......typ
+00003ad0: 6573 7206 0000 005a 0c6d 756c 7469 7072  esr....Z.multipr
+00003ae0: 6f63 6573 7372 be00 0000 da07 6e69 6261  ocessr......niba
+00003af0: 6265 6c72 f200 0000 da06 7061 6e64 6173  belr......pandas
+00003b00: 724c 0000 0072 d900 0000 da1c 6652 4154  rL...r......fRAT
+00003b10: 2e75 7469 6c73 2e66 5241 545f 636f 6e66  .utils.fRAT_conf
+00003b20: 6967 5f73 6574 7570 7256 0000 0072 6900  ig_setuprV...ri.
+00003b30: 0000 7208 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00003b40: 0072 1400 0000 7215 0000 00da 083c 6d6f  .r....r......<mo
+00003b50: 6475 6c65 3e01 0000 0073 2400 0000 0800  dule>....s$.....
+00003b60: 0801 0801 0801 0801 0801 0c01 0c01 1001  ................
+00003b70: 0c01 0802 0801 0801 0801 0802 0402 0401  ................
+00003b80: 1203                                     ..
```

### Comparing `frat_brain-1.4.0/fRAT/utils/analysis.py` & `frat_brain-1.5.0/fRAT/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/bootstrap.css` & `frat_brain-1.5.0/fRAT/utils/bootstrap.css`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/dash_report.py` & `frat_brain-1.5.0/fRAT/utils/dash_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/directory_comparison.py` & `frat_brain-1.5.0/fRAT/utils/directory_comparison.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/fRAT_config_setup.py` & `frat_brain-1.5.0/fRAT/utils/fRAT_config_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,20 +88,20 @@
                          'STN',
                          'striatum-structural',
                          'Talairach-labels',
                          'Thalamus'
                      ],
                      'Description': ''},
 
-    'input_folder_name': {'type': 'Entry', 'Recommended': "func_cleaned", 'save_as': 'string',
+    'input_folder_name': {'type': 'Entry', 'Recommended': "func_preprocessed", 'save_as': 'string',
                           'Description': 'Folder found in each subjects directory containing the files to be analysed. '
-                                         'func_cleaned is the default option as this folder will automatically be '
+                                         'func_preprocessed is the default option as this folder will automatically be '
                                          'created when making statmaps. If the "Noise volume included in time series" '
                                          'option was set to true, or motion outlier removal was used when creating '
-                                         'the statmaps, this folder will contain cleaned versions of the original func '
+                                         'the statmaps, this folder will contain preprocessed versions of the original func '
                                          'files. However if these options were not used when creating the statmaps, '
                                          'the folder will still be present, however the files will be identical to '
                                          'those in the "func" folder.'},
 
     'output_folder': {'type': 'Entry', 'Recommended': 'DEFAULT', 'save_as': 'string', 'label': 'Output directory',
                       'Description': 'Directory to save output. If set to DEFAULT, output directory will be set to '
                                      'the cortical atlas used appended with "_ROI_report". '
```

### Comparing `frat_brain-1.4.0/fRAT/utils/figures.py` & `frat_brain-1.5.0/fRAT/utils/figures.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/html_report.py` & `frat_brain-1.5.0/fRAT/utils/html_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/printResults.py` & `frat_brain-1.5.0/fRAT/utils/printResults.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/statistics.py` & `frat_brain-1.5.0/fRAT/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.4.0/fRAT/utils/statmap.py` & `frat_brain-1.5.0/fRAT/utils/statmap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import itertools
 
 import numpy as np
 from nipype.interfaces import fsl
 import logging
 import time
 
+from ..HOUSE.handler import HOUSE
 from .utils import *
 
 config = None
 config_path = ''
 config_filename = ''
 
 
-def file_setup(func):
+def statmap_file_setup(func):
     file_location = config.input_folder_name
 
     if config.output_folder_name != 'DEFAULT':
         output_folder = f"statmaps/{config.output_folder_name}"
     elif func == 'Image SNR':
         output_folder = 'statmaps/imageSNR_report'
     elif func == 'Temporal SNR':
         output_folder = 'statmaps/temporalSNR_report'
-    elif func == 'Add Gaussian noise':
-        output_folder = 'added_noise'
 
     if config.base_folder in ("", " "):
         print('Select the directory which contains the subject folders.')
         base_sub_location = Utils.file_browser(title='Select the directory which contains the subject folders')
 
     else:
         base_sub_location = config.base_folder
@@ -35,130 +34,103 @@
     participant_dir, _ = Utils.find_participant_dirs(base_sub_location)
     participants = {participant: None for participant in participant_dir}
 
     for participant in participants:
         # Find all nifti and analyze files
         participants[participant] = Utils.find_files(f"{participant}/{file_location}", "hdr", "nii.gz", "nii")
 
-        if 'statmaps' in output_folder:
-            Utils.check_and_make_dir(f"{participant}/statmaps")
-            Utils.check_and_make_dir(f"{participant}/{output_folder}", delete_old=True)
-            Utils.save_config(f"{participant}/{output_folder}", config_path, config_filename,
-                              additional_info=[f"statistical_map_created = '{func}'\n"],
-                              new_config_name='statmap_config')
-        else:
-            Utils.check_and_make_dir(f"{participant}/{file_location}/{output_folder}", delete_old=True)
+        Utils.check_and_make_dir(f"{participant}/statmaps")
+        Utils.check_and_make_dir(f"{participant}/{output_folder}", delete_old=True)
+        Utils.save_config(f"{participant}/{output_folder}", config_path, config_filename,
+                          additional_info=[f"statistical_map_created = '{func}'\n"],
+                          new_config_name='statmap_config')
 
     return participants, output_folder, file_location
 
 
 def calculate_sigma_in_volumes(file_path):
     data = nib.load(file_path)
     TR = data.header['pixdim'][4]  # Find TR
 
     # Equation found here: https://www.jiscmail.ac.uk/cgi-bin/webadmin?A2=FSL;f6fd75a6.1709
     return 1 / (2 * config.highpass_filter_cutoff * TR)
 
 
-def save_brain(data, ext, no_ext_file, output_folder, header=None):
-    brain = nib.Nifti1Pair(data, None, header)
-    nib.save(brain, f"{output_folder}/{no_ext_file}{ext}.nii.gz")
-
-    return f"{output_folder}/{no_ext_file}{ext}.nii.gz"
-
-
 def temporalSNR_calc(file, no_ext_file, output_folder):
     fsl.maths.MeanImage(in_file=file, out_file=f'{output_folder}/{no_ext_file}_tMean.nii.gz').run()  # Mean over time
 
-    fsl.maths.StdImage(in_file=file, out_file=f'{output_folder}/{no_ext_file}_tStd.nii.gz').run()  # Standard dev over time
+    fsl.maths.StdImage(in_file=file,
+                       out_file=f'{output_folder}/{no_ext_file}_tStd.nii.gz').run()  # Standard dev over time
 
     # tMean / tStd
     fsl.maths.BinaryMaths(operation='div', in_file=f'{output_folder}/{no_ext_file}_tMean.nii.gz',
-                      operand_file=f'{output_folder}/{no_ext_file}_tStd.nii.gz',
-                      out_file=f'{output_folder}/{no_ext_file}_tSNR.nii.gz').run()
+                          operand_file=f'{output_folder}/{no_ext_file}_tStd.nii.gz',
+                          out_file=f'{output_folder}/{no_ext_file}_tSNR.nii.gz').run()
 
     # Threshold volume so any tSNR values above 1000 are set to 0
     fsl.maths.Threshold(in_file=f'{output_folder}/{no_ext_file}_tSNR.nii.gz', thresh=1000.0, direction='above',
-                    out_file=f'{output_folder}/{no_ext_file}_tSNR.nii.gz').run()
+                        out_file=f'{output_folder}/{no_ext_file}_tSNR.nii.gz').run()
 
 
 def imageSNR_calc(func_file, noise_file, no_ext_file, output_folder, participant_dir):
-    fsl.maths.MeanImage(in_file=func_file, out_file=f'{output_folder}/{no_ext_file}_tMean.nii.gz').run()  # Mean over time
-
-    if config.iSNR_std_use_only_nonzero_voxels:
-        std_string = '-S'
-    else:
-        std_string = '-s'
+    fsl.maths.MeanImage(in_file=func_file,
+                        out_file=f'{output_folder}/{no_ext_file}_tMean.nii.gz').run()  # Mean over time
 
     if config.noise_volume:
-        std = fsl.ImageStats(in_file=noise_file, op_string=std_string,
-                         terminal_output='allatonce').run()  # Std dev of entire volume
-        noise_value = std.outputs.get()['out_stat']
+        file, _ = Utils.load_brain(noise_file)
+
+        # Std dev of entire volume
+        if config.iSNR_std_use_only_nonzero_voxels:
+            noise_value = file[file != 0].std()
+        else:
+            noise_value = file.std()
 
     else:
         base_sub_location = Path(participant_dir).parents[0]
         participant_name = os.path.split(Path(participant_dir))[1]
 
         noise_value_csv = pd.read_csv(f'{base_sub_location}/noiseValues.csv')
         noise_value = float(noise_value_csv[noise_value_csv['Participant'] == participant_name]['Background noise'])
 
     # tMean / Std
     fsl.maths.BinaryMaths(operation='div',
-                      in_file=f'{output_folder}/{no_ext_file}_tMean.nii.gz',
-                      operand_value=noise_value,
-                      out_file=f'{output_folder}/{no_ext_file}_iSNR.nii.gz').run()
+                          in_file=f'{output_folder}/{no_ext_file}_tMean.nii.gz',
+                          operand_value=noise_value,
+                          out_file=f'{output_folder}/{no_ext_file}_iSNR.nii.gz').run()
 
     if config.magnitude_correction:
         magnitude_correction(f'{output_folder}/{no_ext_file}_iSNR.nii.gz')
 
 
 def magnitude_correction(file_name):
     fsl.maths.BinaryMaths(in_file=file_name, operation='mul', operand_value=0.7, out_file=file_name).run()
 
 
-def separate_noise_from_func(file, no_ext_file, output_folder, participant):
-    data, header = Utils.load_brain(file)
-
-    if config.noise_volume_location == 'End':
-        noise_data, func_data = data[:, :, :, -1], data[:, :, :, :-1]
-    elif config.noise_volume_location == 'Beginning':
-        noise_data, func_data = data[:, :, :, 0], data[:, :, :, 1:]
-    else:
-        raise Exception('Noise volume location not valid.')
-
-    noise_file = save_brain(noise_data, '_noise_volume', no_ext_file, output_folder, header)
-
-    func_file = save_to_cleaned_folder(func_data, header, no_ext_file, participant,
-                                       f'Removed noise volume from {config.noise_volume_location.lower()} of timeseries')
-
-    return func_file, noise_file
-
-
-def save_to_cleaned_folder(data, header, no_ext_file, participant, method):
-    with open(f'{participant}/{config.input_folder_name}_cleaned/changes_made_to_files.txt', 'a+') as f:
+def save_to_preprocessed_folder(data, header, no_ext_file, participant, method):
+    with open(f'{participant}/{config.input_folder_name}_preprocessed/changes_made_to_files.txt', 'a+') as f:
         f.seek(0)  # Go to start of file
         f.write(f'{no_ext_file}: {method}\n')
 
-    data = save_brain(data, '', no_ext_file, f'{participant}/{config.input_folder_name}_cleaned', header)
+    data = Utils.save_brain(data, '', no_ext_file, f'{participant}/{config.input_folder_name}_preprocessed', header)
 
     return data
 
 
 def highpass_filtering(file_path, output_folder, no_ext_file):
     sigma_in_volumes = calculate_sigma_in_volumes(file_path)
 
     fsl.maths.MeanImage(in_file=f'{file_path}', out_file=f'{output_folder}/{no_ext_file}_tMean.nii.gz').run()
 
     fsl.TemporalFilter(in_file=f'{file_path}',
-                   out_file=f'{output_folder}/{no_ext_file}_filtered.nii.gz',
-                   highpass_sigma=sigma_in_volumes).run()
+                       out_file=f'{output_folder}/{no_ext_file}_filtered.nii.gz',
+                       highpass_sigma=sigma_in_volumes).run()
 
     fsl.maths.BinaryMaths(operation='add', in_file=f'{output_folder}/{no_ext_file}_tMean.nii.gz',
-                      operand_file=f'{output_folder}/{no_ext_file}_filtered.nii.gz',
-                      out_file=f'{output_folder}/{no_ext_file}_filtered_restoredmean.nii.gz').run()
+                          operand_file=f'{output_folder}/{no_ext_file}_filtered.nii.gz',
+                          out_file=f'{output_folder}/{no_ext_file}_filtered_restoredmean.nii.gz').run()
 
     return f'{output_folder}/{no_ext_file}_filtered_restoredmean.nii.gz', \
            f'{output_folder}/{no_ext_file}_filtered.nii.gz'
 
 
 def delete_files(redundant_files):
     for file in redundant_files:
@@ -176,33 +148,37 @@
     noise_file = None
 
     redundant_files = []
     outliers = []
 
     # Save original copy of file which may be overwritten later, however allows this folder to always be used
     data, header = Utils.load_brain(file)
-    save_brain(data, '', no_ext_file, f'{participant}/{config.input_folder_name}_cleaned', header)
+    Utils.save_brain(data, '', no_ext_file, f'{participant}/{config.input_folder_name}_preprocessed', header)
 
     if config.noise_volume:
-        file, noise_file = separate_noise_from_func(file, no_ext_file, output_folder, participant)
-        redundant_files.append(noise_file)
+        file = f'{participant}/func_volumes/{no_ext_file}.nii.gz'
+        noise_file = f'{participant}/noise_volume/{no_ext_file}_noise_volume.nii.gz'
+
+        if not os.path.exists(file) or not os.path.exists(noise_file):
+            raise FileNotFoundError('Could not find separate noise and functional volumes. '
+                                    'Run the "separate noise volumes" utility to create these files.')
 
     if config.remove_motion_outliers:
         file, outlier_timepoints, outlier_files = remove_motion_outliers(file, no_ext_file, output_folder, participant)
         redundant_files.extend(outlier_files)
         outliers.extend(outlier_timepoints)
 
     if config.motion_correction:
         output = f'{output_folder}/{no_ext_file}_motion_corrected.nii.gz'
 
         fsl.MCFLIRT(in_file=file, out_file=output).run()
         file = output
 
         data, header = Utils.load_brain(file)
-        file = save_to_cleaned_folder(data, header, no_ext_file, participant, 'Motion corrected data')
+        file = save_to_preprocessed_folder(data, header, no_ext_file, participant, 'Motion corrected data')
 
     if config.spatial_smoothing:
         fsl.SUSAN(in_file=file, fwhm=config.smoothing_fwhm, brightness_threshold=config.smoothing_brightness_threshold,
                   out_file=f'{output_folder}/{no_ext_file}_smoothed.nii.gz').run()
         file = f'{output_folder}/{no_ext_file}_smoothed.nii.gz'
 
     if config.temporal_filter:
@@ -230,15 +206,15 @@
         if outlier_check != -1:
             outlier_timepoints.append(time_point)
 
     data, header = Utils.load_brain(file)
     data = np.delete(data, outlier_timepoints, axis=3)
 
     # Save copy of motion outlier removed files as it may make registration better during main analysis
-    file = save_to_cleaned_folder(data, header, no_ext_file, participant, 'Removed motion outlier timepoints')
+    file = save_to_preprocessed_folder(data, header, no_ext_file, participant, 'Removed motion outlier timepoints')
 
     return file, [no_ext_file, len(outlier_timepoints)], [outlier_file, outlier_plot, outlier_values]
 
 
 def process_files_for_statmaps(file, participant, output_folder, file_location, func, cfg):
     global config
     config = cfg
@@ -269,15 +245,19 @@
               f'\nSaving output in directory: {output_folder}')
 
     for participant_dir, files in participants.items():
         if config.verbose:
             print(f'\nCreating statistical maps for participant: {participant_dir.split("/")[-1]}'
                   f'\n      Creating statmaps for {len(files)} files')
 
-        Utils.check_and_make_dir(f'{participant_dir}/{config.input_folder_name}_cleaned', delete_old=True)
+        Utils.check_and_make_dir(f'{participant_dir}/{config.input_folder_name}_preprocessed', delete_old=True)
+
+        # Save blank txt file
+        with open(f'{participant_dir}/{config.input_folder_name}_preprocessed/changes_made_to_files.txt', 'w') as f:
+            f.write('')
 
         iterable = zip(files,
                        itertools.repeat(participant_dir),
                        itertools.repeat(output_folder),
                        itertools.repeat(file_location),
                        itertools.repeat(func),
                        itertools.repeat(config))
@@ -293,112 +273,46 @@
             with open(f"{participant_dir}/{output_folder}/number_of_outliers_removed.csv", "w") as f:
                 f.write(outliers.to_csv(index=False))
 
     if config.multicore_processing:
         Utils.join_processing_pool(pool, restart=False)
 
 
-def prepare_to_run_utility(participants, output_folder, file_location, func):
-    if config.multicore_processing:
-        pool = Utils.start_processing_pool()
-    else:
-        pool = None
-
-    if config.verbose:
-        print(f'\nSaving output in directory: {config.input_folder_name}/{output_folder}')
-
-    for participant, files in participants.items():
-        participant_dir = f"{participant}/{file_location}"
-
-        if config.verbose:
-            print(f"\nRunning '{func}' utility on participant: {participant_dir.split('/')[-2]}"
-                  f"\n      Running utility on {len(files)} files")
-
-        iterable = zip(files,
-                       itertools.repeat(participant_dir),
-                       itertools.repeat(output_folder),
-                       itertools.repeat(func),
-                       itertools.repeat(config))
-
-        if config.multicore_processing:
-            list(pool.starmap(run_utility, iterable))
-
-        else:
-            list(itertools.starmap(run_utility, iterable))
-
-    if config.multicore_processing:
-        Utils.join_processing_pool(pool, restart=False)
-
-
-def run_utility(file, participant_dir, output_folder, func, cfg):
-    global config
-    config = cfg
-
-    no_ext_file = Utils.strip_ext(file)
-    file = f"{participant_dir}/{file}"
-    base_sub_location = Path(participant_dir).parents[1]
-    participant_name = os.path.split(Path(participant_dir).parents[0])[1]
-
-    if config.verbose:
-        print(f'        Running utility on file: {no_ext_file}')
-
-    if func == 'Add Gaussian noise':
-        noise_value_csv = pd.read_csv(f'{base_sub_location}/noiseValues.csv')
-        participant_noise_level = float(
-            noise_value_csv[noise_value_csv['Participant'] == participant_name]['Noise over time'])
-        add_noise_to_file(file, no_ext_file, participant_dir, output_folder, participant_noise_level)
-
-
-def add_noise_to_file(file, no_ext_file, participant_dir, output_folder, participant_noise_level):
-    data, header = Utils.load_brain(file)
-
-    # Save initial data with no added noise
-    save_brain(data, ext=f'_noiselevel0', no_ext_file=no_ext_file,
-               output_folder=f"{participant_dir}/{output_folder}", header=header)
-
-    for multiplier in config.noise_multipliers:
-        gaussian_noise = np.random.default_rng().normal(loc=0.0,
-                                                        scale=participant_noise_level * multiplier,
-                                                        size=data.shape)
-
-        noisy_data = data + gaussian_noise
-        noisy_data[noisy_data < 0] = 0  # Set values below 0 to 0
-
-        save_brain(noisy_data, ext=f'_noiselevel{multiplier}', no_ext_file=no_ext_file,
-                   output_folder=f"{participant_dir}/{output_folder}", header=header)
-
-
 def main(func, version, config_file, path=None):
     global config, config_path, config_filename
 
     start_time = time.time()
     Utils.checkversion(version)
 
     # Set global variables
     config_path = f'{Path(os.path.abspath(__file__)).parents[1]}/configuration_profiles/maps/'
     config_filename = config_file
 
     # Load config file
     config = Utils.load_config(config_path, config_file, path=path)
 
-    if config.verbose:
-        print('\n--------------------------------\n'
-              '--- Statistical map creation ---\n'
-              '--------------------------------\n'
-              f'\nCreating {func} maps.\n')
-
     logging.getLogger('nipype.workflow').setLevel(0)  # Suppress workflow terminal output
 
     if func == 'Image SNR' and not config.noise_volume and config.verbose:
         print('"Noise volume included in time series" is false. Trying to find values for each participant in '
               'noiseValues.csv instead. If this is not correct, set "Noise volume included in time series" to true.\n')
 
-    participants, output_folder, file_location = file_setup(func)
+    if func in ['Add Gaussian noise', 'Add motion', 'Separate noise volumes']:
+        print('\n--------------------------------\n'
+              '-------- Running utility --------\n'
+              '--------------------------------\n'
+              f'\nRunning {func} utility.\n')
 
-    if func in ['Add Gaussian noise']:
-        prepare_to_run_utility(participants, output_folder, file_location, func)
+        HOUSE(config, func)
 
     else:
+        if config.verbose:
+            print('\n--------------------------------\n'
+                  '--- Statistical map creation ---\n'
+                  '--------------------------------\n'
+                  f'\nCreating {func} maps.\n')
+
+        participants, output_folder, file_location = statmap_file_setup(func)
         calculate_statistical_maps(participants, output_folder, file_location, func)
 
     if config.verbose:
         print(f"\n--- Completed in {round((time.time() - start_time), 2)} seconds ---\n\n")
```

### Comparing `frat_brain-1.4.0/fRAT/utils/statmap_config_setup.py` & `frat_brain-1.5.0/fRAT/utils/statmap_config_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,23 +72,20 @@
                                             'magnitude vs complex images. \nReference: Constantinides, C. D., Atalar, '
                                             'E., & McVeigh, E. R. (1997). Signal-to-Noise Measurements in Magnitude '
                                             'Images from NMR Phased Arrays.'},
 
     'noise_volume': {'type': 'CheckButton', 'Recommended': 'false', 'label': 'Noise volume included in time series',
                      'Description': 'true or false. Select true if a noise volume has been collected as part of the fMRI '
                                     'time series.\n'
-                                    'NOTE: If true, the noise volume in the time series will be separated from the '
-                                    'functional volumes and will be placed into the folder "func_noiseVolumeRemoved".\n'
+                                    'If true, the noise volume in the time series will be separated from the '
+                                    'functional volumes and will be placed into the folder "noise_volume", and the '
+                                    'functional volumes will be placed into the "func_volumes" folder. '
                                     'If "noise volume" is true and "noise value" is not none, the noise volume '
-                                    'will be used in image SNR calculation rather than the user defined noise value.'},
-
-    'noise_volume_location': {'type': 'OptionMenu', 'Recommended': 'End', 'Options': ['Beginning', 'End'],
-                              'save_as': 'string',
-                              'Description': "'max' to select number of cores available on the system, alternatively "
-                                             "an int to manually select number of cores to use. Recommended: 'max'"},
+                                    'will be used in image SNR calculation rather than the user defined noise value.\n'
+                                    'NOTE: Use the "separate noise volume" utility before creating image SNR maps.'},
 
     'iSNR_std_use_only_nonzero_voxels': {'type': 'CheckButton', 'Recommended': 'true',
                                          'label': 'Use only nonzero voxels for iSNR calc',
                                          'Description': 'true or false.'},
 
     'Add Gaussian noise': {'type': 'subheading'},
 
@@ -110,12 +107,19 @@
                                                'participant for use in iSNR calculation. This noise value can be '
                                                'calculated as the standard deviation of voxel values outside of the '
                                                'brain. If "Noise volume included in time series" is set to true, '
                                                'standard deviation of noise will be calculated using the noise volume, '
                                                'even if a noise value has been provided in this file.'},
 
     'noise_multipliers': {'type': 'Entry', 'Recommended': 1, 'save_as': 'list', 'label': 'Noise multiplier(s)',
-                          'Description': "Provide a comma-separated list of multipliers for the standard deviation of "
-                                         "the gaussian noise to plot e.g. '1, 5'. A separate file will be produced for each multiplier."
-                                         "\nNOTE: Noise has a gaussian distribution, with a mean of 0 and a "
-                                         "standard deviation of the noise level of each participant * multiplier."}
+                          'Description': "Provide a comma-separated list of multipliers, "
+                                         "e.g. '1, 5'. A separate file will be produced for each multiplier."
+                                         "\nNOTE: Added has a gaussian distribution, with a mean of 0 and a "
+                                         "standard deviation of the noise level of each participant * multiplier."},
+
+    'motion_multipliers': {'type': 'Entry', 'Recommended': 1, 'save_as': 'list', 'label': 'Motion multiplier(s)',
+                           'Description': "Provide a comma-separated list of multipliers, "
+                                          "e.g. '1, 5'. A separate file will be produced for each multiplier."
+                                          "\nNOTE: Added motion has a gaussian distribution, with a mean of 0 and a "
+                                          "standard deviation of the average rotation/translation of each "
+                                          "participant * multiplier."},
 }
```

### Comparing `frat_brain-1.4.0/fRAT/utils/utils.py` & `frat_brain-1.5.0/fRAT/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,7 +493,14 @@
                 raise FileNotFoundError(
                     'Output folder location (fRAT output folder location) is not a valid directory.')
 
             if config.verbose:
                 print(f'Output folder selection: {json_directory}')
 
         return json_directory
+
+    @staticmethod
+    def save_brain(data, ext, no_ext_file, output_folder, header=None):
+        brain = nib.Nifti1Pair(data, None, header)
+        nib.save(brain, f"{output_folder}/{no_ext_file}{ext}.nii.gz")
+
+        return f"{output_folder}/{no_ext_file}{ext}.nii.gz"
```

### Comparing `frat_brain-1.4.0/pyproject.toml` & `frat_brain-1.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frat-brain"
-version = "1.4.0"
+version = "1.5.0"
 description = "Application for ROI fMRI data analysis."
 authors = ["Elliot Howley <elliohow@hotmail.com>"]
 readme = "README.md"
 homepage = "https://fmri-roi-analysis-tool.readthedocs.io/en/latest/"
 repository = "https://github.com/elliohow/fMRI_ROI_Analysis_Tool"
 packages = [{include = "fRAT"}]
```

### Comparing `frat_brain-1.4.0/setup.py` & `frat_brain-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['fRAT', 'fRAT.utils']
+['fRAT', 'fRAT.HOUSE', 'fRAT.utils']
 
 package_data = \
 {'': ['*'],
  'fRAT': ['configuration_profiles/*',
           'configuration_profiles/maps/*',
           'configuration_profiles/roi_analysis/*',
           'images/*']}
@@ -108,15 +108,15 @@
  'zope-interface==5.2.0']
 
 entry_points = \
 {'console_scripts': ['fRAT = fRAT.__main__:start_gui']}
 
 setup_kwargs = {
     'name': 'frat-brain',
-    'version': '1.4.0',
+    'version': '1.5.0',
     'description': 'Application for ROI fMRI data analysis.',
     'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Reporting bugs\n\nTo report a bug or suggest a new feature, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing to the project\n\nIf you\'d like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n',
     'author': 'Elliot Howley',
     'author_email': 'elliohow@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fmri-roi-analysis-tool.readthedocs.io/en/latest/',
```

### Comparing `frat_brain-1.4.0/PKG-INFO` & `frat_brain-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frat-brain
-Version: 1.4.0
+Version: 1.5.0
 Summary: Application for ROI fMRI data analysis.
 Home-page: https://fmri-roi-analysis-tool.readthedocs.io/en/latest/
 Author: Elliot Howley
 Author-email: elliohow@hotmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

