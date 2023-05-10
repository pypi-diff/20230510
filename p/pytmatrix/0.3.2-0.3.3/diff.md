# Comparing `tmp/pytmatrix-0.3.2.tar.gz` & `tmp/pytmatrix-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytmatrix-0.3.2.tar", last modified: Thu Mar 12 09:17:54 2020, max compression
+gzip compressed data, was "pytmatrix-0.3.3.tar", last modified: Wed May 10 13:43:59 2023, max compression
```

## Comparing `pytmatrix-0.3.2.tar` & `pytmatrix-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,34 @@
-drwxr-xr-x   0 leinonen (210865) lte      (20185)        0 2020-03-12 09:17:54.000000 pytmatrix-0.3.2/
--rwxrwxrwx   0 leinonen (210865) lte      (20185)     3135 2020-03-12 08:57:21.000000 pytmatrix-0.3.2/setup.py
--rw-r--r--   0 leinonen (210865) lte      (20185)      884 2020-03-12 09:17:54.000000 pytmatrix-0.3.2/PKG-INFO
-drwxr-xr-x   0 leinonen (210865) lte      (20185)        0 2020-03-12 09:17:54.000000 pytmatrix-0.3.2/pytmatrix/
-drwxr-xr-x   0 leinonen (210865) lte      (20185)        0 2020-03-12 09:17:54.000000 pytmatrix-0.3.2/pytmatrix/test/
--rw-rw-rw-   0 leinonen (210865) lte      (20185)    13042 2015-03-10 00:07:23.000000 pytmatrix-0.3.2/pytmatrix/test/test_tmatrix.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)        1 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/test/__init__.py
-drwxr-xr-x   0 leinonen (210865) lte      (20185)        0 2020-03-12 09:17:54.000000 pytmatrix-0.3.2/pytmatrix/quadrature/
--rw-rw-rw-   0 leinonen (210865) lte      (20185)     3176 2015-04-08 01:43:24.000000 pytmatrix-0.3.2/pytmatrix/quadrature/quadrature.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)        0 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/quadrature/__init__.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)    13368 2015-04-08 01:41:46.000000 pytmatrix-0.3.2/pytmatrix/tmatrix.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)     5858 2015-04-08 01:43:01.000000 pytmatrix-0.3.2/pytmatrix/tmatrix_psd.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)      678 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/ice_refr.dat
--rw-rw-rw-   0 leinonen (210865) lte      (20185)     3216 2020-03-12 08:58:23.000000 pytmatrix-0.3.2/pytmatrix/tmatrix_aux.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)     4470 2015-04-08 01:42:35.000000 pytmatrix-0.3.2/pytmatrix/radar.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)    17666 2019-07-02 10:12:00.000000 pytmatrix-0.3.2/pytmatrix/psd.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)     4905 2016-02-26 00:08:23.000000 pytmatrix-0.3.2/pytmatrix/orientation.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)     5923 2015-04-08 01:42:49.000000 pytmatrix-0.3.2/pytmatrix/scatter.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)        1 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/__init__.py
-drwxr-xr-x   0 leinonen (210865) lte      (20185)        0 2020-03-12 09:17:54.000000 pytmatrix-0.3.2/pytmatrix/fortran_tm/
--rw-rw-rw-   0 leinonen (210865) lte      (20185)      166 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/fortran_tm/ampld.par.f
--rw-rw-rw-   0 leinonen (210865) lte      (20185)    68962 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/fortran_tm/ampld.lp.f
--rw-rw-rw-   0 leinonen (210865) lte      (20185)     1168 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/fortran_tm/pytmatrix.pyf
--rw-rw-rw-   0 leinonen (210865) lte      (20185)        0 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/fortran_tm/__init__.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)   116546 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/pytmatrix/fortran_tm/lpd.f
--rw-rw-rw-   0 leinonen (210865) lte      (20185)     4947 2015-04-08 01:42:42.000000 pytmatrix-0.3.2/pytmatrix/refractive.py
--rw-rw-rw-   0 leinonen (210865) lte      (20185)       26 2015-03-10 03:45:52.000000 pytmatrix-0.3.2/setup.cfg
--rw-rw-rw-   0 leinonen (210865) lte      (20185)        0 2014-04-11 07:09:09.000000 pytmatrix-0.3.2/README
+drwxr-xr-x   0 jleinone (25897) msclim   (30631)        0 2023-05-10 13:43:59.428167 pytmatrix-0.3.3/
+-rw-r--r--   0 jleinone (25897) msclim   (30631)     1071 2023-05-10 10:23:25.000000 pytmatrix-0.3.3/LICENSE
+-rw-r--r--   0 jleinone (25897) msclim   (30631)        0 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/MANIFEST.in
+-rw-r--r--   0 jleinone (25897) msclim   (30631)      861 2023-05-10 13:43:59.428320 pytmatrix-0.3.3/PKG-INFO
+-rw-r--r--   0 jleinone (25897) msclim   (30631)        0 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/README
+drwxr-xr-x   0 jleinone (25897) msclim   (30631)        0 2023-05-10 13:43:59.423174 pytmatrix-0.3.3/pytmatrix/
+-rw-r--r--   0 jleinone (25897) msclim   (30631)        1 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/__init__.py
+drwxr-xr-x   0 jleinone (25897) msclim   (30631)        0 2023-05-10 13:43:59.425956 pytmatrix-0.3.3/pytmatrix/fortran_tm/
+-rw-r--r--   0 jleinone (25897) msclim   (30631)        0 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/fortran_tm/__init__.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)    68962 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/fortran_tm/ampld.lp.f
+-rw-r--r--   0 jleinone (25897) msclim   (30631)      166 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/fortran_tm/ampld.par.f
+-rw-r--r--   0 jleinone (25897) msclim   (30631)   116546 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/fortran_tm/lpd.f
+-rw-r--r--   0 jleinone (25897) msclim   (30631)      678 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/ice_refr.dat
+-rw-r--r--   0 jleinone (25897) msclim   (30631)     4911 2023-05-10 10:21:09.000000 pytmatrix-0.3.3/pytmatrix/orientation.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)    18113 2023-05-10 10:19:56.000000 pytmatrix-0.3.3/pytmatrix/psd.py
+drwxr-xr-x   0 jleinone (25897) msclim   (30631)        0 2023-05-10 13:43:59.426732 pytmatrix-0.3.3/pytmatrix/quadrature/
+-rw-r--r--   0 jleinone (25897) msclim   (30631)        0 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/quadrature/__init__.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)     3176 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/quadrature/quadrature.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)     4470 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/radar.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)     4947 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/refractive.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)     6035 2023-05-10 10:19:50.000000 pytmatrix-0.3.3/pytmatrix/scatter.py
+drwxr-xr-x   0 jleinone (25897) msclim   (30631)        0 2023-05-10 13:43:59.427343 pytmatrix-0.3.3/pytmatrix/test/
+-rw-r--r--   0 jleinone (25897) msclim   (30631)        1 2022-03-02 18:34:25.000000 pytmatrix-0.3.3/pytmatrix/test/__init__.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)    14105 2023-05-10 12:05:23.000000 pytmatrix-0.3.3/pytmatrix/test/test_tmatrix.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)    13368 2023-05-10 10:09:56.000000 pytmatrix-0.3.3/pytmatrix/tmatrix.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)     3224 2023-05-10 10:25:08.000000 pytmatrix-0.3.3/pytmatrix/tmatrix_aux.py
+-rw-r--r--   0 jleinone (25897) msclim   (30631)     5820 2023-05-10 10:16:49.000000 pytmatrix-0.3.3/pytmatrix/tmatrix_psd.py
+drwxr-xr-x   0 jleinone (25897) msclim   (30631)        0 2023-05-10 13:43:59.424649 pytmatrix-0.3.3/pytmatrix.egg-info/
+-rw-r--r--   0 jleinone (25897) msclim   (30631)      861 2023-05-10 13:43:59.423625 pytmatrix-0.3.3/pytmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 jleinone (25897) msclim   (30631)      650 2023-05-10 13:43:59.424184 pytmatrix-0.3.3/pytmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 jleinone (25897) msclim   (30631)        1 2023-05-10 13:43:59.424462 pytmatrix-0.3.3/pytmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 jleinone (25897) msclim   (30631)       10 2023-05-10 13:43:59.424739 pytmatrix-0.3.3/pytmatrix.egg-info/top_level.txt
+-rw-r--r--   0 jleinone (25897) msclim   (30631)       67 2023-05-10 13:43:59.428715 pytmatrix-0.3.3/setup.cfg
+-rwxr-xr-x   0 jleinone (25897) msclim   (30631)     3135 2023-05-10 10:22:20.000000 pytmatrix-0.3.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytmatrix-0.3.2/setup.py` & `pytmatrix-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 """
 
 import sys
 
 def configuration(parent_package='',top_path=None):
     from numpy.distutils.misc_util import Configuration
     config = Configuration('pytmatrix', parent_package, top_path,
-        version = '0.3.2',
+        version = '0.3.3',
         author  = "Jussi Leinonen",
         author_email = "jsleinonen@gmail.com",
         description = "T-matrix scattering computations",
         license = "MIT",
         url = 'https://github.com/jleinonen/pytmatrix',
         download_url = \
-            'https://github.com/jleinonen/pytmatrix/releases/download/0.3.1/pytmatrix-0.3.1.zip',
+            'https://github.com/jleinonen/pytmatrix/releases/download/0.3.3/pytmatrix-0.3.3.zip',
         long_description = long_description,
         classifiers = [
             "Development Status :: 4 - Beta",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
             "Programming Language :: Fortran",
```

### Comparing `pytmatrix-0.3.2/PKG-INFO` & `pytmatrix-0.3.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pytmatrix
-Version: 0.3.2
+Version: 0.3.3
 Summary: T-matrix scattering computations
 Home-page: https://github.com/jleinonen/pytmatrix
+Download-URL: https://github.com/jleinonen/pytmatrix/releases/download/0.3.3/pytmatrix-0.3.3.zip
 Author: Jussi Leinonen
 Author-email: jsleinonen@gmail.com
 License: MIT
-Download-URL: https://github.com/jleinonen/pytmatrix/releases/download/0.3.1/pytmatrix-0.3.1.zip
-Description: A Python code for computing the scattering properties
-        of homogeneous nonspherical scatterers with the T-Matrix method.
-        
-        Requires NumPy and SciPy.
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Fortran
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires: numpy
 Requires: scipy
+License-File: LICENSE
+
+A Python code for computing the scattering properties
+of homogeneous nonspherical scatterers with the T-Matrix method.
+
+Requires NumPy and SciPy.
```

### Comparing `pytmatrix-0.3.2/pytmatrix/test/test_tmatrix.py` & `pytmatrix-0.3.3/pytmatrix/test/test_tmatrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2009-2013 Jussi Leinonen
+Copyright (C) 2009-2023 Jussi Leinonen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
@@ -320,16 +320,39 @@
 
         # This size-integrated scattering cross section has an analytical value.
         # Check that we can reproduce it.
         sca_xsect_ref = 480*N0*np.pi**5*abs(K)**2/Lambda**7
         sca_xsect = scatter.sca_xsect(sca)
         test_less(self, abs(1-sca_xsect/sca_xsect_ref), 1e-3)
 
+    def test_attn_polarization(self):
+        """Test attenuation calculation for multiple polarization with PSD.
+        """
 
+        wavelength = tmatrix_aux.wl_C
+        m = refractive.m_w_20C[wavelength]
+        K = (m**2-1)/(m**2+2)
+        diam_max = 0.75
+        gamma_psd = psd.GammaPSD(D0=0.25, Nw=10e3, mu=0, D_max=diam_max)
 
+        sca = Scatterer(wavelength=wavelength, m=m)
+        sca.axis_ratio = 1.0/0.6
+        sca.psd_integrator = psd.PSDIntegrator()        
+        sca.psd = gamma_psd
+        sca.psd_integrator.D_max = sca.psd.D_max
+        # 64 is quite low, but we want to run the test reasonably fast
+        sca.psd_integrator.num_points = 64
+        sca.psd_integrator.init_scatter_table(sca, angular_integration=True)
+
+        self.assertEqual(radar.Ai(sca), radar.Ai(sca, h_pol=True))
+        test_less(self, 0, radar.Ai(sca, h_pol=True))
+        test_less(self, 0, radar.Ai(sca, h_pol=False))
+        # Check that we have differential attenuation
+        test_less(self, radar.Ai(sca, h_pol=False), radar.Ai(sca, h_pol=True))
+        
 
 def test_relative(tests, x, x_ref, limit=epsilon):
     abs_diff = abs(x-x_ref)
     rel_diff = abs_diff/abs(x_ref)
     try:
         shape = x.shape
         if not shape:
```

### Comparing `pytmatrix-0.3.2/pytmatrix/quadrature/quadrature.py` & `pytmatrix-0.3.3/pytmatrix/quadrature/quadrature.py`

 * *Files identical despite different names*

### Comparing `pytmatrix-0.3.2/pytmatrix/tmatrix.py` & `pytmatrix-0.3.3/pytmatrix/tmatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import warnings
 import numpy as np
 from pytmatrix.fortran_tm import pytmatrix
 from pytmatrix.quadrature import quadrature
 import pytmatrix.orientation as orientation
 
 
-
 class Scatterer(object):
     """T-Matrix scattering from nonspherical particles.
 
     Class for simulating scattering from nonspherical particles with the 
     T-Matrix method. Uses a wrapper to the Fortran code by M. Mishchenko.
 
     Usage instructions:
@@ -245,20 +244,20 @@
 
 
     def equal_volume_from_maximum(self):
         if self.shape == Scatterer.SHAPE_SPHEROID:
             if self.axis_ratio > 1.0: # oblate
                 r_eq = self.radius/self.axis_ratio**(1.0/3.0)
             else: # prolate
-                r_eq = self.radius/self.axis_ratio**(2.0/3.0)
+                r_eq = self.radius*self.axis_ratio**(2.0/3.0)
         elif self.shape == Scatterer.SHAPE_CYLINDER:
             if self.axis_ratio > 1.0: # oblate
-                r_eq = self.radius*(0.75/self.axis_ratio)**(1.0/3.0)
+                r_eq = self.radius*(1.5/self.axis_ratio)**(1.0/3.0)
             else: # prolate
-                r_eq = self.radius*(0.75/self.axis_ratio)**(2.0/3.0)
+                r_eq = self.radius*(1.5*self.axis_ratio**2)**(1.0/3.0)
         else:
             raise AttributeError("Unsupported shape for maximum radius.")
         return r_eq
 
 
     def get_SZ_single(self, alpha=None, beta=None):
         """Get the S and Z matrices for a single orientation.
```

### Comparing `pytmatrix-0.3.2/pytmatrix/tmatrix_psd.py` & `pytmatrix-0.3.3/pytmatrix/tmatrix_psd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2009-2013 Jussi LeinonenCopyright (C) 2009-2015 Jussi Leinonen, Finnish Meteorological Institute, 
+Copyright (C) 2009-2015 Jussi Leinonen, Finnish Meteorological Institute, 
 California Institute of Technology
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `pytmatrix-0.3.2/pytmatrix/ice_refr.dat` & `pytmatrix-0.3.3/pytmatrix/ice_refr.dat`

 * *Files identical despite different names*

### Comparing `pytmatrix-0.3.2/pytmatrix/tmatrix_aux.py` & `pytmatrix-0.3.3/pytmatrix/tmatrix_aux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2009-2015 Jussi Leinonen, Finnish Meteorological Institute, 
+Copyright (C) 2009-2023 Jussi Leinonen, Finnish Meteorological Institute, 
 California Institute of Technology
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
@@ -17,15 +17,15 @@
 FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 
 #current version
-VERSION = "0.3.2"
+VERSION = "0.3.3"
 
 #typical wavelengths [mm] at different bands
 wl_S = 111.0
 wl_C = 53.5
 wl_X = 33.3
 wl_Ku = 22.0
 wl_Ka = 8.43
@@ -72,22 +72,22 @@
 
     Arguments:
         D_eq: Drop volume-equivalent diameter (mm)
     Returns:
         r: The vertical-to-horizontal drop axis ratio. Note: the Scatterer class
         expects horizontal to vertical, so you should pass 1/dsr_pb
     """
-    return 1.03-0.062*D_eq
+    return 1.03 - 0.062*D_eq
 
 
 def dsr_bc(D_eq):
     """
     Beard and Chuang drop shape relationship function.
     Arguments:
         D_eq: Drop volume-equivalent diameter (mm)
     Returns:
         r: The vertical-to-horizontal drop axis ratio. Note: the Scatterer class
         expects horizontal to vertical, so you should pass 1/dsr_bc
     """
 
-    return 1.0048 + 5.7e-04 - 2.628e-02 * D_eq**2 +\
+    return 1.0048 + 5.7e-04*D_eq - 2.628e-02 * D_eq**2 + \
         3.682e-03*D_eq**3 - 1.677e-04 * D_eq**4
```

### Comparing `pytmatrix-0.3.2/pytmatrix/radar.py` & `pytmatrix-0.3.3/pytmatrix/radar.py`

 * *Files identical despite different names*

### Comparing `pytmatrix-0.3.2/pytmatrix/psd.py` & `pytmatrix-0.3.3/pytmatrix/psd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2009-2015 Jussi Leinonen, Finnish Meteorological Institute, 
+Copyright (C) 2009-2023 Jussi Leinonen, Finnish Meteorological Institute, 
 California Institute of Technology
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
@@ -330,42 +330,43 @@
                     trapz(self._Z_table[geom] * psd_w, self._psd_D)
 
             self._previous_psd = psd
 
         return (self._S_dict[geometry], self._Z_dict[geometry])
 
 
-    def get_angular_integrated(self, psd, geometry, property_name):
+    def get_angular_integrated(self, psd, geometry, property_name, h_pol=True):
         if self._angular_table is None:
             raise AttributeError(
                 "Initialize or load the table of angular-integrated " + 
                 "quantities first."
             )
 
+        pol = "h_pol" if h_pol else "v_pol"
         psd_w = psd(self._psd_D)
 
         def sca_xsect(geom):
             return trapz(
-                self._angular_table["sca_xsect"][geom] * psd_w, 
+                self._angular_table["sca_xsect"][pol][geom] * psd_w, 
                 self._psd_D
             )
     
         if property_name == "sca_xsect":
             sca_prop = sca_xsect(geometry)
         elif property_name == "ext_xsect":
             sca_prop = trapz(
-                self._angular_table["ext_xsect"][geometry] * psd_w, 
+                self._angular_table["ext_xsect"][pol][geometry] * psd_w, 
                 self._psd_D
             )
         elif property_name == "asym":
             sca_xsect_int = sca_xsect(geometry)
             if sca_xsect_int > 0:
                 sca_prop = trapz(
-                    self._angular_table["asym"][geometry] * \
-                    self._angular_table["sca_xsect"][geometry] * psd_w,  
+                    self._angular_table["asym"][pol][geometry] * \
+                    self._angular_table["sca_xsect"][pol][geometry] * psd_w,  
                     self._psd_D
                 )
                 sca_prop /= sca_xsect_int
             else:
                 sca_prop = 0.0
 
         return sca_prop
@@ -395,16 +396,19 @@
             self.num_points)
 
         self._S_table = {}
         self._Z_table = {}
         self._previous_psd = None
         self._m_table = np.empty(self.num_points, dtype=complex)
         if angular_integration:
-            self._angular_table = {"sca_xsect": {}, "ext_xsect": {}, 
-                "asym": {}}
+            self._angular_table = {
+                "sca_xsect": {"h_pol": {}, "v_pol": {}},
+                "ext_xsect": {"h_pol": {}, "v_pol": {}}, 
+                "asym": {"h_pol": {}, "v_pol": {}}
+            }
         else:
             self._angular_table = None
         
         (old_m, old_axis_ratio, old_radius, old_geom, old_psd_integrator) = \
             (tm.m, tm.axis_ratio, tm.radius, tm.get_geometry(), 
                 tm.psd_integrator)
         
@@ -415,16 +419,17 @@
             for geom in self.geometries:
                 self._S_table[geom] = \
                     np.empty((2,2,self.num_points), dtype=complex)
                 self._Z_table[geom] = np.empty((4,4,self.num_points))
 
                 if angular_integration:
                     for int_var in ["sca_xsect", "ext_xsect", "asym"]:
-                        self._angular_table[int_var][geom] = \
-                            np.empty(self.num_points)
+                        for pol in ["h_pol", "v_pol"]:
+                            self._angular_table[int_var][pol][geom] = \
+                                np.empty(self.num_points)
 
             for (i,D) in enumerate(self._psd_D):
                 if verbose:
                     print("Computing point {i} at D={D}...".format(i=i, D=D))
                 if self.m_func != None:
                     tm.m = self.m_func(D)
                 if self.axis_ratio_func != None:
@@ -434,28 +439,29 @@
                 for geom in self.geometries:
                     tm.set_geometry(geom)
                     (S, Z) = tm.get_SZ_orient()
                     self._S_table[geom][:,:,i] = S
                     self._Z_table[geom][:,:,i] = Z
 
                     if angular_integration:
-                        self._angular_table["sca_xsect"][geom][i] = \
-                            scatter.sca_xsect(tm)
-                        self._angular_table["ext_xsect"][geom][i] = \
-                            scatter.ext_xsect(tm)
-                        self._angular_table["asym"][geom][i] = \
-                            scatter.asym(tm)
+                        for pol in ["h_pol", "v_pol"]:
+                            h_pol = (pol == "h_pol")
+                            self._angular_table["sca_xsect"][pol][geom][i] = \
+                                scatter.sca_xsect(tm, h_pol=h_pol)
+                            self._angular_table["ext_xsect"][pol][geom][i] = \
+                                scatter.ext_xsect(tm, h_pol=h_pol)
+                            self._angular_table["asym"][pol][geom][i] = \
+                                scatter.asym(tm, h_pol=h_pol)
         finally:
             #restore old values
             (tm.m, tm.axis_ratio, tm.radius, tm.psd_integrator) = \
                 (old_m, old_axis_ratio, old_radius, old_psd_integrator) 
             tm.set_geometry(old_geom)
 
 
-
     def save_scatter_table(self, fn, description=""):
         """Save the scattering lookup tables.
         
         Save the state of the scattering lookup tables to a file.
         This can be loaded later with load_scatter_table.
 
         Other variables will not be saved, but this does not matter because
```

### Comparing `pytmatrix-0.3.2/pytmatrix/orientation.py` & `pytmatrix-0.3.3/pytmatrix/orientation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2009-2015 Jussi Leinonen, Finnish Meteorological Institute, 
+Copyright (C) 2009-2023 Jussi Leinonen, Finnish Meteorological Institute, 
 California Institute of Technology
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
@@ -63,15 +63,15 @@
     return pdf
 
 
 def orient_single(tm):
     """Compute the T-matrix using a single orientation scatterer.
 
     Args:
-        tm: TMatrix (or descendant) instance
+        tm: Scatterer (or descendant) instance
 
     Returns:
         The amplitude (S) and phase (Z) matrices.
     """
     return tm.get_SZ_single()
 
 
@@ -79,15 +79,15 @@
     """Compute the T-matrix using variable orientation scatterers.
     
     This method uses a very slow adaptive routine and should mainly be used
     for reference purposes. Uses the set particle orientation PDF, ignoring
     the alpha and beta attributes.
 
     Args:
-        tm: TMatrix (or descendant) instance
+        tm: Scatterer (or descendant) instance
 
     Returns:
         The amplitude (S) and phase (Z) matrices.
     """
     S = np.zeros((2,2), dtype=complex)
     Z = np.zeros((4,4))
 
@@ -121,15 +121,15 @@
     """Compute the T-matrix using variable orientation scatterers.
     
     This method uses a fast Gaussian quadrature and is suitable
     for most use. Uses the set particle orientation PDF, ignoring
     the alpha and beta attributes.
 
     Args:
-        tm: TMatrix (or descendant) instance.
+        tm: Scatterer (or descendant) instance.
 
     Returns:
         The amplitude (S) and phase (Z) matrices.
     """
     S = np.zeros((2,2), dtype=complex)
     Z = np.zeros((4,4))
     ap = np.linspace(0, 360, tm.n_alpha+1)[:-1]
```

### Comparing `pytmatrix-0.3.2/pytmatrix/scatter.py` & `pytmatrix-0.3.3/pytmatrix/scatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (C) 2009-2015 Jussi Leinonen, Finnish Meteorological Institute, 
+Copyright (C) 2009-2023 Jussi Leinonen, Finnish Meteorological Institute, 
 California Institute of Technology
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
@@ -74,15 +74,17 @@
 
     Returns:
         The scattering cross section.
     """
 
     if scatterer.psd_integrator is not None:
         return scatterer.psd_integrator.get_angular_integrated(
-            scatterer.psd, scatterer.get_geometry(), "sca_xsect")
+            scatterer.psd, scatterer.get_geometry(), "sca_xsect",
+            h_pol=h_pol
+        )
 
     old_geom = scatterer.get_geometry()    
 
     def d_xsect(thet, phi):
         (scatterer.phi, scatterer.thet) = (phi*rad_to_deg, thet*rad_to_deg)        
         Z = scatterer.get_Z()        
         I = sca_intensity(scatterer, h_pol)
@@ -108,29 +110,29 @@
     Returns:
         The extinction cross section.
     """
 
     if scatterer.psd_integrator is not None:
         try:
             return scatterer.psd_integrator.get_angular_integrated(
-                scatterer.psd, scatterer.get_geometry(), "ext_xsect")
+                scatterer.psd, scatterer.get_geometry(), "ext_xsect",
+                h_pol=h_pol
+            )
         except AttributeError:
             # Fall back to the usual method of computing this from S
             pass
 
     old_geom = scatterer.get_geometry()
     (thet0, thet, phi0, phi, alpha, beta) = old_geom
     try:
         scatterer.set_geometry((thet0, thet0, phi0, phi0, alpha, beta))
         S = scatterer.get_S()        
     finally:
         scatterer.set_geometry(old_geom)
 
-
-
     if h_pol:
         return 2 * scatterer.wavelength * S[1,1].imag
     else:
         return 2 * scatterer.wavelength * S[0,0].imag
 
 
 def ssa(scatterer, h_pol=True):
@@ -159,15 +161,17 @@
 
     Returns:
         The asymmetry parameter.
     """
 
     if scatterer.psd_integrator is not None:
         return scatterer.psd_integrator.get_angular_integrated(
-            scatterer.psd, scatterer.get_geometry(), "asym")
+            scatterer.psd, scatterer.get_geometry(), "asym",
+            h_pol=h_pol    
+        )
 
     old_geom = scatterer.get_geometry()
 
     cos_t0 = np.cos(scatterer.thet0 * deg_to_rad)
     sin_t0 = np.sin(scatterer.thet0 * deg_to_rad)
     p0 = scatterer.phi0 * deg_to_rad
     def integrand(thet, phi):
```

### Comparing `pytmatrix-0.3.2/pytmatrix/fortran_tm/ampld.lp.f` & `pytmatrix-0.3.3/pytmatrix/fortran_tm/ampld.lp.f`

 * *Files identical despite different names*

### Comparing `pytmatrix-0.3.2/pytmatrix/fortran_tm/lpd.f` & `pytmatrix-0.3.3/pytmatrix/fortran_tm/lpd.f`

 * *Files identical despite different names*

### Comparing `pytmatrix-0.3.2/pytmatrix/refractive.py` & `pytmatrix-0.3.3/pytmatrix/refractive.py`

 * *Files identical despite different names*

