# Comparing `tmp/haicu-0.9.1.tar.gz` & `tmp/haicu-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.9.1.tar", last modified: Wed May 10 19:21:10 2023, max compression
+gzip compressed data, was "haicu-0.9.2.tar", last modified: Wed May 10 21:01:38 2023, max compression
```

## Comparing `haicu-0.9.1.tar` & `haicu-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 19:21:10.963298 haicu-0.9.1/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.9.1/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-05-10 19:21:10.963298 haicu-0.9.1/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     2619 2023-05-09 22:37:20.000000 haicu-0.9.1/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 19:21:10.963298 haicu-0.9.1/haicu/
--rwxrwxr-x   0 bry       (1000) bry       (1000)    27584 2023-05-10 17:46:13.000000 haicu-0.9.1/haicu/__haicu_ctl.py
--rw-rw-r--   0 bry       (1000) bry       (1000)       43 2023-05-10 19:18:48.000000 haicu-0.9.1/haicu/__init__.py
--rw-rw-r--   0 bry       (1000) bry       (1000)       80 2023-05-10 17:49:55.000000 haicu-0.9.1/haicu/__main__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    22189 2023-05-10 19:20:54.000000 haicu-0.9.1/haicu/format.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    15626 2023-05-10 17:46:15.000000 haicu-0.9.1/haicu/ftdi.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 19:21:10.963298 haicu-0.9.1/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-05-10 19:21:10.000000 haicu-0.9.1/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      295 2023-05-10 19:21:10.000000 haicu-0.9.1/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-05-10 19:21:10.000000 haicu-0.9.1/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       53 2023-05-10 19:21:10.000000 haicu-0.9.1/haicu.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-05-10 19:21:10.000000 haicu-0.9.1/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-05-10 19:21:10.000000 haicu-0.9.1/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      832 2023-05-10 17:49:32.000000 haicu-0.9.1/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-05-10 19:21:10.963298 haicu-0.9.1/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 21:01:38.537605 haicu-0.9.2/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.9.2/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-05-10 21:01:38.537605 haicu-0.9.2/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2619 2023-05-09 22:37:20.000000 haicu-0.9.2/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 21:01:38.537605 haicu-0.9.2/haicu/
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    27557 2023-05-10 20:58:28.000000 haicu-0.9.2/haicu/__haicu_ctl.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)       43 2023-05-10 21:01:34.000000 haicu-0.9.2/haicu/__init__.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)       80 2023-05-10 17:49:55.000000 haicu-0.9.2/haicu/__main__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    22343 2023-05-10 20:04:34.000000 haicu-0.9.2/haicu/format.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)    15631 2023-05-10 19:56:51.000000 haicu-0.9.2/haicu/ftdi.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 21:01:38.537605 haicu-0.9.2/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      295 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       53 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-05-10 21:01:38.000000 haicu-0.9.2/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      832 2023-05-10 17:49:32.000000 haicu-0.9.2/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-05-10 21:01:38.537605 haicu-0.9.2/setup.cfg
```

### Comparing `haicu-0.9.1/LICENSE` & `haicu-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.9.1/PKG-INFO` & `haicu-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.9.1
+Version: 0.9.2
 Summary: package for HAICU experiment
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.9.1/README.md` & `haicu-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `haicu-0.9.1/haicu/__haicu_ctl.py` & `haicu-0.9.2/haicu/__haicu_ctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,15 +479,15 @@
         sys.exit(-1)
 
     in_name, in_ext = os.path.splitext(args.file)
 
     try:
         if(in_ext.lower() == ".txt"):
             print("Generating RLE from " + args.file)
-            rle = haicu_format.convert_derived_absolute2rle(args.file)
+            rle = haicu_format.convert_derived2rle(args.file)
         elif(in_ext.lower() == ".rle"):
             rle = haicu_format.load_rle_from_file(args.file)
         else:
             print("Invalid filetype " + in_ext + ". Must be .rle or .txt")
             sys.exit(-1)
 
     except:
@@ -513,15 +513,15 @@
     in_name, in_ext = os.path.splitext(in_file)
 
     # Load the RLE file
     try:
         if(in_ext.lower() == ".txt"):
             if(args.verbose > 0):
                 print("Generating RLE from " + in_file)
-            rle = haicu_format.convert_derived_absolute2rle(in_file)
+            rle = haicu_format.convert_derived2rle(in_file)
         elif(in_ext.lower() == ".rle"):
             if(args.verbose > 0):
                 print("Loading RLE payload from " + in_file)
             rle = haicu_format.load_rle_from_file(in_file)
         else:
             if(args.verbose > 0):
                 print("Invalid filetype " + in_ext + ". Must be .rle or .txt")
@@ -583,15 +583,15 @@
         sys.exit(-1)
 
     out_name, out_ext = os.path.splitext(args.outfile)
     if(out_ext != ".rle"):
         print("Invalid extension, output file must be .rle")
         sys.exit(-1)
 
-    rle = haicu_format.convert_derived_absolute2rle(args.infile)
+    rle = haicu_format.convert_derived2rle(args.infile)
     if(args.verbose > 1):
         pprint.pprint(rle) # Debug print, only useful for tiny derived.txt files
 
     if(args.verbose > 0):
         print("Creating RLE file " + args.outfile)
 
     with open(args.outfile, "wb+") as f:
```

### Comparing `haicu-0.9.1/haicu/format.py` & `haicu-0.9.2/haicu/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import struct
-import csv
-import pprint
 from simplejson import dumps
 
-
 NUM_RUN_BITS = 13  # 13-bit maximum in run-length encoding 'run' field
 MAX_RUN_ALLOWED_RLE = pow(2, NUM_RUN_BITS)
 
-def convert_derived_absolute2rle(derived_file_name):
+def convert_derived_absolute2rle(derived_file_name: str) -> list[list[bytearray]]:
     """Convert absolute timing derived file to RLE format suitable for upload to device
 
     Args:
         derived_file_name(str): File to convert to RLE format
 
     Returns:
         A list containing each section found in derived file. Each section is given as an array of bytes
@@ -196,15 +193,15 @@
         for time_div in range(len(initial[section][0])):
             time_required = time_required + int(initial[section][0][time_div])
 
         # print("Time required for section " + str(section) + ":" + str(time_required * 10) + "ns (" + str(time_required * 10 / 1000000) + "ms)")
 
     return final
 
-def convert_derived2rle(derived_file_name):
+def convert_derived2rle(derived_file_name: str) -> list[list[bytearray]]:
     """Convert derived file to RLE format suitable for upload to device
 
     Args:
         derived_file_name(str): File to convert to RLE format
 
     Returns:
         A list containing each section found in derived file. Each section is given as an array of bytes
@@ -337,15 +334,15 @@
         # print()
         # final[section] = rle
 
     return final
 
 
 
-def convert_rle2raw(rle_file_name):
+def convert_rle2raw(rle_file_name: str) -> list[list[int]]:
     """Convert RLE file to raw format. Typical use for allowing comparisons between different formats
 
     Args:
         rle_file_name(str): File to convert to 'raw' format
 
     Returns:
         List containing each section, inside of which is an array of the 8 tuneboxes, and the address (Left + Right + Front Panel)
@@ -390,15 +387,15 @@
                 # print("Sum per line: " + str(val))
 
             # print()
             section = section + 1
 
     return final
 
-def convert_derived2raw(derived_file_name):
+def convert_derived2raw(derived_file_name: str) -> list[list[int]]:
     """Convert derived file to raw format. Typical use for allowing comparisons between different formats
 
     Args:
         derived_file_name(str): File to convert to 'raw' format
 
     Returns:
         List containing each section, inside of which is an array of the 8 tuneboxes, and the address (Left + Right + Front Panel)
@@ -453,15 +450,15 @@
             #     val = val + final[section][n][i]
             # print("Sum per line: " + str(val))
 
         # print()
 
     return final
 
-def load_rle_from_file(rle_file_name):
+def load_rle_from_file(rle_file_name: str) -> list[list[int]]:
     """Load an RLE file from disk into memory. Each section is loaded as an array of 32-bit integer values
 
     Args:
         rle_file_name(str): Path to RLE file to load
 
     Returns:
         List of sections, each containing an array of integer values
@@ -479,15 +476,15 @@
                 final[section].append(section_data)
 
             section = section + 1
             chunk = f.read(4)
 
     return final
 
-def match(derived_file, rle_file):
+def match(derived_file: str, rle_file: str) -> bool:
     """Checks if a derived file and and RLE file match output when converted to the same 'raw' format
 
     Args:
         derived_file(str): Path to derived file
 
         rle_file(str): Path to RLE file
 
@@ -501,14 +498,17 @@
     bin_json = dumps(derived_binary)
 
     rle_binary = convert_rle2raw(rle_file)
     rle_json = dumps(rle_binary)
 
     return True if rle_json == bin_json else False
 
+# import csv
+# import pprint
+
 # def convert_sum_to_obj(sum_file):
 #     sum_obj = {}
 #     sum_obj['data'] = []
 #     with(open(sum_file, "rt")) as f:
 #         reader = csv.reader(f)
 #         for n, row in enumerate(reader):
 #             if(n == 0):
```

### Comparing `haicu-0.9.1/haicu/ftdi.py` & `haicu-0.9.2/haicu/ftdi.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     if(val == None):
         # Second call fixes the data alignment
         read_status(ftdi_dev, 0)
 
     return ftdi_dev
 
 
-def list_devices() -> list:
+def list_devices() -> list[str]:
     """Get a list of available MLD1200 devices connected to host
 
     Args: None
 
     Returns:
         List containing serial number of each device found that matched the MLD1200 VID and PID
```

### Comparing `haicu-0.9.1/haicu.egg-info/PKG-INFO` & `haicu-0.9.2/haicu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.9.1
+Version: 0.9.2
 Summary: package for HAICU experiment
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.9.1/pyproject.toml` & `haicu-0.9.2/pyproject.toml`

 * *Files identical despite different names*

