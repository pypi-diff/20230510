# Comparing `tmp/openvisuspy-1.0.1-py3-none-any.whl.zip` & `tmp/openvisuspy-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 25028 bytes, number of entries: 15
--rw-r--r--  2.0 unx      239 b- defN 23-May-08 20:27 openvisuspy/__init__.py
--rw-r--r--  2.0 unx     3757 b- defN 23-May-08 20:27 openvisuspy/app.py
--rw-r--r--  2.0 unx     6033 b- defN 23-May-08 20:27 openvisuspy/backend.py
--rw-r--r--  2.0 unx     7093 b- defN 23-May-08 20:27 openvisuspy/backend_cpp.py
--rw-r--r--  2.0 unx    11577 b- defN 23-May-08 20:27 openvisuspy/backend_py.py
--rw-r--r--  2.0 unx     4417 b- defN 23-May-08 20:27 openvisuspy/canvas.py
--rw-r--r--  2.0 unx     6655 b- defN 23-May-08 20:27 openvisuspy/slice.py
--rw-r--r--  2.0 unx     1498 b- defN 23-May-08 20:27 openvisuspy/slices.py
--rw-r--r--  2.0 unx     7249 b- defN 23-May-08 20:27 openvisuspy/utils.py
--rw-r--r--  2.0 unx    16756 b- defN 23-May-08 20:27 openvisuspy/widgets.py
--rw-r--r--  2.0 unx     1849 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2068 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1195 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/RECORD
-15 files, 70490 bytes uncompressed, 23072 bytes compressed:  67.3%
+Zip file size: 25203 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      239 b- defN 23-May-08 21:22 openvisuspy/__init__.py
+-rw-r--r--  2.0 unx     3757 b- defN 23-May-08 21:22 openvisuspy/app.py
+-rw-r--r--  2.0 unx     6033 b- defN 23-May-08 21:22 openvisuspy/backend.py
+-rw-r--r--  2.0 unx     7093 b- defN 23-May-08 21:22 openvisuspy/backend_cpp.py
+-rw-r--r--  2.0 unx    11577 b- defN 23-May-08 21:22 openvisuspy/backend_py.py
+-rw-r--r--  2.0 unx     4417 b- defN 23-May-08 21:22 openvisuspy/canvas.py
+-rw-r--r--  2.0 unx     6655 b- defN 23-May-08 21:22 openvisuspy/slice.py
+-rw-r--r--  2.0 unx     1498 b- defN 23-May-08 21:22 openvisuspy/slices.py
+-rw-r--r--  2.0 unx     7249 b- defN 23-May-08 21:22 openvisuspy/utils.py
+-rw-r--r--  2.0 unx    16756 b- defN 23-May-08 21:22 openvisuspy/widgets.py
+-rwxrwxrwx  2.0 unx     1849 b- defN 23-May-10 18:54 openvisuspy-1.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2737 b- defN 23-May-10 18:54 openvisuspy-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 18:54 openvisuspy-1.0.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       12 b- defN 23-May-10 18:54 openvisuspy-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1195 b- defN 23-May-10 18:54 openvisuspy-1.0.2.dist-info/RECORD
+15 files, 71159 bytes uncompressed, 23247 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: openvisuspy/utils.py
 Comment: 
 
 Filename: openvisuspy/widgets.py
 Comment: 
 
-Filename: openvisuspy-1.0.1.dist-info/LICENSE
+Filename: openvisuspy-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: openvisuspy-1.0.1.dist-info/METADATA
+Filename: openvisuspy-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: openvisuspy-1.0.1.dist-info/WHEEL
+Filename: openvisuspy-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: openvisuspy-1.0.1.dist-info/top_level.txt
+Filename: openvisuspy-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: openvisuspy-1.0.1.dist-info/RECORD
+Filename: openvisuspy-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `openvisuspy-1.0.1.dist-info/LICENSE` & `openvisuspy-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openvisuspy-1.0.1.dist-info/METADATA` & `openvisuspy-1.0.2.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openvisuspy
-Version: 1.0.1
+Version: 1.0.2
 Summary: openvisuspy
 Author: OpenVisus developers
 Project-URL: Homepage, https://github.com/sci-visus/openvisuspy
 Project-URL: Bug Tracker, https://github.com/sci-visus/openvisuspy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -52,14 +52,23 @@
 
 ```
 python3 -m bokeh serve "examples/dashboards/run.py"  --dev --address localhost --args --single
 python3 -m bokeh serve "examples/dashboards/run.py"  --dev --address localhost --args --multi
 python3 -m bokeh serve "examples/dashboards/nasa.py" --dev --address localhost --args --single
 ```
 
+Other misc examples:
+
+```
+python -m bokeh serve "examples/dashboards/run.py"  --dev --args --dataset  "https://atlantis.sci.utah.edu/mod_visus?dataset=david_subsampled&cached=1" --palette Greys256    --palette-range "[0, 255]"
+python -m bokeh serve "examples/dashboards/run.py"  --dev --args --dataset  "https://atlantis.sci.utah.edu/mod_visus?dataset=2kbit1&cached=1"           --palette Greys256    --palette-range "[0, 255]"
+python -m bokeh serve "examples/dashboards/run.py"  --dev --args --dataset  "https://atlantis.sci.utah.edu/mod_visus?dataset=chess-zip&cached=1"        --palette Viridis256  --palette-range "[-0.017141795, 0.012004322]" --num-views 3 
+
+```
+
 ## Panel Dashboards 
 
 ```
 python -m panel serve "examples/dashboards/run.py"  --dev --address localhost --args --single
 python -m panel serve "examples/dashboards/run.py"  --dev --address localhost --args --multi
 python -m panel serve "examples/dashboards/nasa.py" --dev --address localhost --args --single
 ```
```

## Comparing `openvisuspy-1.0.1.dist-info/RECORD` & `openvisuspy-1.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 openvisuspy/backend_cpp.py,sha256=ZukezVcj3DikB823ZvinWDb2Tlefke5CjRoSLCDjNTw,7093
 openvisuspy/backend_py.py,sha256=B-ns-tcnhhrE9AedVS6nrVICxZjkkYkqr_oa9mBd2uk,11577
 openvisuspy/canvas.py,sha256=oa42eKl7mQSRnagJ9Kz0uG8duJV0eKaaeG8fFLE6N3A,4417
 openvisuspy/slice.py,sha256=lrerqoE5fekQ0-D0KBWKk_dugRVHKFT-NavfJ3iR3-E,6655
 openvisuspy/slices.py,sha256=ijF00q4UpLMsYC1poXVjr2ZvZM2nl5OZnLh94scjWEM,1498
 openvisuspy/utils.py,sha256=DGfo09rGiKQdB6SHJiEWmOYeMTJnxRJFNUNWPUTxmVQ,7249
 openvisuspy/widgets.py,sha256=OADksn13PktE8giInU-IVH9Ti8skz_S6mdLrVMkzWeQ,16756
-openvisuspy-1.0.1.dist-info/LICENSE,sha256=6e8f7JrZAwWAqUNg-mtEFpikTHZvcDrSGPViHeAlgrw,1849
-openvisuspy-1.0.1.dist-info/METADATA,sha256=tICbGsHvEsP4bSxgkGx9D5rBD__EYTtATVsNOEuVTNs,2068
-openvisuspy-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openvisuspy-1.0.1.dist-info/top_level.txt,sha256=o9WLF82UoNRuLU1MIOWVUfHBb7u7oGs9w2i6lfhRy_Y,12
-openvisuspy-1.0.1.dist-info/RECORD,,
+openvisuspy-1.0.2.dist-info/LICENSE,sha256=6e8f7JrZAwWAqUNg-mtEFpikTHZvcDrSGPViHeAlgrw,1849
+openvisuspy-1.0.2.dist-info/METADATA,sha256=2G4th87WwkN7VXxbMqm0GWP4oHAaovUTROXSRHKLXVU,2737
+openvisuspy-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openvisuspy-1.0.2.dist-info/top_level.txt,sha256=o9WLF82UoNRuLU1MIOWVUfHBb7u7oGs9w2i6lfhRy_Y,12
+openvisuspy-1.0.2.dist-info/RECORD,,
```

