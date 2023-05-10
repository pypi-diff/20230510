# Comparing `tmp/utracto-0.0.5.tar.gz` & `tmp/utracto-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utracto-0.0.5.tar", last modified: Wed May 10 12:52:29 2023, max compression
+gzip compressed data, was "utracto-0.0.6.tar", last modified: Wed May 10 13:12:56 2023, max compression
```

## Comparing `utracto-0.0.5.tar` & `utracto-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:52:29.600000 utracto-0.0.5/
--rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1893 2023-05-10 12:52:30.000000 utracto-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1392 2023-05-10 12:17:46.000000 utracto-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 12:52:30.000000 utracto-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1070 2023-05-10 12:33:10.000000 utracto-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:52:29.620000 utracto-0.0.5/utracto/
--rw-rw-rw-   0        0        0       74 2023-05-10 12:52:22.000000 utracto-0.0.5/utracto/__init__.py
--rw-rw-rw-   0        0        0     2690 2022-12-13 15:12:08.000000 utracto-0.0.5/utracto/core.py
--rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.5/utracto/example.py
--rw-rw-rw-   0        0        0     5932 2023-05-10 12:48:36.000000 utracto-0.0.5/utracto/tracking.py
--rw-rw-rw-   0        0        0     5172 2023-05-10 12:44:16.000000 utracto-0.0.5/utracto/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:52:29.620000 utracto-0.0.5/utracto.egg-info/
--rw-rw-rw-   0        0        0     1893 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 12:52:30.000000 utracto-0.0.5/utracto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-10 13:12:56.740000 utracto-0.0.6/
+-rw-rw-rw-   0        0        0    35823 2022-11-24 12:53:54.000000 utracto-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1893 2023-05-10 13:12:58.000000 utracto-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1392 2023-05-10 12:17:46.000000 utracto-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 13:12:58.000000 utracto-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2023-05-10 13:04:52.000000 utracto-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:12:56.740000 utracto-0.0.6/utracto/
+-rw-rw-rw-   0        0        0       74 2023-05-10 13:12:42.000000 utracto-0.0.6/utracto/__init__.py
+-rw-rw-rw-   0        0        0     2690 2022-12-13 15:12:08.000000 utracto-0.0.6/utracto/core.py
+-rw-rw-rw-   0        0        0      480 2022-12-12 15:40:08.000000 utracto-0.0.6/utracto/example.py
+-rw-rw-rw-   0        0        0     5822 2023-05-10 13:10:26.000000 utracto-0.0.6/utracto/tracking.py
+-rw-rw-rw-   0        0        0     5172 2023-05-10 12:44:16.000000 utracto-0.0.6/utracto/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 13:12:56.750000 utracto-0.0.6/utracto.egg-info/
+-rw-rw-rw-   0        0        0     1893 2023-05-10 13:12:58.000000 utracto-0.0.6/utracto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-05-10 13:12:58.000000 utracto-0.0.6/utracto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 13:12:58.000000 utracto-0.0.6/utracto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-10 13:12:58.000000 utracto-0.0.6/utracto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 13:12:58.000000 utracto-0.0.6/utracto.egg-info/top_level.txt
```

### Comparing `utracto-0.0.5/LICENSE` & `utracto-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `utracto-0.0.5/PKG-INFO` & `utracto-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `utracto-0.0.5/README.md` & `utracto-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `utracto-0.0.5/setup.py` & `utracto-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     author_email='nicolas.delinte@uclouvain.be',
     license='GNU General Public License v3.0',
     packages=['utracto'],
     install_requires=['dipy',
                       'nibabel',
                       'numpy',
                       'tqdm',
+			    'pilab-binama',
                       ],
 
     classifiers=['Development Status :: 4 - Beta',
                  'Intended Audience :: Science/Research',
                  'Natural Language :: English',
                  'Programming Language :: Python'],
 )
```

### Comparing `utracto-0.0.5/utracto/core.py` & `utracto-0.0.6/utracto/core.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.5/utracto/tracking.py` & `utracto-0.0.6/utracto/tracking.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from dipy.data import get_sphere
 from dipy.reconst.csdeconv import (ConstrainedSphericalDeconvModel,
                                    auto_response_ssst)
 from binama.utils import dilation
 from utracto.utils import mrtrix_fod_to_dipy
 
 
-def brainTracking(Patient_files, params, seed_files=None, target_files=None,
-                  all_seed=False, dilate=[0, 0], in_fod=None,
-                  in_fod_from_mrtrix=False, angle_var=None,
-                  wmfod=None, ptt: bool = False):
+def brain_tracking(Patient_files, params, seed_files=None, target_files=None,
+                   all_seed: bool = False, dilate=[0, 0], in_fod=None,
+                   in_fod_from_mrtrix: bool = False, angle_var=None,
+                   wmfod=None, ptt: bool = False):
     '''
 
 
     Parameters
     ----------
     Patient_files : path to diffusion files + filename (without extension)
     params : parameters dictionary (ex: {'fa_thr':.6,'gfa_thresh':.35,
@@ -52,21 +52,22 @@
 
     if all_seed:
         seed_mask = np.ones(data.shape[:-1])
         white_matter = seed_mask.copy()
 
     else:
 
-        mask_data, white_matter = median_otsu(data, vol_idx=[0, 1], median_radius=4, numpass=2,
+        mask_data, white_matter = median_otsu(data, vol_idx=[0, 1],
+                                              median_radius=4, numpass=2,
                                               autocrop=False, dilate=1)
         # white_matter=load_nifti_data(root+Patient+mas_dir+Patient+'_wm_mask'+'.nii.gz')
 
         seed_mask = white_matter
 
-    if seed_files != None:
+    if seed_files is not None:
         if type(seed_files[0]) == str:
             seed_mask = load_nifti_data(seed_files[0]+'.nii.gz')
             for i in range(1, len(seed_files)):
                 seed_mask += load_nifti_data(seed_files[i]+'.nii.gz')
                 seed_mask[seed_mask > 1] = 1
         else:
             seed_mask = seed_files[0]
@@ -77,18 +78,14 @@
     if in_fod is None:
         response, ratio = auto_response_ssst(
             gtab, data, roi_radii=10, fa_thr=params['fa_thr'])
         csd_model = ConstrainedSphericalDeconvModel(gtab, response, sh_order=8)
         csd_fit = csd_model.fit(data, mask=white_matter)
         fod = csd_fit.shm_coeff
 
-        # # Temp
-        # out = nib.Nifti1Image(csd_fit.shm_coeff, img.affine, img.header)
-        # out.to_filename('C:/users/nicol/Desktop/disco_dipy_fod.nii.gz')
-
     else:
         fod = in_fod
 
     if wmfod is None:
 
         from dipy.reconst.shm import CsaOdfModel
 
@@ -107,26 +104,24 @@
 
     # SH
     default_sphere = get_sphere('repulsion724')
 
     if in_fod_from_mrtrix:
         print('Tournier convention used for SH')
 
-        # # Temp
-        # out = nib.Nifti1Image(fod, img.affine, img.header)
-        # out.to_filename('C:/users/nicol/Desktop/disco_mrtrix_dipy_fod.nii.gz')
-
         fod = mrtrix_fod_to_dipy(fod)
 
     if ptt:
 
         fod = csd_fit.odf(default_sphere)
         pmf = fod.clip(min=0)
-        prob_dg = PTTDirectionGetter.from_pmf(pmf, max_angle=params['max_angle'],
-                                              probe_length=0.5,
+        prob_dg = PTTDirectionGetter.from_pmf(pmf,
+                                              max_angle=params['max_angle'],
+                                              probe_length=params['probe_length'],
+                                              probe_radius=params['probe_radius'],
                                               sphere=default_sphere)
 
     elif angle_var is None:
         prob_dg = ProbabilisticDirectionGetter.from_shcoeff(fod,
                                                             max_angle=params['max_angle'],
                                                             sphere=default_sphere)
 
@@ -140,15 +135,15 @@
                                                             )
         print('launching with modified DIPY')
 
     streamline_generator = LocalTracking(prob_dg, stopping_criterion, seeds,
                                          affine, step_size=params['step_size'])
     streamlines = Streamlines(streamline_generator)
 
-    if target_files != None:
+    if target_files is not None:
         for i, target_file in enumerate(target_files):
             if len(dilate[1]) > 1:
                 dilat = dilate[1][i]
             else:
                 dilat = dilate[1][0]
             target_roi = load_nifti_data(target_file+'.nii.gz')
             target_roi = dilation(target_roi, dilat)
```

### Comparing `utracto-0.0.5/utracto/utils.py` & `utracto-0.0.6/utracto/utils.py`

 * *Files identical despite different names*

### Comparing `utracto-0.0.5/utracto.egg-info/PKG-INFO` & `utracto-0.0.6/utracto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utracto
-Version: 0.0.5
+Version: 0.0.6
 Summary: Implementation of UTracto
 Home-page: https://github.com/DelinteNicolas/UTracto
 Author: Nicolas Delinte
 Author-email: nicolas.delinte@uclouvain.be
 License: GNU General Public License v3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

