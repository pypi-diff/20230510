# Comparing `tmp/ligo-raven-3.1.dev0.tar.gz` & `tmp/ligo-raven-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-raven-3.1.dev0.tar", last modified: Fri Mar 24 20:26:25 2023, max compression
+gzip compressed data, was "ligo-raven-3.2.tar", last modified: Tue May  9 22:25:23 2023, max compression
```

## Comparing `ligo-raven-3.1.dev0.tar` & `ligo-raven-3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.135446 ligo-raven-3.1.dev0/
--rw-r--r--   0 naresh     (505) staff       (20)    35147 2023-03-06 14:54:32.000000 ligo-raven-3.1.dev0/COPYING
--rw-r--r--   0 naresh     (505) staff       (20)      113 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/MANIFEST.in
--rw-r--r--   0 naresh     (505) staff       (20)      671 2023-03-24 20:26:25.135635 ligo-raven-3.1.dev0/PKG-INFO
--rw-r--r--   0 naresh     (505) staff       (20)     1331 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/README.md
-drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.125741 ligo-raven-3.1.dev0/bin/
--rw-r--r--   0 naresh     (505) staff       (20)     6013 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/bin/raven_calc_signif_gracedb
--rw-r--r--   0 naresh     (505) staff       (20)     5980 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/bin/raven_coinc_far
--rw-r--r--   0 naresh     (505) staff       (20)     3721 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/bin/raven_query
--rw-r--r--   0 naresh     (505) staff       (20)     3600 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/bin/raven_search
--rw-r--r--   0 naresh     (505) staff       (20)     4018 2023-03-06 14:54:32.000000 ligo-raven-3.1.dev0/bin/raven_skymap_overlap
-drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.126322 ligo-raven-3.1.dev0/ligo/
--rw-r--r--   0 naresh     (505) staff       (20)       56 2023-03-06 14:54:32.000000 ligo-raven-3.1.dev0/ligo/__init__.py
-drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.127725 ligo-raven-3.1.dev0/ligo/raven/
--rw-r--r--   0 naresh     (505) staff       (20)        0 2023-03-06 14:54:32.000000 ligo-raven-3.1.dev0/ligo/raven/__init__.py
--rw-r--r--   0 naresh     (505) staff       (20)     9718 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/ligo/raven/gracedb_events.py
--rw-r--r--   0 naresh     (505) staff       (20)    27451 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/ligo/raven/search.py
-drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.134263 ligo-raven-3.1.dev0/ligo/raven/tests/
--rw-r--r--   0 naresh     (505) staff       (20)     9571 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/FAR_study.py
--rw-r--r--   0 naresh     (505) staff       (20)     9745 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/FAR_subgrb_study.py
--rw-r--r--   0 naresh     (505) staff       (20)        0 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/__init__.py
--rw-r--r--   0 naresh     (505) staff       (20)     7403 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/mock_gracedb_rest.py
--rw-r--r--   0 naresh     (505) staff       (20)     7530 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/mock_gracedb_sdk.py
--rw-r--r--   0 naresh     (505) staff       (20)     9995 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/test_overlap_integral.py
--rw-r--r--   0 naresh     (505) staff       (20)    30184 2023-03-24 20:19:19.000000 ligo-raven-3.1.dev0/ligo/raven/tests/test_raven_search.py
--rw-r--r--   0 naresh     (505) staff       (20)     7811 2023-03-06 14:56:49.000000 ligo-raven-3.1.dev0/ligo/raven/tests/test_search_window.py
-drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-03-24 20:26:25.135088 ligo-raven-3.1.dev0/ligo_raven.egg-info/
--rw-r--r--   0 naresh     (505) staff       (20)      536 2023-03-24 20:26:25.000000 ligo-raven-3.1.dev0/ligo_raven.egg-info/SOURCES.txt
--rw-r--r--   0 naresh     (505) staff       (20)      254 2023-03-24 20:26:25.136417 ligo-raven-3.1.dev0/setup.cfg
--rwxr-xr-x   0 naresh     (505) staff       (20)     2220 2023-03-24 20:22:37.000000 ligo-raven-3.1.dev0/setup.py
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-05-09 22:25:23.717754 ligo-raven-3.2/
+-rw-r--r--   0 naresh     (505) staff       (20)    35147 2023-03-06 14:54:32.000000 ligo-raven-3.2/COPYING
+-rw-r--r--   0 naresh     (505) staff       (20)      113 2023-03-06 14:56:49.000000 ligo-raven-3.2/MANIFEST.in
+-rw-r--r--   0 naresh     (505) staff       (20)      638 2023-05-09 22:25:23.717931 ligo-raven-3.2/PKG-INFO
+-rw-r--r--   0 naresh     (505) staff       (20)     1331 2023-03-06 14:56:49.000000 ligo-raven-3.2/README.md
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-05-09 22:25:23.706313 ligo-raven-3.2/bin/
+-rw-r--r--   0 naresh     (505) staff       (20)     6013 2023-03-24 20:19:19.000000 ligo-raven-3.2/bin/raven_calc_signif_gracedb
+-rw-r--r--   0 naresh     (505) staff       (20)     5980 2023-03-24 20:19:19.000000 ligo-raven-3.2/bin/raven_coinc_far
+-rw-r--r--   0 naresh     (505) staff       (20)     3721 2023-03-06 14:56:49.000000 ligo-raven-3.2/bin/raven_query
+-rw-r--r--   0 naresh     (505) staff       (20)     3600 2023-03-06 14:56:49.000000 ligo-raven-3.2/bin/raven_search
+-rw-r--r--   0 naresh     (505) staff       (20)     4018 2023-03-06 14:54:32.000000 ligo-raven-3.2/bin/raven_skymap_overlap
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-05-09 22:25:23.707148 ligo-raven-3.2/ligo/
+-rw-r--r--   0 naresh     (505) staff       (20)       56 2023-03-06 14:54:32.000000 ligo-raven-3.2/ligo/__init__.py
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-05-09 22:25:23.708695 ligo-raven-3.2/ligo/raven/
+-rw-r--r--   0 naresh     (505) staff       (20)        0 2023-03-06 14:54:32.000000 ligo-raven-3.2/ligo/raven/__init__.py
+-rw-r--r--   0 naresh     (505) staff       (20)     9718 2023-03-24 20:19:19.000000 ligo-raven-3.2/ligo/raven/gracedb_events.py
+-rw-r--r--   0 naresh     (505) staff       (20)    27219 2023-05-09 22:05:59.000000 ligo-raven-3.2/ligo/raven/search.py
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-05-09 22:25:23.716667 ligo-raven-3.2/ligo/raven/tests/
+-rw-r--r--   0 naresh     (505) staff       (20)     9571 2023-03-06 14:56:49.000000 ligo-raven-3.2/ligo/raven/tests/FAR_study.py
+-rw-r--r--   0 naresh     (505) staff       (20)     9745 2023-03-06 14:56:49.000000 ligo-raven-3.2/ligo/raven/tests/FAR_subgrb_study.py
+-rw-r--r--   0 naresh     (505) staff       (20)        0 2023-03-06 14:56:49.000000 ligo-raven-3.2/ligo/raven/tests/__init__.py
+-rw-r--r--   0 naresh     (505) staff       (20)     7400 2023-05-09 22:05:59.000000 ligo-raven-3.2/ligo/raven/tests/mock_gracedb_rest.py
+-rw-r--r--   0 naresh     (505) staff       (20)     7527 2023-05-09 22:05:59.000000 ligo-raven-3.2/ligo/raven/tests/mock_gracedb_sdk.py
+-rw-r--r--   0 naresh     (505) staff       (20)     9995 2023-03-06 14:56:49.000000 ligo-raven-3.2/ligo/raven/tests/test_overlap_integral.py
+-rw-r--r--   0 naresh     (505) staff       (20)    30167 2023-05-09 22:05:59.000000 ligo-raven-3.2/ligo/raven/tests/test_raven_search.py
+-rw-r--r--   0 naresh     (505) staff       (20)     7811 2023-03-06 14:56:49.000000 ligo-raven-3.2/ligo/raven/tests/test_search_window.py
+drwxr-xr-x   0 naresh     (505) staff       (20)        0 2023-05-09 22:25:23.717345 ligo-raven-3.2/ligo_raven.egg-info/
+-rw-r--r--   0 naresh     (505) staff       (20)      536 2023-05-09 22:25:23.000000 ligo-raven-3.2/ligo_raven.egg-info/SOURCES.txt
+-rw-r--r--   0 naresh     (505) staff       (20)      254 2023-05-09 22:25:23.718672 ligo-raven-3.2/setup.cfg
+-rwxr-xr-x   0 naresh     (505) staff       (20)     2241 2023-05-09 22:24:45.000000 ligo-raven-3.2/setup.py
```

### Comparing `ligo-raven-3.1.dev0/COPYING` & `ligo-raven-3.2/COPYING`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/README.md` & `ligo-raven-3.2/README.md`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/bin/raven_calc_signif_gracedb` & `ligo-raven-3.2/bin/raven_calc_signif_gracedb`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/bin/raven_coinc_far` & `ligo-raven-3.2/bin/raven_coinc_far`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/bin/raven_query` & `ligo-raven-3.2/bin/raven_query`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/bin/raven_search` & `ligo-raven-3.2/bin/raven_search`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/bin/raven_skymap_overlap` & `ligo-raven-3.2/bin/raven_skymap_overlap`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/ligo/raven/gracedb_events.py` & `ligo-raven-3.2/ligo/raven/gracedb_events.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/ligo/raven/search.py` & `ligo-raven-3.2/ligo/raven/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 __author__ = "Alex Urban <alexander.urban@ligo.org>"
 
 
 # Imports.
 import json
 import re
 import sys
-import warnings
 
 from astropy import units as u
 from astropy.coordinates import SkyCoord
 import astropy_healpix as ah
 import healpy as hp
 import numpy as np
 
@@ -310,17 +309,17 @@
     se_order = 'nested' if se_nested or any(se_skymap_uniq) else 'ring'
     ext_order = 'nested' if ext_nested or any(ext_skymap_uniq) else 'ring'
 
     # Enforce the sky maps to be non-negative
     se_skymap = np.abs(se_skymap)
     exttrig_skymap = np.abs(exttrig_skymap)
 
-    if not any(exttrig_skymap) and not (ra and dec):
+    if not any(exttrig_skymap) and not (ra is not None and dec is not None):
         # Raise error if external info not given
-        raise AssertionError('Provide external sky map or ra/dec')
+        raise ValueError("Please provide external sky map or ra/dec")
 
     # Use multi-ordered GW sky map
     if any(se_skymap_uniq):
         # gw_skymap is the probability density instead of probability
         # convert GW sky map uniq to ra and dec
         level, ipix = ah.uniq_to_level_ipix(se_skymap_uniq)
         nsides = ah.level_to_nside(level)
@@ -341,61 +340,55 @@
                                      order=ext_order)
             # Find closest external pixels to gw pixels
             c = SkyCoord(ra=ra_gw, dec=dec_gw)
             catalog = SkyCoord(ra=ra_ext, dec=dec_ext)
             ext_ind, d2d, d3d = c.match_to_catalog_sky(catalog)
             ext_norm = np.sum(exttrig_skymap * ah.nside_to_pixel_area(nsides))
 
-            skymap_overlap_integral = \
-                np.sum(se_skymap * areas *
-                       exttrig_skymap[ext_ind] /
-                       sky_prior / se_norm / ext_norm).to(1).value
+            return np.sum(se_skymap * areas * exttrig_skymap[ext_ind] /
+                          sky_prior / se_norm / ext_norm).to(1).value
 
-        elif ra and dec:
+        elif ra is not None and dec is not None:
             # Use multi-ordered gw sky map and one external point
             # Relevant for very well localized experiments
             # such as Swift
             c = SkyCoord(ra=ra*u.degree, dec=dec*u.degree)
             catalog = SkyCoord(ra=ra_gw, dec=dec_gw)
             ind, d2d, d3d = c.match_to_catalog_sky(catalog)
 
-            skymap_overlap_integral = \
-                (se_skymap[ind] / u.sr / sky_prior / se_norm).to(1).value
+            return (se_skymap[ind] / u.sr / sky_prior / se_norm).to(1).value
 
         elif any(exttrig_skymap):
             # Use multi-ordered gw sky map and flat external sky map
             # Find matching external sky map indices using GW ra/dec
             ext_nside = ah.npix_to_nside(len(exttrig_skymap))
             ext_ind = \
                 ah.lonlat_to_healpix(ra_gw, dec_gw, ext_nside,
                                      order=ext_order)
 
             ext_norm = np.sum(exttrig_skymap)
 
-            skymap_overlap_integral = \
-                np.sum(se_skymap * areas *
-                       exttrig_skymap[ext_ind] /
-                       ah.nside_to_pixel_area(ext_nside) /
-                       sky_prior / se_norm / ext_norm).to(1).value
+            return np.sum(se_skymap * areas * exttrig_skymap[ext_ind] /
+                          ah.nside_to_pixel_area(ext_nside) /
+                          sky_prior / se_norm / ext_norm).to(1).value
 
     # Use flat GW sky map
     else:
-        if ra and dec:
+        if ra is not None and dec is not None:
             # Use flat gw sky and one external point
             se_nside = ah.npix_to_nside(len(se_skymap))
             ind = ah.lonlat_to_healpix(ra * u.deg, dec * u.deg, se_nside,
                                        order=se_order)
             se_norm = sum(se_skymap)
-            skymap_overlap_integral = se_skymap[ind] * len(se_skymap) / se_norm
+            return se_skymap[ind] * len(se_skymap) / se_norm
 
         elif any(exttrig_skymap):
             if se_nested != ext_nested:
-                warnings.warn('Sky maps not both using the same ordering '
-                              '(nested or ring). Result is likely '
-                              'incorrect.')
+                raise ValueError("Sky maps must both use nested or ring"
+                                 "ordering")
             # Use two flat sky maps
             nside_s = hp.npix2nside(len(se_skymap))
             nside_e = hp.npix2nside(len(exttrig_skymap))
             if nside_s > nside_e:
                 exttrig_skymap = hp.ud_grade(exttrig_skymap,
                                              nside_out=nside_s,
                                              order_in=('NESTED' if ext_nested
@@ -404,24 +397,21 @@
                 se_skymap = hp.ud_grade(se_skymap,
                                         nside_out=nside_e,
                                         order_in=('NESTED' if se_nested
                                                   else 'RING'))
             se_norm = se_skymap.sum()
             exttrig_norm = exttrig_skymap.sum()
             if se_norm > 0 and exttrig_norm > 0:
-                skymap_overlap_integral = (
-                    np.dot(se_skymap, exttrig_skymap)
-                    / se_norm / exttrig_norm
-                    * len(se_skymap))
+                return (np.dot(se_skymap, exttrig_skymap) / se_norm /
+                        exttrig_norm * len(se_skymap))
             else:
-                message = ("RAVEN: ERROR: At least one sky map has a "
-                           "probability density that sums to zero or less.")
-                return message
+                return ("RAVEN: ERROR: At least one sky map has a "
+                        "probability density that sums to zero or less.")
 
-    return skymap_overlap_integral
+    raise ValueError("Please provide both GW and external sky map info")
 
 
 def coinc_far(se_id, ext_id, tl, th, grb_search='GRB', se_fitsfile=None,
               ext_fitsfile=None, incl_sky=False,
               gracedb=None, far_grb=None, em_rate=None,
               far_gw_thresh=None, far_grb_thresh=None,
               se_dict=None, ext_dict=None,
```

### Comparing `ligo-raven-3.1.dev0/ligo/raven/tests/FAR_study.py` & `ligo-raven-3.2/ligo/raven/tests/FAR_study.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/ligo/raven/tests/FAR_subgrb_study.py` & `ligo-raven-3.2/ligo/raven/tests/FAR_subgrb_study.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/ligo/raven/tests/mock_gracedb_rest.py` & `ligo-raven-3.2/ligo/raven/tests/mock_gracedb_rest.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,20 +73,20 @@
                     "group": "External",
                     "pipeline": "Swift",
                     "search": "SubGRB",
                     "extra_attributes": {
                         "GRB": {
                             "ra": 20.,
                             "dec": 30.}}}
-        if self.graceid=='E5':
-            return {"graceid": "E5",
+        if self.graceid=='M5':
+            return {"graceid": "M5",
                     "gpstime": 104.0,
                     "group": "External",
                     "pipeline": "Fermi",
-                    "search": "SubGRB"}
+                    "search": "MDC"}
     class logs(object):
         @mock.create_autospec
         def create(*args, **kwargs):
             print("Sent log message")
             return
     class files(object):
         def __getitem__(self, file):
```

### Comparing `ligo-raven-3.1.dev0/ligo/raven/tests/mock_gracedb_sdk.py` & `ligo-raven-3.2/ligo/raven/tests/mock_gracedb_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,20 @@
                     "group": "External",
                     "pipeline": "Swift",
                     "search": "SubGRB",
                     "extra_attributes": {
                         "GRB": {
                             "ra": 20.,
                             "dec": 30.}}}
-        if self.graceid=='E5':
-            return {"graceid": "E5",
+        if self.graceid=='M5':
+            return {"graceid": "M5",
                     "gpstime": 104.0,
                     "group": "External",
                     "pipeline": "Fermi",
-                    "search": "SubGRB"}
+                    "search": "MDC"}
     class logs(object):
         @mock.create_autospec
         def create(*args, **kwargs):
             print("Sent log message")
             return
     class files(object):
         def __getitem__(self, file):
```

### Comparing `ligo-raven-3.1.dev0/ligo/raven/tests/test_overlap_integral.py` & `ligo-raven-3.2/ligo/raven/tests/test_overlap_integral.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/ligo/raven/tests/test_raven_search.py` & `ligo-raven-3.2/ligo/raven/tests/test_raven_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,26 +129,26 @@
     [['E100','Superevent', 100, -5, 1, None, [], [], [], mock_gracedb_rest],
      ['E101','Superevent', 100, -600, 60, 'Burst', [], [], [], mock_gracedb_rest],
      ['E102','Superevent', 100, -5, 1, 'CBC', [], [], [], mock_gracedb_rest],
      ['S100','External', 100, -1, 5, None, ['Fermi','Swift'], [], [], mock_gracedb_rest],
      ['S100','External', 100, -1, 5, None, ['Fermi','Swift'], ['SubGRB'], [], mock_gracedb_rest],
      ['S101','External', 100, -10, 10, None, ['SNEWS'], [], [], mock_gracedb_rest],
      ['S102','External', 100, -1, 5, 'CBC', ['Fermi'], ['MDC'], ['MDC'], mock_gracedb_rest],
-     ['E101','Superevent', 100, -5, 1, 'CBC', [], ['MDC'], ['MDC'], mock_gracedb_rest],
+     ['M103','Superevent', 100, -5, 1, 'CBC', [], ['MDC'], ['MDC'], mock_gracedb_rest],
      ['S102','External', 100, -113, 56, None, ['AGILE'], ['LVOM'], [], mock_gracedb_rest],
      ['E102','Superevent', 100, -5, 1, 'CBC', None, None, None, mock_gracedb_rest],
      # Repeat all tests with GraceDB SDK
      ['E100','Superevent', 100, -5, 1, None, [], [], [], mock_gracedb_sdk],
      ['E101','Superevent', 100, -600, 60, 'Burst', [], [], [], mock_gracedb_sdk],
      ['E102','Superevent', 100, -5, 1, 'CBC', [], [], [], mock_gracedb_sdk],
      ['S100','External', 100, -1, 5, None, ['Fermi','Swift'], [], [], mock_gracedb_sdk],
      ['S100','External', 100, -1, 5, None, ['Fermi','Swift'], ['SubGRB'], [], mock_gracedb_sdk],
      ['S101','External', 100, -10, 10, None, ['SNEWS'], [], [], mock_gracedb_sdk],
      ['S102','External', 100, -1, 5, 'CBC', ['Fermi'], ['MDC'], ['MDC'], mock_gracedb_sdk],
-     ['E101','Superevent', 100, -5, 1, 'CBC', [], ['MDC'], ['MDC'], mock_gracedb_sdk],
+     ['M103','Superevent', 100, -5, 1, 'CBC', [], ['MDC'], ['MDC'], mock_gracedb_sdk],
      ['S102','External', 100, -113, 56, None, ['AGILE'], ['LVOM'], [], mock_gracedb_sdk],
      ['E102','Superevent', 100, -5, 1, 'CBC', None, None, None, mock_gracedb_sdk]])
 def test_search_return(gracedb_id, event_type, gpstime, tl, th, group, pipelines,
                        searches, se_searches, mock_gracedb):
 
     if gracedb_id.startswith('S'):
         event_dict = {'superevent': gracedb_id,
@@ -186,16 +186,16 @@
             "RAVEN: External ['Fermi', 'Swift'] event <a href='https://gracedb-mock.org/events/E4'>E4</a> within [-1, +5] seconds, about 0.500 second(s) before Superevent. Search triggered from S100",
             "RAVEN: Superevent candidate <a href='https://gracedb-mock.org/superevents/S100'>S100</a> within [-5, +1] seconds, about 0.500 second(s) after External event. Search triggered from S100",
             "RAVEN: External ['Fermi', 'Swift'] ['SubGRB'] event <a href='https://gracedb-mock.org/events/E4'>E4</a> within [-1, +5] seconds, about 0.500 second(s) before Superevent. Search triggered from S100",
             "RAVEN: Superevent candidate <a href='https://gracedb-mock.org/superevents/S101'>S101</a> within [-10, +10] seconds, about 6.000 second(s) before External event. Search triggered from S101",
             "RAVEN: External ['SNEWS'] event <a href='https://gracedb-mock.org/events/E2'>E2</a> within [-10, +10] seconds, about 6.000 second(s) after Superevent. Search triggered from S101",
             "RAVEN: Superevent CBC ['MDC'] candidate <a href='https://gracedb-mock.org/superevents/S102'>S102</a> within [-5, +1] seconds, about 0.000 second(s) after External event. Search triggered from S102",
             "RAVEN: External ['Fermi'] ['MDC'] event <a href='https://gracedb-mock.org/events/E4'>E4</a> within [-1, +5] seconds, about 0.000 second(s) before Superevent. Search triggered from S102",
-            "RAVEN: Superevent CBC ['MDC'] candidate <a href='https://gracedb-mock.org/superevents/S4'>S4</a> within [-5, +1] seconds, about 0.500 second(s) after External event. Search triggered from E101",
-            "RAVEN: External ['MDC'] event <a href='https://gracedb-mock.org/events/E101'>E101</a> within [-1, +5] seconds, about 0.500 second(s) before Superevent. Search triggered from E101",
+            "RAVEN: Superevent CBC ['MDC'] candidate <a href='https://gracedb-mock.org/superevents/S4'>S4</a> within [-5, +1] seconds, about 0.500 second(s) after External event. Search triggered from M103",
+            "RAVEN: External ['MDC'] event <a href='https://gracedb-mock.org/events/M103'>M103</a> within [-1, +5] seconds, about 0.500 second(s) before Superevent. Search triggered from M103",
             "RAVEN: No External ['AGILE'] ['LVOM'] candidates in window [-113, +56] seconds. Search triggered from S102"
         ]
  
     if gracedb_id=='E100':
         if is_gracedb_sdk:
             calls_list = mockgracedb.events['E100'].logs.create.call_args_list
             assert calls_list[0][1]['comment'] == message_list[0]
@@ -209,15 +209,15 @@
         else:
             calls_list = mockgracedb.writeLog.call_args_list
             assert calls_list[0][1]['message'] == message_list[0]
             assert calls_list[1][1]['message'] == message_list[1]
             assert calls_list[2][1]['message'] == message_list[2]
             assert calls_list[3][1]['message'] == message_list[3]
 
-    elif gracedb_id=='E101' and not searches:
+    elif gracedb_id=='E101':
         if is_gracedb_sdk:
             calls_list = mockgracedb.events['E101'].logs.create.call_args_list
             assert calls_list[2][1]['comment'] == message_list[4]
 
             calls_list = mockgracedb.superevents['S2'].logs.create.call_args_list
             assert calls_list[2][1]['comment'] == message_list[5]
         else:
@@ -287,15 +287,15 @@
             calls_list = mockgracedb.superevents['S102'].logs.create.call_args_list
             assert calls_list[8][1]['comment'] == message_list[17]
         else:
             calls_list = mockgracedb.writeLog.call_args_list
             assert calls_list[16][1]['message'] == message_list[16]
             assert calls_list[17][1]['message'] == message_list[17]
 
-    elif gracedb_id=='E101':
+    elif gracedb_id=='M103':
         if is_gracedb_sdk:
             calls_list = mockgracedb.events['E4'].logs.create.call_args_list
             assert calls_list[9][1]['comment'] == message_list[18]
 
             calls_list = mockgracedb.superevents['S102'].logs.create.call_args_list
             assert calls_list[9][1]['comment'] == message_list[19]
         else:
@@ -355,15 +355,15 @@
 
 
 @pytest.mark.parametrize('mock_gracedb', [mock_gracedb_rest, mock_gracedb_sdk])
 @patch('ligo.raven.gracedb_events.SE')
 @patch('ligo.raven.gracedb_events.ExtTrig')
 def test_coinc_far_mdc(mock_ExtTrig, mock_SE, mock_gracedb):
 
-    result = raven.search.coinc_far('S100', 'E5', -1, 5, gracedb=mock_gracedb(),
+    result = raven.search.coinc_far('S100', 'M5', -1, 5, gracedb=mock_gracedb(),
                                     grb_search='MDC')
     assert isclose(result['temporal_coinc_far'], 5.8980e-10, abs_tol=1e-13)
     assert result['preferred_event'] == 'G1'
 
 
 @pytest.mark.parametrize('mock_gracedb', [mock_gracedb_rest, mock_gracedb_sdk])
 @patch('ligo.raven.gracedb_events.SE')
```

### Comparing `ligo-raven-3.1.dev0/ligo/raven/tests/test_search_window.py` & `ligo-raven-3.2/ligo/raven/tests/test_search_window.py`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/ligo_raven.egg-info/SOURCES.txt` & `ligo-raven-3.2/ligo_raven.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ligo-raven-3.1.dev0/setup.py` & `ligo-raven-3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='ligo-raven',
-    version='3.1.dev0',
+    version='3.2',
     url='http://gracedb.ligo.org',
     author='Alex Urban',
     author_email='alexander.urban@ligo.org',
     maintainer="Brandon Piotrzkowski",
     maintainer_email="brandon.piotrzkowski@ligo.org",
     description='Low-latency coincidence search between external triggers and GW candidates',
+    readme = "README.md",
     license='GNU General Public License Version 3',
     classifiers=(
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Astronomy",
         "Topic :: Scientific/Engineering :: Physics"
```

