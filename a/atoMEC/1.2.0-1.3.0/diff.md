# Comparing `tmp/atoMEC-1.2.0.tar.gz` & `tmp/atoMEC-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atoMEC-1.2.0.tar", last modified: Mon Nov 28 14:02:45 2022, max compression
+gzip compressed data, was "atoMEC-1.3.0.tar", last modified: Wed May 10 08:45:30 2023, max compression
```

## Comparing `atoMEC-1.2.0.tar` & `atoMEC-1.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-28 14:02:45.280519 atoMEC-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1570 2022-11-28 14:02:33.000000 atoMEC-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       16 2022-11-28 14:02:33.000000 atoMEC-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7825 2022-11-28 14:02:45.280519 atoMEC-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5671 2022-11-28 14:02:33.000000 atoMEC-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-28 14:02:45.276519 atoMEC-1.2.0/atoMEC/
--rw-r--r--   0 runner    (1001) docker     (116)     7335 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    34181 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/check_inputs.py
--rw-r--r--   0 runner    (1001) docker     (116)      959 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/config.py
--rw-r--r--   0 runner    (1001) docker     (116)     3494 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/convergence.py
--rw-r--r--   0 runner    (1001) docker     (116)    13154 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (116)    17757 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/models.py
--rw-r--r--   0 runner    (1001) docker     (116)    20734 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/numerov.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-28 14:02:45.280519 atoMEC-1.2.0/atoMEC/postprocess/
--rw-r--r--   0 runner    (1001) docker     (116)       69 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/postprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    35597 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/postprocess/conductivity.py
--rw-r--r--   0 runner    (1001) docker     (116)    12729 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/postprocess/localization.py
--rw-r--r--   0 runner    (1001) docker     (116)     9611 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/postprocess/pressure.py
--rw-r--r--   0 runner    (1001) docker     (116)    50681 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/staticKS.py
--rw-r--r--   0 runner    (1001) docker     (116)      182 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/unitconv.py
--rw-r--r--   0 runner    (1001) docker     (116)    20542 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/writeoutput.py
--rw-r--r--   0 runner    (1001) docker     (116)    13303 2022-11-28 14:02:33.000000 atoMEC-1.2.0/atoMEC/xc.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-28 14:02:45.280519 atoMEC-1.2.0/atoMEC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7825 2022-11-28 14:02:45.000000 atoMEC-1.2.0/atoMEC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      543 2022-11-28 14:02:45.000000 atoMEC-1.2.0/atoMEC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-28 14:02:45.000000 atoMEC-1.2.0/atoMEC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      286 2022-11-28 14:02:45.000000 atoMEC-1.2.0/atoMEC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-11-28 14:02:45.000000 atoMEC-1.2.0/atoMEC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      104 2022-11-28 14:02:33.000000 atoMEC-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-28 14:02:45.280519 atoMEC-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)      825 2022-11-28 14:02:33.000000 atoMEC-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:45:30.761155 atoMEC-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-10 08:45:19.000000 atoMEC-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 08:45:19.000000 atoMEC-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-05-10 08:45:30.761155 atoMEC-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-10 08:45:19.000000 atoMEC-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:45:30.757155 atoMEC-1.3.0/atoMEC/
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34817 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/check_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20734 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/numerov.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:45:30.761155 atoMEC-1.3.0/atoMEC/postprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/postprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35597 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/postprocess/conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/postprocess/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/postprocess/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53200 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/staticKS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/unitconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20542 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/writeoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-05-10 08:45:19.000000 atoMEC-1.3.0/atoMEC/xc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:45:30.761155 atoMEC-1.3.0/atoMEC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-05-10 08:45:30.000000 atoMEC-1.3.0/atoMEC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-10 08:45:30.000000 atoMEC-1.3.0/atoMEC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:45:30.000000 atoMEC-1.3.0/atoMEC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-10 08:45:30.000000 atoMEC-1.3.0/atoMEC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 08:45:30.000000 atoMEC-1.3.0/atoMEC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 08:45:19.000000 atoMEC-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 08:45:30.761155 atoMEC-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      825 2023-05-10 08:45:19.000000 atoMEC-1.3.0/setup.py
```

### Comparing `atoMEC-1.2.0/LICENSE` & `atoMEC-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/PKG-INFO` & `atoMEC-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atoMEC
-Version: 1.2.0
+Version: 1.3.0
 Summary: KS-DFT average-atom code
 Home-page: https://github.com/atomec-project/atoMEC
 Author: Tim Callow et al.
 Author-email: t.callow@hzdr.de
 License: BSD 3-Clause License
         
         Copyright (c) 2021 (in alphabetical order), Tim Callow, Attila Cangi, Eli Kraisler
@@ -48,14 +48,15 @@
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5205718.svg)](https://doi.org/10.5281/zenodo.5205718)
 [![docs](https://github.com/atomec-project/atoMEC/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/atomec-project/atoMEC/actions/workflows/gh-pages.yml)
 [![image](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/atoMEC.svg)](https://badge.fury.io/py/atoMEC)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![codecov](https://codecov.io/gh/atomec-project/atoMEC/branch/develop/graph/badge.svg?token=V66CJJ3KPI)](https://codecov.io/gh/atomec-project/atoMEC)
 
 atoMEC is a python-based average-atom code for simulations of high energy density phenomena such as in warm dense matter.
 It is designed as an open-source and modular python package.
 
 atoMEC uses Kohn-Sham density functional theory, in combination with an average-atom approximation,
 to solve the electronic structure problem for single-element materials at finite temperature.
```

### Comparing `atoMEC-1.2.0/README.md` & `atoMEC-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5205718.svg)](https://doi.org/10.5281/zenodo.5205718)
 [![docs](https://github.com/atomec-project/atoMEC/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/atomec-project/atoMEC/actions/workflows/gh-pages.yml)
 [![image](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/atoMEC.svg)](https://badge.fury.io/py/atoMEC)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![codecov](https://codecov.io/gh/atomec-project/atoMEC/branch/develop/graph/badge.svg?token=V66CJJ3KPI)](https://codecov.io/gh/atomec-project/atoMEC)
 
 atoMEC is a python-based average-atom code for simulations of high energy density phenomena such as in warm dense matter.
 It is designed as an open-source and modular python package.
 
 atoMEC uses Kohn-Sham density functional theory, in combination with an average-atom approximation,
 to solve the electronic structure problem for single-element materials at finite temperature.
```

### Comparing `atoMEC-1.2.0/atoMEC/__init__.py` & `atoMEC-1.3.0/atoMEC/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Classes
 -------
 * :class:`Atom` : the main object for atoMEC calculations, containing information \
                   about physical material properties
 """
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
 # standard libraries
 from math import pi
 
 # global imports
 from . import config
 from . import check_inputs
```

### Comparing `atoMEC-1.2.0/atoMEC/check_inputs.py` & `atoMEC-1.3.0/atoMEC/check_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         -------
         density : float
             the mass density
         """
         # radius in cm
         rad_cm = radius / unitconv.cm_to_bohr
         # volume in cm
-        vol_cm = (4.0 * pi * rad_cm ** 3) / 3.0
+        vol_cm = (4.0 * pi * rad_cm**3) / 3.0
         # atomic mass in g
         mass_g = config.mp_g * atom.at_mass
         # density in g cm^-3
         density = mass_g / vol_cm
 
         return density
 
@@ -748,28 +748,29 @@
             density and potential convergence parameters
 
         Returns
         -------
         conv_params : dict of floats
             dictionary of convergence parameters as follows:
             {
-            `econv` (``float``)  : convergence for total energy,
-            `nconv` (``float``)  : convergence for density,
-            `vconv` (``float``)  : convergence for electron number,
-            `eigtol` (``float``) : tolerance for eigenvalues
+            `econv` (``float``)   : convergence for total energy,
+            `nconv` (``float``)   : convergence for density,
+            `vconv` (``float``)   : convergence for electron number,
+            `eigtol` (``float``)  : tolerance for eigenvalues,
+            `bandtol` (``float``) : tolerance for n(l)max warning
             }
 
         Raises
         ------
         InputError.conv_error
             if a convergence parameter is invalid (not float or negative).
         """
         conv_params = {}
         # loop through the convergence parameters
-        for conv in ["econv", "nconv", "vconv", "eigtol"]:
+        for conv in ["econv", "nconv", "vconv", "eigtol", "bandtol"]:
             # assign value if not given
             try:
                 x_conv = input_params[conv]
             except KeyError:
                 x_conv = config.conv_params[conv]
 
             # check float
@@ -1167,7 +1168,31 @@
             + ". Proceeding anyway, but results may be "
             + err2
             + "\n"
             + "Suggested grid range is between 1000-5000 but should be tested wrt"
             " convergence \n"
         )
         return warning
+
+    def norbs_warning(quantum_num):
+        """
+        Warn if either nmax or lmax is too low for convergence.
+
+        Parameters
+        ----------
+        quantum_num : str
+            lmax or nmax
+
+        Returns
+        -------
+        warning : str
+            full error message
+        """
+        warning = (
+            "Warning: "
+            + quantum_num
+            + " appears to be too low. Proceeding anyway, but suggest to increase "
+            + quantum_num
+            + " and restart calculation"
+        )
+
+        return warning
```

### Comparing `atoMEC-1.2.0/atoMEC/config.py` & `atoMEC-1.3.0/atoMEC/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 bc = "dirichlet"  # boundary condition
 unbound = "ideal"  # treatment for unbound electrons
 v_shift = True  # whether to shift the KS potential vertically
 
 # numerical grid for static calculations
 grid_params = {"ngrid": 1000, "x0": -12, "ngrid_coarse": 300}
 # convergence parameters for static calculations
-conv_params = {"econv": 1.0e-5, "nconv": 1.0e-4, "vconv": 1.0e-4, "eigtol": 1.0e-4}
+conv_params = {
+    "econv": 1.0e-5,
+    "nconv": 1.0e-4,
+    "vconv": 1.0e-4,
+    "eigtol": 1.0e-4,
+    "bandtol": 1.0e-3,
+}
 # scf parameters
 scf_params = {"maxscf": 50, "mixfrac": 0.3}
 # band parameters for massacrier band model
 band_params = {"nkpts": 50, "de_min": 1e-3}
 
 # forced bound energy levels (default none)
 force_bound = []
```

### Comparing `atoMEC-1.2.0/atoMEC/convergence.py` & `atoMEC-1.3.0/atoMEC/convergence.py`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/atoMEC/mathtools.py` & `atoMEC-1.3.0/atoMEC/mathtools.py`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/atoMEC/models.py` & `atoMEC-1.3.0/atoMEC/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,16 @@
             }
         conv_params : dict, optional
             dictionary of convergence parameters as follows:
             {
             `econv` (``float``)  : convergence for total energy,
             `nconv` (``float``)  : convergence for density,
             `vconv` (``float``)  : convergence for electron number,
-            `eigtol` (``float``) : convergence for eigenvalues
+            `eigtol` (``float``) : convergence for eigenvalues,
+            `bandtol` (``float``) : tolerance for n(l)max warning
             }
         scf_params : dict, optional
             dictionary for scf cycle parameters as follows:
             {
             `maxscf`  (``int``)   : maximum number of scf cycles,
             `mixfrac` (``float``) : density mixing fraction
             }
@@ -454,14 +455,15 @@
         conv_params={},
         scf_params={},
         band_params={},
         force_bound=[],
         write_info=False,
         verbosity=0,
         dR=0.01,
+        method="A",
     ):
         r"""
         Calculate the electronic pressure using the finite differences method.
 
         N.B.: This is just a wrapper for the postprocess.pressure.finite_diff function.
         It is maintained to support backwards compatibility until next major release.
 
@@ -519,10 +521,11 @@
             energy_output["potential"],
             conv_params,
             scf_params,
             force_bound,
             write_info,
             verbosity,
             dR,
+            method,
         )
 
         return P_e
```

### Comparing `atoMEC-1.2.0/atoMEC/numerov.py` & `atoMEC-1.3.0/atoMEC/numerov.py`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/atoMEC/postprocess/conductivity.py` & `atoMEC-1.3.0/atoMEC/postprocess/conductivity.py`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/atoMEC/postprocess/localization.py` & `atoMEC-1.3.0/atoMEC/postprocess/localization.py`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/atoMEC/postprocess/pressure.py` & `atoMEC-1.3.0/atoMEC/postprocess/pressure.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,37 +2,39 @@
 The pressure module contains functions to compute the pressure with various approaches.
 
 Functions
 ---------
 * :func:`finite_diff` : Calculate electronic pressure with finite-difference method.
 * :func:`stress_tensor` : Calculate electronic pressure with stress-tensor method.
 * :func:`virial` : Calculate electronic pressure with virial method.
+* :func:`ideal_electron` : Calculate electronic pressure with ideal method.
 * :func:`calc_Wd_xc` : Calculate the derivative contribution to virial pressure.
 * :func:`ions_ideal` : Calculate ionic pressure with ideal gas law.
 """
 
 # external libs
 import numpy as np
 
 # internal libs
-from atoMEC import mathtools, xc, config
+from atoMEC import mathtools, xc, config, staticKS
 from atoMEC.check_inputs import InputError
 
 
 def finite_diff(
     atom,
     model,
     orbs,
     pot,
     conv_params={},
     scf_params={},
     force_bound=[],
     write_info=False,
     verbosity=0,
     dR=0.01,
+    method="A",
 ):
     r"""
     Calculate the electronic pressure using the finite differences method.
 
     Parameters
     ----------
     atom : atoMEC.Atom
@@ -65,18 +67,19 @@
         issues.
     verbosity : int, optional
         how much information is printed at each SCF cycle.
         `verbosity=0` prints the total energy and convergence values (default)
         `verbosity=1` prints the above and the KS eigenvalues and occupations.
     write_info : bool, optional
         prints the scf cycle and final parameters
-        defaults to False
     dR : float, optional
         radius difference for finite difference calculation
-        defaults to 0.01
+    method : str, optional
+        method for computing the free energy: can either use normal construction ("A")
+        or with the EnergyAlt class ("B")
 
     Returns
     -------
     P_e : float
         electronic pressure in Ha
     """
     # set up grid and band dictionaries
@@ -112,15 +115,20 @@
         verbosity=verbosity,
         write_info=write_info,
         guess=True,
         guess_pot=pot.v_s,
         write_density=False,
         write_potential=False,
     )
-    F1 = output1["energy"].F_tot
+    if method == "B":
+        F1 = staticKS.EnergyAlt(
+            output1["orbitals"], output1["density"], output1["potential"]
+        ).F_tot
+    elif method == "A":
+        F1 = output1["energy"].F_tot
 
     # change main radius by -dR
     atom.radius = main_rad - dR
 
     # calculate free energy for new radius and store it
     output2 = model.CalcEnergy(
         nmax,
@@ -133,37 +141,46 @@
         verbosity=verbosity,
         write_info=write_info,
         guess=True,
         guess_pot=pot.v_s,
         write_density=False,
         write_potential=False,
     )
-    F2 = output2["energy"].F_tot
+
+    if method == "B":
+        F2 = staticKS.EnergyAlt(
+            output2["orbitals"], output2["density"], output2["potential"]
+        ).F_tot
+    elif method == "A":
+        F2 = output2["energy"].F_tot
 
     dFdR = (F1 - F2) / (2 * dR)  # finite differences
     dRdV = 1 / (4 * np.pi * main_rad**2)  # V = sphere of radius R (main_rad) volume
 
     # calculate pressure by thermodynamic definition p = -dFdV and chain rule
     P_e = -dFdR * dRdV
 
     # convert atom.radius back to its correct value
     atom.radius = main_rad
 
     return P_e
 
 
-def stress_tensor(Atom, model, orbs, pot):
+def stress_tensor(Atom, model, orbs, pot, only_rr=False):
     r"""Calculate the pressure with the stress tensor approach [9]_.
 
     Parameters
     ----------
     orbs : staticKS.Orbitals
         the orbitals object
     pot : staticKS.Potential
         the potential object
+    only_rr : bool, optional
+        whether to use just the radial component of the stress tensor (True)
+        or the full trace (False). See [9]_ for definitions.
 
     Returns
     -------
     P_e : float
         the electronic pressure
 
     References
@@ -190,14 +207,18 @@
 
     # chain rule to convert from dP_dx to dX_dr
     grad_orbs = np.exp(-1.5 * xgrid) * (deriv_orbs - 0.5 * orbs.eigfuncs)
 
     # compute the "gradient" term
     grad_sq = grad_orbs**2
 
+    # add a correction if only rr used
+    if only_rr:
+        grad_sq += 2 * np.exp(-1.5 * xgrid) * orbs.eigfuncs * grad_orbs
+
     # compute the l*(l+1) array
     l_arr = np.fromiter((l * (l + 1.0) for l in range(lmax)), float, lmax)
 
     # get the X(R)^2 term
     orb_sq = orbs.eigfuncs**2 * np.exp(-xgrid)
 
     # compute the l(l+1)/r^2 X(R)^2 term
@@ -207,72 +228,98 @@
     v_E_arr = (
         -pot.v_s[np.newaxis, :, np.newaxis, np.newaxis, :]
         + orbs.eigvals[:, :, :, :, np.newaxis]
     )
     eps_term = 2 * v_E_arr * orb_sq
 
     # sum the orbital based terms
-    sum_terms = grad_sq + lsq_term + eps_term
+    if only_rr:
+        sum_terms = (grad_sq - lsq_term + eps_term) / 2
+    else:
+        sum_terms = (grad_sq + lsq_term + eps_term) / 6
 
     # put everything together
-    P_arr = np.einsum("ijkl,ijklm->m", orbs.occnums_w, sum_terms) / 6
+    P_arr = np.einsum("ijkl,ijklm->m", orbs.occnums_w, sum_terms)
 
     # return the value of P at the sphere edge
     P_e = P_arr[-1]
 
     return P_e
 
 
-def virial(atom, model, energy, density):
+def virial(atom, model, energy, density, orbs, use_correction=False):
     r"""Compute the pressure using the virial theorem (see notes).
 
     Parameters
     ----------
     atom : atoMEC.Atom
         the Atom object
     model : models.ISModel
         the ISModel object
     energy : staticKS.Energy
         the Energy object
     density : staticKS.Density
         the density object
+    use_correction: bool, optional
+        whether to use boundary condition correction described in [10]_
 
     Returns
     -------
     P_e : float
         the electronic pressure
 
     Notes
     -----
-    The virial pressure is given by the formula [10]_
+    The virial pressure is given by the formula [10]_ [12]_
 
     .. math::
 
-        P &= \frac{2T + E_\mathrm{en} + E_\mathrm{Ha} + W_\mathrm{xc}}{3V}\ , \\
+        P &= \frac{K1 + K2 + E_\mathrm{en} + E_\mathrm{Ha} + W_\mathrm{xc}}{3V}\ , \\
         W_\mathrm{xc} &= 3 (W^\mathrm{d}_\mathrm{xc} - E_\mathrm{xc})
 
+    If `use_correction==True`, :math:`K1` and :math:`K2` are respectively the integrated
+    kinetic energy densities "B" and "A" as in :func:`staticKS.Energy.calc_E_kin_dens`.
+
+    If `use_correction==False`, both terms :math:`K1` and :math:`K2` are the same and
+    both given by method "A" in :func:`staticKS.Energy.calc_E_kin_dens`.
+
     References
     ----------
     .. [10] P. Legrand and F. Perrot, Virial theorem and pressure calculations in the
         GGA, J. Phys.: Condens. Matter 13 (2001) 287–301
         `DOI:10.1088/0953-8984/13/2/306
         <https://doi.org/10.1088/0953-8984/13/2/306>`__.
+    .. [12] J. C. Pain, A model of dense-plasma atomic structure for equation-of-state
+        calculations, J. Phys. B: At. Mol. Opt. Phys. 40 (2007) 1553-1573
+        `DOI:10.1088/0953-4075/40/8/008
+        <https://doi.org/10.1088/0953-4075/40/8/008>`__.
     """
     # compute the sphere volume
     sph_vol = (4.0 * np.pi / 3.0) * atom.radius**3
 
     # compute the derivative term of the W_xc component
     Wd_x = calc_Wd_xc(model.xfunc_id, density)
     Wd_c = calc_Wd_xc(model.cfunc_id, density)
 
     # compute total W_xc component
     W_xc = -3 * energy.E_xc["xc"] + 3 * (Wd_x + Wd_c)
 
+    K2 = energy.E_kin["tot"]
+
+    if not use_correction:
+        K1 = energy.E_kin["tot"]
+    else:
+        E_kin_alt_dens = staticKS.Energy.calc_E_kin_dens(
+            orbs.eigfuncs, orbs.occnums_w, orbs._xgrid, method="B"
+        )
+        # integrate over sphere
+        K1 = mathtools.int_sphere(np.sum(E_kin_alt_dens, axis=0), orbs._xgrid)
+
     # compute E_V = 2*T + U + W_xc
-    E_V = 2 * energy.E_kin["tot"] + energy.E_en + energy.E_ha + W_xc
+    E_V = K1 + K2 + energy.E_en + energy.E_ha + W_xc
 
     # compute the virial pressure
     P_e = E_V / (3 * sph_vol)
 
     return P_e
 
 
@@ -319,14 +366,47 @@
     Wd_xc = 0.0
     for sp in range(spindims):
         Wd_xc += mathtools.int_sphere(density.total[sp] * v_xc[sp], density._xgrid)
 
     return Wd_xc
 
 
+def ideal_electron(Atom, chem_pot):
+    r"""
+    Compute the ideal electron pressure.
+
+    Parameters
+    ----------
+    Atom : atoMEC.Atom
+        the atom object
+    chem_pot : float
+        the chemical potential
+
+    Returns
+    -------
+    P_e : float
+        the ideal electron pressure
+
+    Notes
+    -----
+    The formula to determine the ideal electron pressure is
+
+    .. math::
+
+        P_\textrm{e} = \frac{2^{3/2}}{3\pi^2} \int\mathrm{d}\epsilon
+        \epsilon^{3/2} f_\textrm{FD}(\epsilon,\beta,\mu)
+    """
+    beta = 1.0 / Atom.temp
+    prefac = 2**1.5 / (3 * np.pi**2)
+    fd_int = mathtools.fd_int_complete(chem_pot, beta, 3)
+    P_e = prefac * fd_int
+
+    return P_e
+
+
 def ions_ideal(atom):
     r"""Compute the the ideal gas pressure for the ions.
 
     In atomic units, the ideal gas pressure is simply P = T/V.
 
     Parameters
     ----------
```

### Comparing `atoMEC-1.2.0/atoMEC/staticKS.py` & `atoMEC-1.3.0/atoMEC/staticKS.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from math import sqrt, pi, exp
 
 # internal modules
 from . import config
 from . import numerov
 from . import mathtools
 from . import xc
+from . import check_inputs
 
 # from . import writeoutput
 
 
 # the logarithmic grid
 def log_grid(x_r):
     """
@@ -131,14 +132,22 @@
             raise Exception("Band weightings have not been initialized")
         return self._kpt_int_weight
 
     @property
     def occnums_w(self):
         r"""ndarray: Weighted KS occupation numbers."""
         self._occnums_w = self.occnums * self.occ_weight
+        # check if more bands are needed
+        norbs_ok, lorbs_ok = self.check_orbs(
+            self._occnums_w, config.conv_params["bandtol"]
+        )
+        if not norbs_ok:
+            print(check_inputs.InputWarning.norbs_warning("nmax"))
+        if not lorbs_ok:
+            print(check_inputs.InputWarning.norbs_warning("lmax"))
         return self._occnums_w
 
     @property
     def occnums(self):
         r"""ndarray: Bare KS occupation numbers (Fermi-Dirac)."""
         if np.all(self._occnums == 0.0):
             raise Exception("Occupation numbers have not been initialized")
@@ -460,15 +469,15 @@
             np.sqrt(np.abs(hub_func)),
             1.0,
         )
 
         # compute the pre-factor when the energy gap is large enough for a band
         prefac = np.where(
             eig_diff > config.band_params["de_min"],
-            2.0 / (pi * delta ** 2.0),
+            2.0 / (pi * delta**2.0),
             1.0,
         )
 
         # compute the dos
         dos = prefac * f_sqrt
 
         return dos
@@ -523,15 +532,15 @@
 
                 # take the sqrt when the energy gap is big enough to justify a band
                 f_sqrt = np.where(hub_func > 0, np.sqrt(np.abs(hub_func)), 0.0)
 
                 # compute the pre-factor when the energy gap is large enough for a band
                 prefac = np.where(
                     e_gap_arr > config.band_params["de_min"],
-                    2.0 / (pi * delta ** 2.0),
+                    2.0 / (pi * delta**2.0),
                     0.0,
                 )
 
                 # compute the dos
                 dos_knl[i, sp] = prefac[sp] * f_sqrt[sp]
 
                 # compute the Fermi-Dirac distribution
@@ -593,14 +602,48 @@
                 )
                 e_tot_arr = np.concatenate((e_tot_arr, e_pt_arr))
 
         # sort the array
         e_tot_arr = np.sort(e_tot_arr)
         return e_tot_arr
 
+    @staticmethod
+    def check_orbs(occnums_w, threshold):
+        r"""Check the values of nmax and lmax are sufficient.
+
+        Finds the values of the occupations of the final orbitals in lmax
+        and nmax directions. If either is above the threshold, returns False
+        (which triggers a warning elsewhere).
+
+        Parameters
+        ----------
+        occnums_w : np.ndarray
+            weighted orbital occupations
+        threshold : float
+            the threshold occupation number at which to trigger a warning
+
+        Returns
+        -------
+        norbs_ok, lorbs_ok : tuple of bools
+            whether the values of nmax and lmax are sufficient
+
+        """
+        lorbs_ok = True
+        norbs_ok = True
+        # sum over the first two dimensions (spin and kpts)
+        occs_sum = np.sum(occnums_w, axis=(0, 1))
+        # check the l dimension
+        occs_l = occs_sum[:, -1]
+        if max(occs_l) > threshold:
+            lorbs_ok = False
+        occs_n = occs_sum[-1, :]
+        if max(occs_n) > threshold:
+            norbs_ok = False
+        return lorbs_ok, norbs_ok
+
 
 class Density:
     """
     Class holding the static KS density and routines required to compute its components.
 
     Parameters
     ----------
@@ -689,15 +732,15 @@
 
         # first of all construct the density
         # rho_b(r) = \sum_{n,l} (2l+1) f_{nl} |R_{nl}(r)|^2
         # occnums in atoMEC are defined as (2l+1)*f_{nl}
 
         # R_{nl}(r) = exp(x/2) P_{nl}(x), P(x) are eigfuncs
         orbs_R = np.exp(-xgrid / 2.0) * eigfuncs
-        orbs_R_sq = orbs_R ** 2.0
+        orbs_R_sq = orbs_R**2.0
 
         # sum over the (l,n) dimensions of the orbitals to get the density
         dens["rho"] = np.einsum("ijkl,ijklm->jm", occnums, orbs_R_sq)
 
         # compute the number of unbound electrons
         dens["N"] = np.sum(occnums, axis=(0, 2, 3))
 
@@ -725,15 +768,15 @@
         N_unbound = np.zeros((config.spindims))
 
         # so far only the ideal approximation is implemented
         if config.unbound == "ideal":
 
             # unbound density is constant
             for i in range(config.spindims):
-                prefac = (2.0 / config.spindims) * 1.0 / (sqrt(2) * pi ** 2)
+                prefac = (2.0 / config.spindims) * 1.0 / (sqrt(2) * pi**2)
                 n_ub = prefac * mathtools.fd_int_complete(
                     config.mu[i], config.beta, 1.0
                 )
                 rho_unbound[i] = n_ub
                 N_unbound[i] = n_ub * config.sph_vol
 
             unbound = {"rho": rho_unbound, "N": N_unbound}
@@ -1040,30 +1083,34 @@
             the local kinetic energy density
 
         Notes
         -----
         The methods 'A' and 'B' in this function are given according to the definitions
         in [3]_ and [4]_.
 
-        They of course (should) both integrate to the same kinetic energy. The
-        definition 'B' is the one used in the usual definition of the electron
-        localization function [5]_.
+        Both methods should integrate to the same kinetic energy, in the case of Neumann
+        or Diriclet boundary conditions; for the bands condition they will be different.
+        The definition 'B' is the one used in the usual definition of the electron
+        localization function [5]_. It is given by formula (B.8) in [11]_.
 
         References
         ----------
         .. [3] H. Jiang, The local kinetic energy density revisited,
            New J. Phys. 22 103050 (2020), `DOI:10.1088/1367-2630/abbf5d
            <https://doi.org/10.1088/1367-2630/abbf5d>`__.
         .. [4] L. Cohen, Local kinetic energy in quantum mechanics,
            J. Chem. Phys. 70, 788 (1979), `DOI:10.1063/1.437511
            <https://doi.org/10.1063/1.437511>`__.
         .. [5] A. Savin et al., Electron Localization in Solid-State Structures of the
            Elements: the Diamond Structure, Angew. Chem. Int. Ed. Engl. 31: 187-188
            (1992), `DOI:10.1002/anie.199201871
            <https://doi.org/10.1002/anie.199201871>`__.
+        .. [11] J. Pain, A model of dense-plasma atomic structure for equation-of-state
+           calculations. J. Phys. B, 40(8):1553 (2007), `DOI:10.1088/0953-4075/40/8/008
+           <https://dx.doi.org/10.1088/0953-4075/40/8/008>`__.
         """
         if method == "A":
             # compute the grad^2 component
             grad2_orbs = mathtools.laplace(eigfuncs, xgrid)
 
             # compute the (l+1/2)^2 component
             l_arr = np.fromiter(
@@ -1081,27 +1128,31 @@
         elif method == "B":
 
             # compute the gradient of the orbitals
             grad_eigfuncs = np.gradient(eigfuncs, xgrid, axis=-1, edge_order=2)
 
             # compute the (l+1/2) component
             l_arr = np.fromiter(
-                ((2 * l + 1.0) for l in range(config.lmax)), float, config.lmax
+                (l * (l + 1.0) for l in range(config.lmax)), float, config.lmax
+            )
+            eigs_mod = eigfuncs * np.exp(-xgrid / 2)
+            lhalf_orbs = np.einsum("k,ijklm->ijklm", l_arr, eigs_mod**2) / np.exp(
+                2 * xgrid
             )
-            lhalf_orbs = np.einsum("k,ijklm->ijklm", l_arr, eigfuncs)
 
             # chain rule to convert from dP_dx to dX_dr
-            grad_orbs = np.exp(-1.5 * xgrid) * (grad_eigfuncs - 0.5 * lhalf_orbs)
+            grad_orbs = np.exp(-1.5 * xgrid) * (grad_eigfuncs - 0.5 * eigfuncs)
 
             # square it
-            # grad_orbs_sq = np.einsum("k,ijklm->ijklm", l_arr, grad_orbs ** 2.0)
-            grad_orbs_sq = grad_orbs ** 2.0
+            grad_orbs_sq = grad_orbs**2.0
 
             # multiply and sum over occupation numbers
-            e_kin_dens = 0.5 * np.einsum("ijkl,ijklm->jm", occnums, grad_orbs_sq)
+            e_kin_dens = 0.5 * np.einsum(
+                "ijkl,ijklm->jm", occnums, grad_orbs_sq + lhalf_orbs
+            )
 
         return e_kin_dens
 
     @staticmethod
     def calc_E_kin_unbound():
         r"""
         Compute the contribution from unbound (continuum) electrons to kinetic energy.
@@ -1128,15 +1179,15 @@
 
         where :math:`I_{3/2}(\mu,\beta)` denotes the complete Fermi-Diract integral
         """
         # currently only ideal treatment supported
         if config.unbound == "ideal":
             E_kin_unbound = 0.0  # initialize
             for i in range(config.spindims):
-                prefac = (2.0 / config.spindims) * config.sph_vol / (sqrt(2) * pi ** 2)
+                prefac = (2.0 / config.spindims) * config.sph_vol / (sqrt(2) * pi**2)
                 E_kin_unbound += prefac * mathtools.fd_int_complete(
                     config.mu[i], config.beta, 3.0
                 )
 
         return E_kin_unbound
 
     def calc_entropy(self, orbs):
@@ -1194,16 +1245,16 @@
         The entropy of non-interacting (KS) electrons is given by:
 
         .. math::
             S_\mathrm{b} = -\sum_{s,l,n} g_{ln} (2l+1) [ f_{nls} \log(f_{nls}) \
                            + (1-f_{nls}) (\log(1-f_{nls}) ]
         """
         # replace zeros in occupation numbers with finite numbers (for taking log)
-        occnums_mod1 = np.where(occnums > 1e-5, occnums, 0.5)
-        occnums_mod2 = np.where(occnums < 1.0 - 1e-5, occnums, 0.5)
+        occnums_mod1 = np.where(occnums > 1e-20, occnums, 1)
+        occnums_mod2 = np.where(occnums < 1.0 - 1e-20, occnums, 0)
 
         # now compute the terms in the square bracket
         term1 = occnums * np.log(occnums_mod1)
         term2 = (1.0 - occnums) * np.log(1.0 - occnums_mod2)
 
         # multiply by degeneracy (dos * (2l+1))
         g_nls = degen * (term1 + term2)
@@ -1240,15 +1291,15 @@
         """
         # currently only ideal treatment supported
         if config.unbound == "ideal":
             S_unbound = 0.0  # initialize
             for i in range(config.spindims):
                 if config.nele[i] > 1e-5:
                     prefac = (
-                        (2.0 / config.spindims) * config.sph_vol / (sqrt(2) * pi ** 2)
+                        (2.0 / config.spindims) * config.sph_vol / (sqrt(2) * pi**2)
                     )
 
                     S_unbound -= prefac * mathtools.ideal_entropy_int(
                         config.mu[i], config.beta, 1.0
                     )
                 else:
                     S_unbound += 0.0
@@ -1343,16 +1394,18 @@
         self._dens = dens.total
         self._xgrid = dens._xgrid
         self._pot = pot
 
         # initialize attributes
         self._F_tot = 0.0
         self._E_tot = 0.0
+        self._E_kin = {"tot": 0.0, "bound": 0.0, "unbound": 0.0}
         self._entropy = {"tot": 0.0, "bound": 0.0, "unbound": 0.0}
         self._E_eps = 0.0
+        self._E_en = 0.0
         self._E_unbound = 0.0
         self._E_v_hxc = 0.0
         self._E_ha = 0.0
         self._E_xc = {"xc": 0.0, "x": 0.0, "c": 0.0}
 
     @property
     def F_tot(self):
@@ -1387,14 +1440,29 @@
         Given by :math:`E=\sum_{nl\sigma} (2l+1) f_{nl}^\sigma \epsilon_{nl}^\sigma`
         """
         if self._E_eps == 0.0:
             self._E_eps = np.sum(self._orbs.occnums_w * self._orbs.eigvals)
         return self._E_eps
 
     @property
+    def E_en(self):
+        r"""float: Electron-nuclear attraction energy."""
+        if self._E_en == 0.0:
+            self._E_en = Energy.calc_E_en(self._dens, self._xgrid)
+        return self._E_en
+
+    @property
+    def E_kin(self):
+        r"""Dict of floats: Kinetic energy components."""
+        if self._E_kin["tot"] == 0.0:
+            self._E_kin["bound"] = self.E_eps - self.E_v_hxc - self.E_en
+            self._E_kin["tot"] = self._E_kin["bound"] + self._E_kin["unbound"]
+        return self._E_kin
+
+    @property
     def E_unbound(self):
         r"""float: The energy of the unbound part of the electron density."""
         if self._E_unbound == 0.0 and config.unbound == "ideal":
             self._E_unbound = Energy.calc_E_kin_unbound()
         return self._E_unbound
 
     @property
```

### Comparing `atoMEC-1.2.0/atoMEC/writeoutput.py` & `atoMEC-1.3.0/atoMEC/writeoutput.py`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/atoMEC/xc.py` & `atoMEC-1.3.0/atoMEC/xc.py`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/atoMEC.egg-info/PKG-INFO` & `atoMEC-1.3.0/atoMEC.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atoMEC
-Version: 1.2.0
+Version: 1.3.0
 Summary: KS-DFT average-atom code
 Home-page: https://github.com/atomec-project/atoMEC
 Author: Tim Callow et al.
 Author-email: t.callow@hzdr.de
 License: BSD 3-Clause License
         
         Copyright (c) 2021 (in alphabetical order), Tim Callow, Attila Cangi, Eli Kraisler
@@ -48,14 +48,15 @@
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5205718.svg)](https://doi.org/10.5281/zenodo.5205718)
 [![docs](https://github.com/atomec-project/atoMEC/actions/workflows/gh-pages.yml/badge.svg)](https://github.com/atomec-project/atoMEC/actions/workflows/gh-pages.yml)
 [![image](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/atoMEC.svg)](https://badge.fury.io/py/atoMEC)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
+[![codecov](https://codecov.io/gh/atomec-project/atoMEC/branch/develop/graph/badge.svg?token=V66CJJ3KPI)](https://codecov.io/gh/atomec-project/atoMEC)
 
 atoMEC is a python-based average-atom code for simulations of high energy density phenomena such as in warm dense matter.
 It is designed as an open-source and modular python package.
 
 atoMEC uses Kohn-Sham density functional theory, in combination with an average-atom approximation,
 to solve the electronic structure problem for single-element materials at finite temperature.
```

### Comparing `atoMEC-1.2.0/atoMEC.egg-info/SOURCES.txt` & `atoMEC-1.3.0/atoMEC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atoMEC-1.2.0/setup.py` & `atoMEC-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'dev': ['bump2version'],
     'docs': open('docs/requirements.txt').read().splitlines(),
     'tests': open('tests/requirements.txt').read().splitlines(),
 }
 
 setup(
     name="atoMEC",
-    version="1.2.0",
+    version="1.3.0",
     description="KS-DFT average-atom code",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Tim Callow et al.",
     author_email="t.callow@hzdr.de",
     url="https://github.com/atomec-project/atoMEC",
     license=license,
```

