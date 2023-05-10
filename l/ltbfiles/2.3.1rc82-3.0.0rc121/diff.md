# Comparing `tmp/ltbfiles-2.3.1rc82.tar.gz` & `tmp/ltbfiles-3.0.0rc121.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltbfiles-2.3.1rc82.tar", last modified: Fri May  5 13:30:05 2023, max compression
+gzip compressed data, was "ltbfiles-3.0.0rc121.tar", last modified: Wed May 10 12:02:25 2023, max compression
```

## Comparing `ltbfiles-2.3.1rc82.tar` & `ltbfiles-3.0.0rc121.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/LICENSE_GPL_v3.txt
--rw-r--r--   0 root         (0) root         (0)     1119 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.858968 ltbfiles-2.3.1rc82/ltbfiles/
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/ltbfiles/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15777 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/ltbfiles/ltbfiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.860968 ltbfiles-2.3.1rc82/ltbfiles.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1119 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 13:30:05.000000 ltbfiles-2.3.1rc82/ltbfiles.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       43 2023-05-05 13:30:05.861968 ltbfiles-2.3.1rc82/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 13:30:05.860968 ltbfiles-2.3.1rc82/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4776 2023-05-05 13:29:53.000000 ltbfiles-2.3.1rc82/tests/test_load_files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:02:25.977824 ltbfiles-3.0.0rc121/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/LICENSE_GPL_v3.txt
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-05-10 12:02:25.975990 ltbfiles-3.0.0rc121/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:02:25.972323 ltbfiles-3.0.0rc121/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:02:25.974157 ltbfiles-3.0.0rc121/python/ltbfiles/
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/python/ltbfiles/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16202 2023-05-10 12:02:12.000000 ltbfiles-3.0.0rc121/python/ltbfiles/ltbfiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:02:25.975990 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-10 12:02:25.000000 ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-10 12:02:25.977824 ltbfiles-3.0.0rc121/setup.cfg
```

### Comparing `ltbfiles-2.3.1rc82/LICENSE_GPL_v3.txt` & `ltbfiles-3.0.0rc121/LICENSE_GPL_v3.txt`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.1rc82/PKG-INFO` & `ltbfiles-3.0.0rc121/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 2.3.1rc82
+Version: 3.0.0rc121
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ltbfiles-2.3.1rc82/README.md` & `ltbfiles-3.0.0rc121/README.md`

 * *Files identical despite different names*

### Comparing `ltbfiles-2.3.1rc82/ltbfiles/ltbfiles.py` & `ltbfiles-3.0.0rc121/python/ltbfiles/ltbfiles.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,26 +50,30 @@
     if ".ary" == ext:
         return read_ltb_ary(filename)
     if  ".aryx" == ext:
         return read_ltb_aryx(filename)
     raise UnknownTypeException(ext)
 
 
-def load_files(filelist: Union[List[Path],List[str]]) -> Spectra:
+def load_files(filelist: Union[List[Path],List[str]], *, interpolate:bool=False) -> Spectra:
     """
     This function reads the content of multiple spectra files into a merged numpy-array.
 
     Syntax
     ------
         >>> Y,x,o,head = load_files(filenames)
 
     Inputs
     ------
         filenames : list[Path]|list[str]
             List of filenames to be loaded
+    Keyword Arguments
+    -----------------
+        interpolate: bool
+            Interpolate if wavelength axis does not match.
     Outputs
     -------
         Y: numpy-array (m x n)
             2D array containing the intensity values, where the number of
             rows (m) corresponds to the spectral pixels und the number of
             columns (n) corresponds to the number of spectra
         x: numpy-array (m x 1)
@@ -85,33 +89,39 @@
     y, wl, order, h = _load_file(filelist[0])
     Y = np.full((len(y), len(filelist)), np.nan)
     Y[:,0] = y
     head = [h]
     if len(filelist) > 1:
         for i_file, file in enumerate(filelist[1:], start=1):
             y,x,o,h = _load_file(file)
-            assert np.array_equal(x, wl), f"Can only merge spectra with identical wavelength axis (current: '{str(file)}'"
-            assert np.array_equal(o, order), f"Can only merge spectra with identical orders (current: '{str(file)}'"
+            if not (np.array_equal(x, wl) and np.array_equal(o, order)):
+                if not interpolate:
+                    raise IncompatibleSpectraException(
+                        f"Can only merge spectra with identical wavelength axis (current: '{str(file)}'")
+                y = np.interp(wl, x, y)
+                order = np.zeros(x.shape)
             Y[:,i_file] = y
             head.append(h)
     return Spectra(Y, wl, order, head)
 
 
-def find_spectra_in_folder(folder: Union[Path,str], extensions=None) -> List[Path]:
+def scan_for_files(folder: Union[Path,str], *, extensions=None) -> List[Path]:
     """
     Returns a list of all spectra in a given folder.
 
     Syntax
     ------
-        >>> files = find_spectra_in_folder(folder, extensions=SPEC_EXTENSIONS)
+        >>> files = scan_for_files(folder, extensions=SPEC_EXTENSIONS)
 
     Inputs
     ------
         folder : Path|str
             Name of the folder to be scanned for files
+    Keyword Arguments
+    -----------------
         extensions : list[str]
             File extensions that should be searched for. Default = ['.ary', '.aryx']
     Outputs
     -------
         files : list[Path]
             List of spectra files found within the folder
     """
@@ -120,62 +130,65 @@
         extensions = SPEC_EXTENSIONS
     return [
         folder / file for file in folder.iterdir()
         if any(ext == file.suffix for ext in extensions)
     ]
 
 
-def load_folder(folder: Union[Path,str], extensions=None) -> Optional[Spectra]:
+def load_folder(folder: Union[Path,str], *, interpolate:bool=False, extensions=None) -> Optional[Spectra]:
     """
     Load all spectra to be found in a given folder
 
     Syntax
     ------
         >>> Spectra = load_folder(folder, extensions=SPEC_EXTENSIONS)
         >>> Y,x,o,head = load_folder(folder, extensions=SPEC_EXTENSIONS)
 
     Inputs
     ------
         folder : Path|str
             Name of the folder to be scanned for spectra
+    Keyword Arguments
+    -----------------
+        interpolate: bool
+            Interpolate if wavelength axis does not match.
         extensions : list[str]
             File extensions that should be searched for. Default = ['.ary', '.aryx']
     Outputs
     -------
         Spectra : namedtuple
             Spectra loaded from the folder.
             Spectra.Y is a p x n numpy array with "n" being the number of spectra and "p" the number of pixels.
             Spectra.x is the wavelength axis, a p x 1 numpy array
             Spectra.o is the spectral order information, a p x 1 numpy array
             Spectra.head is a list[dict] containing the spectra metadata. Its len is "n"
     """
     if extensions is None:
         extensions = SPEC_EXTENSIONS
-    files = find_spectra_in_folder(folder, extensions)
+    files = scan_for_files(folder, extensions=extensions)
     if len(files) > 0:
-        try:
-            Y, x, o, head = load_files(files)
-        except AssertionError as msg:
-            raise IncompatibleSpectraException(f"Error loading folder: {folder}\n{msg}") from msg
+        Y, x, o, head = load_files(files, interpolate=interpolate)
         return Spectra(Y,x,o,head)
     return None
 
 
-def read_ltb_ary(filename: Union[Path,str], sort_wl: bool=True) -> Spectra:
+def read_ltb_ary(filename: Union[Path,str], *, sort_wl: bool=True) -> Spectra:
     """
     This function reads data from binary *.ary files for LTB spectrometers.
 
     Syntax
     ------
         >>> y,x,o,head = read_ltb_ary(filename, sort_wl)
 
     Inputs
     ------
        filename : Path|str
            Name of the *.ary file to be read. May be a relative path or full filename.
+    Keyword Arguments
+    -----------------
        sortWL : bool
            OPTIONAL flag, if spectra should be sorted by their wavelength after reading. default: true
     Outputs
     -------
        x : float array
            Wavelengths
        o : float array
@@ -251,26 +264,28 @@
             o = o[sort_order]
         else:
             o = np.ones(x.size)
 
     return Spectra(y, x, o, head)
 
 
-def read_ltb_aryx(filename: Union[Path,str], sort_wl:bool=True) -> Spectra:
+def read_ltb_aryx(filename: Union[Path,str], *, sort_wl:bool=True) -> Spectra:
     """
     This function reads data from binary *.aryx files for LTB spectrometers.
 
     Syntax
     ------
         >>> y,x,o,head = read_ltb_aryx(filename, sort_wl)
 
     Inputs
     ------
        filename : Path
            Name of the *.aryx file to be read. May be a relative path or full filename.
+    Keyword Arguments
+    -----------------
        sortWL : bool
            OPTIONAL flag, if spectra should be sorted by their wavelength after reading. default: true
     Outputs
     -------
        x : float array
            Wavelengths
        o : float array
```

### Comparing `ltbfiles-2.3.1rc82/ltbfiles.egg-info/PKG-INFO` & `ltbfiles-3.0.0rc121/python/ltbfiles.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ltbfiles
-Version: 2.3.1rc82
+Version: 3.0.0rc121
 Summary: Module for loading of files created with spectrometers from LTB
 Author: Sven Merk
 Project-URL: Homepage, https://gitlab.com/ltb_berlin/ltb_files
 Project-URL: Bug Tracker, https://gitlab.com/ltb_berlin/ltb_files/-/issues
 Project-URL: Wiki, https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ltbfiles-2.3.1rc82/pyproject.toml` & `ltbfiles-3.0.0rc121/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,14 @@
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/ltb_berlin/ltb_files"
 "Bug Tracker" = "https://gitlab.com/ltb_berlin/ltb_files/-/issues"
 "Wiki" = "https://gitlab.com/ltb_berlin/ltb_files/-/wikis/home"
 
-[tool.setuptools]
-packages = [
-    "ltbfiles"
-]
+[tool.setuptools.packages.find]
+where = ["python"]
+include = ["ltbfiles"]
+exclude = ["tests"]
 
 [tool.setuptools.dynamic]
 version = {attr = "ltbfiles.__version__"}
```

