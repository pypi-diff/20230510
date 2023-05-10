# Comparing `tmp/JanusReader-0.4.2.tar.gz` & `tmp/JanusReader-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JanusReader-0.4.2.tar", last modified: Tue Apr  4 10:49:33 2023, max compression
+gzip compressed data, was "JanusReader-0.5.0.tar", last modified: Wed May 10 08:10:10 2023, max compression
```

## Comparing `JanusReader-0.4.2.tar` & `JanusReader-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-04-04 10:49:33.693545 JanusReader-0.4.2/
--rw-r--r--   0 romolo.politi   (501) staff       (20)      420 2023-04-04 10:49:33.693328 JanusReader-0.4.2/PKG-INFO
--rw-r--r--   0 romolo.politi   (501) staff       (20)      228 2023-03-18 08:22:58.000000 JanusReader-0.4.2/README.md
--rw-r--r--   0 romolo.politi   (501) staff       (20)      437 2023-04-04 10:49:17.000000 JanusReader-0.4.2/pyproject.toml
--rw-r--r--   0 romolo.politi   (501) staff       (20)       38 2023-04-04 10:49:33.693610 JanusReader-0.4.2/setup.cfg
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-04-04 10:49:33.690189 JanusReader-0.4.2/src/
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-04-04 10:49:33.691777 JanusReader-0.4.2/src/JanusReader/
--rw-r--r--   0 romolo.politi   (501) staff       (20)       88 2023-03-03 08:06:39.000000 JanusReader-0.4.2/src/JanusReader/__init__.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)      103 2022-05-04 08:58:16.000000 JanusReader-0.4.2/src/JanusReader/exceptions.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)    12314 2023-04-04 10:42:23.000000 JanusReader-0.4.2/src/JanusReader/janusReader.py
--rw-r--r--   0 romolo.politi   (501) staff       (20)     2302 2023-03-03 15:12:36.000000 JanusReader-0.4.2/src/JanusReader/vicar_head.py
-drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-04-04 10:49:33.692998 JanusReader-0.4.2/src/JanusReader.egg-info/
--rw-r--r--   0 romolo.politi   (501) staff       (20)      420 2023-04-04 10:49:33.000000 JanusReader-0.4.2/src/JanusReader.egg-info/PKG-INFO
--rw-r--r--   0 romolo.politi   (501) staff       (20)      337 2023-04-04 10:49:33.000000 JanusReader-0.4.2/src/JanusReader.egg-info/SOURCES.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)        1 2023-04-04 10:49:33.000000 JanusReader-0.4.2/src/JanusReader.egg-info/dependency_links.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)       73 2023-04-04 10:49:33.000000 JanusReader-0.4.2/src/JanusReader.egg-info/requires.txt
--rw-r--r--   0 romolo.politi   (501) staff       (20)       12 2023-04-04 10:49:33.000000 JanusReader-0.4.2/src/JanusReader.egg-info/top_level.txt
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-10 08:10:10.483035 JanusReader-0.5.0/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-10 08:10:10.482807 JanusReader-0.5.0/PKG-INFO
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      257 2023-05-10 08:09:29.000000 JanusReader-0.5.0/README.md
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      437 2023-05-10 08:08:52.000000 JanusReader-0.5.0/pyproject.toml
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       38 2023-05-10 08:10:10.483118 JanusReader-0.5.0/setup.cfg
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-10 08:10:10.479426 JanusReader-0.5.0/src/
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-10 08:10:10.481039 JanusReader-0.5.0/src/JanusReader/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       88 2023-03-03 08:06:39.000000 JanusReader-0.5.0/src/JanusReader/__init__.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      103 2022-05-04 08:58:16.000000 JanusReader-0.5.0/src/JanusReader/exceptions.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)    12458 2023-05-10 08:08:22.000000 JanusReader-0.5.0/src/JanusReader/janusReader.py
+-rw-r--r--   0 romolo.politi   (501) staff       (20)     2302 2023-03-03 15:12:36.000000 JanusReader-0.5.0/src/JanusReader/vicar_head.py
+drwxr-xr-x   0 romolo.politi   (501) staff       (20)        0 2023-05-10 08:10:10.482456 JanusReader-0.5.0/src/JanusReader.egg-info/
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      449 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/PKG-INFO
+-rw-r--r--   0 romolo.politi   (501) staff       (20)      337 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/SOURCES.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)        1 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/dependency_links.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       73 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/requires.txt
+-rw-r--r--   0 romolo.politi   (501) staff       (20)       12 2023-05-10 08:10:10.000000 JanusReader-0.5.0/src/JanusReader.egg-info/top_level.txt
```

### Comparing `JanusReader-0.4.2/src/JanusReader/janusReader.py` & `JanusReader-0.5.0/src/JanusReader/janusReader.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,38 +87,40 @@
     
     def __init__(self,proc):
         self.badPixelCorrection = int(getValue(
             proc, 'juice_janus:bad_pixel_correction'))
         self.badPixelMapName = getValue(
             proc, 'juice_janus:bad_pixel_map_name')
         self.badPixelCount = int(getValue(proc, 'juice_janus:bad_pixel_count'))
-        self.dnsuCorrection = int(getValue(proc, 'juice_janus:dsnu_correction'))
-        self.dnsuMapName = getValue(proc, 'juice_janus:dsnu_map_name')
+        self.fpnCorrection = int(getValue(proc, 'juice_janus:fpn_correction'))
+        self.fpnMapName = getValue(proc, 'juice_janus:fpn_map_name')
         self.spikeMaximumValue = int(
             getValue(proc, 'juice_janus:spike_maximum_value'))
         self.spikeDistance = int(getValue(proc, 'juice_janus:spike_distance'))
         self.spikeCount = int(getValue(proc, 'juice_janus:spike_count'))
+        self.spikeCorrection = int(getValue(proc, 'juice_janus:spike_correction'))
     
     def Show(self):
         tb = Table(expand=False, show_header=False,
                    show_lines=False, box=box.SIMPLE_HEAD,
                    title="Onboard Processing", title_style="italic yellow")
         tb.add_column(style='yellow', justify='left')
         tb.add_column()
         tb.add_column()
         tb.add_row("Bad Pixels Correction", "",str(self.badPixelCorrection))
         tb.add_row("Bad Pixel Map Name","", self.badPixelMapName)
         tb.add_row("Bad Pixel Count","", str(self.badPixelCount))
         tb.add_section()
-        tb.add_row("DSNU Correction", "", str(self.dnsuCorrection))
-        tb.add_row("DSNU Map Name","", self.dnsuMapName)
+        tb.add_row("FPN Correction", "", str(self.fpnCorrection))
+        tb.add_row("FPN Map Name","", self.fpnMapName)
         tb.add_section()
         tb.add_row("Spike Maximum Value", "", str(self.spikeMaximumValue))
         tb.add_row("Spike Distance","", str(self.spikeDistance))
         tb.add_row("Spike Distance","", str(self.spikeDistance))
+        tb.add_row("Spike Correction","", str(self.spikeCorrection))
         return tb
 
 class JanusReader:
     """Reader of the JANUS Data File
 
         Args:
             fileName (Path): input filename
@@ -128,15 +130,15 @@
             fileName (Path): input filename
             img (np.array): image data
 
         Raises:
             NOT_VALID_VICAR_FILE
                 The input file ``fileName`` is not ion VICAR format.
         """
-    __version__="0.1.2"
+    __version__="0.4.2"
     def __init__(self, fileName:Path, console:Console=None,debug:bool=False,vicar:bool=False):
         # Check if console exists, if not create one
         if console is None:
             console=Console()
         self.console=console
         # Check the file type, is str convert to Path
         if type(fileName) is not Path:
```

### Comparing `JanusReader-0.4.2/src/JanusReader/vicar_head.py` & `JanusReader-0.5.0/src/JanusReader/vicar_head.py`

 * *Files identical despite different names*

