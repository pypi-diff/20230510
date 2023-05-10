# Comparing `tmp/intnan-0.1.3.tar.gz` & `tmp/intnan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intnan-0.1.3.tar", last modified: Sun Mar 26 15:51:18 2023, max compression
+gzip compressed data, was "intnan-0.1.4.tar", last modified: Wed May 10 12:44:52 2023, max compression
```

## Comparing `intnan-0.1.3.tar` & `intnan-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2023-03-26 15:51:18.899900 intnan-0.1.3/
--rw-rw-r--   0 michael   (1001) michael   (1001)     1317 2022-07-15 21:02:19.000000 intnan-0.1.3/LICENSE
--rw-rw-r--   0 michael   (1001) michael   (1001)     1331 2023-03-26 15:51:18.899900 intnan-0.1.3/PKG-INFO
--rw-rw-r--   0 michael   (1001) michael   (1001)     1640 2022-07-16 12:27:56.000000 intnan-0.1.3/README.md
-drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2023-03-26 15:51:18.899900 intnan-0.1.3/intnan/
--rw-rw-r--   0 michael   (1001) michael   (1001)       91 2022-07-16 10:08:08.000000 intnan-0.1.3/intnan/__init__.py
--rw-rw-r--   0 michael   (1001) michael   (1001)     6319 2023-03-26 15:26:15.000000 intnan-0.1.3/intnan/intnan_np.py
--rw-rw-r--   0 michael   (1001) michael   (1001)     3984 2022-07-16 10:07:50.000000 intnan-0.1.3/intnan/intnan_numba.py
-drwxrwxr-x   0 michael   (1001) michael   (1001)        0 2023-03-26 15:51:18.899900 intnan-0.1.3/intnan.egg-info/
--rw-rw-r--   0 michael   (1001) michael   (1001)     1331 2023-03-26 15:51:18.000000 intnan-0.1.3/intnan.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1001) michael   (1001)      208 2023-03-26 15:51:18.000000 intnan-0.1.3/intnan.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1001) michael   (1001)        1 2023-03-26 15:51:18.000000 intnan-0.1.3/intnan.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1001) michael   (1001)        7 2023-03-26 15:51:18.000000 intnan-0.1.3/intnan.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1001) michael   (1001)       38 2023-03-26 15:51:18.899900 intnan-0.1.3/setup.cfg
--rw-rw-r--   0 michael   (1001) michael   (1001)     3281 2023-03-26 15:48:42.000000 intnan-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:44:52.539379 intnan-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-10 12:44:37.000000 intnan-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-10 12:44:52.539379 intnan-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-10 12:44:37.000000 intnan-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:44:52.539379 intnan-0.1.4/intnan/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 12:44:37.000000 intnan-0.1.4/intnan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 12:44:52.539379 intnan-0.1.4/intnan/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-10 12:44:37.000000 intnan-0.1.4/intnan/intnan_np.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-10 12:44:37.000000 intnan-0.1.4/intnan/intnan_numba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:44:52.539379 intnan-0.1.4/intnan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-10 12:44:52.000000 intnan-0.1.4/intnan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-10 12:44:52.000000 intnan-0.1.4/intnan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:44:52.000000 intnan-0.1.4/intnan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 12:44:52.000000 intnan-0.1.4/intnan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 12:44:52.539379 intnan-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-10 12:44:37.000000 intnan-0.1.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-10 12:44:37.000000 intnan-0.1.4/versioneer.py
```

### Comparing `intnan-0.1.3/LICENSE` & `intnan-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `intnan-0.1.3/PKG-INFO` & `intnan-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intnan
-Version: 0.1.3
+Version: 0.1.4
 Summary: Function collection for handling integers with NaNs
 Home-page: https://github.com/ml31415/intnan
 Download-URL: https://github.com/ml31415/intnan/archive/master.zip
 Author: Michael Loeffler
 Author-email: ml@occam.com.ua
 License: BSD
 Project-URL: Source, https://github.com/ml31415/intnan
```

### Comparing `intnan-0.1.3/README.md` & `intnan-0.1.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-[![GitHub Workflow CI Status](https://img.shields.io/github/workflow/status/ml31415/intnan/Python%20package?logo=github&style=flat)](https://github.com/ml31415/intnan/actions)
+[![GitHub Workflow CI Status](https://img.shields.io/github/actions/workflow/status/ml31415/intnan/python-package.yml?branch=master&logo=github&style=flat)](https://github.com/ml31415/intnan/actions)
 [![Supported Versions](https://img.shields.io/pypi/pyversions/intnan.svg)](https://pypi.org/project/intnan)
 [![PyPI](https://img.shields.io/pypi/v/intnan.svg?style=flat)](https://pypi.org/project/intnan/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # intnan
 
 Integer data types lack special values for `-inf`, `inf` and `NaN`. Especially
 `NaN` as an indication for missing data would be useful in many scientific contexts.
 
 Of course there is `numpy.ma.MaskedArray` around for the very same reason. Nevertheless,
```

### Comparing `intnan-0.1.3/intnan/intnan_np.py` & `intnan-0.1.4/intnan/intnan_np.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,220 +6,264 @@
 The special nan values are chosen depending on the array type.
 Large negative values are used, so that especially python indexing 
 (from the end) is unlikely to work.
 """
 
 import numpy as np
 
-__all__ = ['NANVALS', 'INTNAN32', 'INTNAN64', 'nanval', 'isnan', 'fix_invalid', 'asfloat',
-           'allnan', 'anynan', 'nanmin', 'nanmax', 'nanmaximum', 'nanminimum',
-           'nanmean', 'nanstd', 'nanvar', 'nansum', 'nancumsum', 'nanprod',
-           'nanequal', 'nanclose']
-
-INTNAN32 = np.iinfo('int32').min  # -2147483648
-INTNAN64 = np.iinfo('int64').min  # -9223372036854775808
-NANVALS = dict(d=np.nan, f=np.nan, e=np.nan, S=b'', l=INTNAN64, q=INTNAN32, i=INTNAN32,
-               b=-1, h=-1, B=0, H=0, L=0, Q=0, O=None)
-
-
-def nanval(x):
-    """ Return the corresponding NAN value for a column """
-    return NANVALS.get(x.dtype.char)
+__all__ = [
+    "NANVALS",
+    "INTNAN32",
+    "INTNAN64",
+    "nanval",
+    "isnan",
+    "fix_invalid",
+    "asfloat",
+    "allnan",
+    "anynan",
+    "nanmin",
+    "nanmax",
+    "nanmaximum",
+    "nanminimum",
+    "nanmean",
+    "nanstd",
+    "nanvar",
+    "nansum",
+    "nancumsum",
+    "nanprod",
+    "nanequal",
+    "nanclose",
+]
+
+INTNAN32 = np.iinfo("int32").min  # -2147483648
+INTNAN64 = np.iinfo("int64").min  # -9223372036854775808
+NANVALS = dict(
+    d=np.nan,
+    f=np.nan,
+    e=np.nan,
+    S=b"",
+    U="",
+    l=INTNAN64,
+    q=INTNAN32,
+    i=INTNAN32,
+    b=-1,
+    h=-1,
+    B=0,
+    H=0,
+    L=0,
+    Q=0,
+    O=None,
+)
+
+
+def nanval(x, default=0):
+    """Return the corresponding NAN value for a column or type"""
+    dtype = x.dtype if isinstance(x, np.ndarray) else np.dtype(x)
+    return NANVALS.get(dtype.char, default)
 
 
 def isnan(x):
     if isinstance(x, np.ndarray):
-        nanval = NANVALS.get(x.dtype.char, 0)
-        if nanval is np.nan:
+        nv = nanval(x)
+        if nv is np.nan:
             return np.isnan(x)
-        elif nanval is None:
+        elif nv is None:
             return np.array([val is None for val in x])
         else:
-            return x == nanval
-    elif x in {np.nan, None, '', INTNAN32, INTNAN64}:
+            return x == nv
+    elif x in {np.nan, None, b"", "", INTNAN32, INTNAN64}:
         return True
     else:
         try:
             return np.isnan(x)
         except TypeError:
             return False
 
 
 def fix_invalid(x, copy=True, fill_value=0):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         if copy:
             return np.where(np.isnan(x), fill_value, x)
         else:
             x[np.isnan(x)] = fill_value
             return x
-    elif nanval is None:
+    elif nv is None:
         ret = np.zeros_like(x)
         x_flat = x.flat
         for i in range(x.size):
             if x_flat[i] is None:
                 ret[i] = fill_value
             else:
                 ret[i] = x_flat[i]
         return ret
     else:
         if copy:
-            return np.where(x == nanval, fill_value, x)
+            return np.where(x == nv, fill_value, x)
         else:
-            x[x == nanval] = fill_value
+            x[x == nv] = fill_value
             return x
 
 
 def asfloat(x):
     if issubclass(x.dtype.type, np.floating):
         return x.copy()
     elif issubclass(x.dtype.type, np.bool_):
         return np.array(x, dtype=float)
     return fix_invalid(x, fill_value=np.nan)
 
 
+def asint(x):
+    if issubclass(x.dtype.type, np.integer):
+        return x.copy()
+    elif issubclass(x.dtype.type, np.bool_):
+        return np.array(x, dtype=int)
+    nv = nanval(int)
+    return np.nan_to_num(x, nan=nv, posinf=nv, neginf=nv).astype(int)
+
+
 def anynan(x):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.any(np.isnan(x))
-    elif nanval is None:
+    elif nv is None:
         return any(val is None for val in x.flat)
     else:
-        return nanval in x
+        return nv in x
 
 
 def allnan(x):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.all(np.isnan(x))
-    elif nanval is None:
+    elif nv is None:
         return all(val is None for val in x.flat)
     else:
-        return np.all(x == nanval)
+        return np.all(x == nv)
 
 
 def nanmax(x):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.nanmax(x)
     else:
         try:
-            return np.max(x[x != nanval])
+            return np.max(x[x != nv])
         except ValueError as e:
-            if 'zero-size' in str(e):
-                return nanval
+            if "zero-size" in str(e):
+                return nv
             else:
                 raise
 
 
 def nanmin(x):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.nanmin(x)
     else:
         try:
-            return np.min(x[x != nanval])
+            return np.min(x[x != nv])
         except ValueError as e:
-            if 'zero-size' in str(e):
-                return nanval
+            if "zero-size" in str(e):
+                return nv
             else:
                 raise
 
 
 def nanmaximum(x, y):
-    """ Does the same as numpy.maximum (element-wise maximum operation of two arrays) but ignores NaNs """
+    """Does the same as numpy.maximum (element-wise maximum operation of two arrays) but ignores NaNs"""
     z = np.maximum(x, y)
     badx = isnan(x)
     bady = isnan(y)
     z[badx] = y[badx]
     z[bady] = x[bady]
     return z
 
 
 def nanminimum(x, y):
-    """ Does the same as numpy.minimum (element-wise minimum operation of two arrays) but ignores NaNs """
+    """Does the same as numpy.minimum (element-wise minimum operation of two arrays) but ignores NaNs"""
     z = np.minimum(x, y)
     badx = isnan(x)
     bady = isnan(y)
     z[badx] = y[badx]
     z[bady] = x[bady]
     return z
 
 
 def nansum(x):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.nansum(x)
     else:
-        return np.sum(x[x != nanval])
+        return np.sum(x[x != nv])
 
 
 def nanprod(x):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.nanprod(x, dtype=np.float64)
     else:
-        return np.prod(x[x != nanval])
+        return np.prod(x[x != nv])
 
 
 def nancumsum(x):
-    nanval = NANVALS.get(x.dtype.char, 0)
+    nv = nanval(x)
     result = np.cumsum(fix_invalid(x))
 
     if anynan(x):
         # cumsum is undefined before the first valid number appears, so we need to replace
         # the nans starting from the beginning of the array
         # TODO: Finding the first instance of a value this way is quite some overhead
         good_idx = np.where(~isnan(x))[0]
         if len(good_idx) > 0:
-            result[:good_idx[0]] = nanval
+            result[: good_idx[0]] = nv
         else:
-            result[:] = nanval
+            result[:] = nv
     return result
 
 
 def nanmean(x):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.nanmean(x)
     else:
-        with np.errstate(invalid='ignore'):
-            return np.mean(x[x != nanval])
+        with np.errstate(invalid="ignore"):
+            return np.mean(x[x != nv])
 
 
 def nanvar(x, ddof=0):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.nanvar(x, ddof=ddof)
     else:
-        with np.errstate(invalid='ignore'):
-            return np.var(x[x != nanval], ddof=ddof)
+        with np.errstate(invalid="ignore"):
+            return np.var(x[x != nv], ddof=ddof)
 
 
 def nanstd(x, ddof=0):
-    nanval = NANVALS.get(x.dtype.char, 0)
-    if nanval is np.nan:
+    nv = nanval(x)
+    if nv is np.nan:
         return np.nanstd(x, ddof=ddof)
     else:
-        with np.errstate(invalid='ignore'):
-            return np.std(x[x != nanval], ddof=ddof)
+        with np.errstate(invalid="ignore"):
+            return np.std(x[x != nv], ddof=ddof)
 
 
 def nanequal(x, y):
     """Treat NaN as an ordinary value when comparing for equality."""
     if x.dtype != y.dtype:
-        raise TypeError("nanequal requires same data type: %s != %s" % (x.dtype, y.dtype))
+        raise TypeError(f"nanequal requires same data type: {x.dtype} != {y.dtype}")
     if issubclass(x.dtype.type, np.floating) and issubclass(y.dtype.type, np.floating):
         return np.isclose(x, y, 0, 0, equal_nan=True)
     else:
         return x == y
 
 
 def nanclose(x, y, delta=np.finfo(float).eps):
     if x.dtype != y.dtype:
-        raise TypeError("nanclose requires same data type: %s != %s" % (x.dtype, y.dtype))
+        raise TypeError(f"nanclose requires same data type: {x.dtype} != {y.dtype}")
     if issubclass(x.dtype.type, np.integer):
         return np.isclose(x, y, atol=delta, equal_nan=True)
     elif issubclass(x.dtype.type, str):
         return x == y
     else:
         return np.isclose(x, y, atol=delta, equal_nan=True)
```

### Comparing `intnan-0.1.3/intnan/intnan_numba.py` & `intnan-0.1.4/intnan/intnan_numba.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 """ A bunch of small functions that replace and improve former usage of numexpr and bottleneck """
 
 import numpy as np
 import numba as nb
 
 
-from .intnan_np import (INTNAN32, INTNAN64,  NANVALS, nanval, isnan, asfloat,
-                        nanequal, nanclose, __all__)
+from .intnan_np import (
+    INTNAN32,
+    INTNAN64,
+    NANVALS,
+    nanval,
+    isnan,
+    asfloat,
+    nanequal,
+    nanclose,
+    __all__,
+)
 
 
 def nancalc(func):
     jfunc = nb.njit(func)
 
     def wrapped(*args, **kwargs):
         nv = nanval(args[0])
@@ -181,14 +190,15 @@
     ex_mean = 0
     for x_ in x.flat:
         if not isnan_vec(x_, nan):
             inc = x_ - mean
             ex_mean += inc * inc
     return ex_mean / (cnt - ddof)
 
+
 _jnanvar = nb.njit(_nanvar)
 nanvar = nancalc(_nanvar)
 
 
 @nancalc
 def nanstd(x, nan, ddof=0):
     return np.sqrt(_jnanvar(x, nan, ddof=ddof))
```

### Comparing `intnan-0.1.3/intnan.egg-info/PKG-INFO` & `intnan-0.1.4/intnan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intnan
-Version: 0.1.3
+Version: 0.1.4
 Summary: Function collection for handling integers with NaNs
 Home-page: https://github.com/ml31415/intnan
 Download-URL: https://github.com/ml31415/intnan/archive/master.zip
 Author: Michael Loeffler
 Author-email: ml@occam.com.ua
 License: BSD
 Project-URL: Source, https://github.com/ml31415/intnan
```

### Comparing `intnan-0.1.3/setup.py` & `intnan-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 
 import os
 from setuptools import setup, Command
 from shutil import rmtree
+import versioneer
 
 base_path = os.path.dirname(os.path.abspath(__file__))
 
 long_description = """
 Integer data types lack special values for -inf, inf and NaN. Especially
 NaN as an indication for missing data would be useful in many scientific contexts.
 
@@ -26,58 +27,60 @@
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
-        for folder in ('build', 'dist', 'intnan.egg-info'):
+        for folder in ("build", "dist", "intnan.egg-info"):
             path = os.path.join(base_path, folder)
             if os.path.isdir(path):
                 print("removing '{}' (and everything under it)".format(path))
                 if not self.dry_run:
                     rmtree(path)
         self._rm_walk()
 
     def _rm_walk(self):
         for path, dirs, files in os.walk(base_path):
-            if any(p.startswith('.') for p in path.split(os.path.sep)):
+            if any(p.startswith(".") for p in path.split(os.path.sep)):
                 # Skip hidden directories like the git folder right away
                 continue
-            if path.endswith('__pycache__'):
+            if path.endswith("__pycache__"):
                 print("removing '{}' (and everything under it)".format(path))
                 if not self.dry_run:
                     rmtree(path)
             else:
                 for fname in files:
-                    if fname.endswith('.pyc') or fname.endswith('.so'):
+                    if fname.endswith(".pyc") or fname.endswith(".so"):
                         fpath = os.path.join(path, fname)
                         print("removing '{}'".format(fpath))
                         if not self.dry_run:
                             os.remove(fpath)
 
 
-setup(name='intnan',
-      version="0.1.3",
-      author="Michael Loeffler",
-      author_email="ml@occam.com.ua",
-      license='BSD',
-      description="Function collection for handling integers with NaNs",
-      long_description=long_description,
-      long_description_content_type="text/x-rst",
-      url="https://github.com/ml31415/intnan",
-      download_url="https://github.com/ml31415/intnan/archive/master.zip",
-      keywords=[ "integer", "nan", "missing values", "intnan"],
-      packages=["intnan"],
-      install_requires=[],
-      setup_requires=["pytest-runner"],
-      tests_require=["pytest", "numpy", "numba"],
-      classifiers=['Development Status :: 4 - Beta',
-                   'Intended Audience :: Science/Research',
-                   'Programming Language :: Python :: 3.7',
-                   'Programming Language :: Python :: 3.8',
-                   'Programming Language :: Python :: 3.9',
-                   'Programming Language :: Python :: 3.10',
-                   ],
-      cmdclass={"clean": Clean},
-      project_urls={"Source": "https://github.com/ml31415/intnan"}
+setup(
+    name="intnan",
+    version=versioneer.get_version(),
+    author="Michael Loeffler",
+    author_email="ml@occam.com.ua",
+    license="BSD",
+    description="Function collection for handling integers with NaNs",
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
+    url="https://github.com/ml31415/intnan",
+    download_url="https://github.com/ml31415/intnan/archive/master.zip",
+    keywords=["integer", "nan", "missing values", "intnan"],
+    packages=["intnan"],
+    install_requires=[],
+    setup_requires=["pytest-runner", "versioneer"],
+    tests_require=["pytest", "numpy", "numba"],
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Science/Research",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+    ],
+    cmdclass=versioneer.get_cmdclass({"clean": Clean}),
+    project_urls={"Source": "https://github.com/ml31415/intnan"},
 )
```

