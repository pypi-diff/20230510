# Comparing `tmp/camerahub_tagger-0.3.3.tar.gz` & `tmp/camerahub_tagger-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub_tagger-0.3.3.tar", max compression
+gzip compressed data, was "camerahub_tagger-0.4.0.tar", max compression
```

## Comparing `camerahub_tagger-0.3.3.tar` & `camerahub_tagger-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2839 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/__init__.py
--rw-r--r--   0        0        0     2159 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/api.py
--rw-r--r--   0        0        0     2037 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/config.py
--rw-r--r--   0        0        0     6899 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/funcs.py
--rwxr-xr-x   0        0        0     7043 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/main.py
--rw-r--r--   0        0        0      670 2023-05-05 19:40:33.226040 camerahub_tagger-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 camerahub_tagger-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     2908 2023-05-10 15:05:37.952776 camerahub_tagger-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 15:05:37.952776 camerahub_tagger-0.4.0/camerahub_tagger/__init__.py
+-rw-r--r--   0        0        0     2159 2023-05-10 15:05:37.952776 camerahub_tagger-0.4.0/camerahub_tagger/api.py
+-rw-r--r--   0        0        0     2037 2023-05-10 15:05:37.952776 camerahub_tagger-0.4.0/camerahub_tagger/config.py
+-rw-r--r--   0        0        0     6899 2023-05-10 15:05:37.952776 camerahub_tagger-0.4.0/camerahub_tagger/funcs.py
+-rwxr-xr-x   0        0        0     7632 2023-05-10 15:05:37.952776 camerahub_tagger-0.4.0/camerahub_tagger/main.py
+-rw-r--r--   0        0        0      670 2023-05-10 15:06:01.837121 camerahub_tagger-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 camerahub_tagger-0.4.0/PKG-INFO
```

### Comparing `camerahub_tagger-0.3.3/README.md` & `camerahub_tagger-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,14 +56,18 @@
 
 Image file to be tagged. If not supplied, tag everything in the current directory.
 
 ### `-p --profile PROFILE`
 
 CameraHub connection profile. Default: `prod`.
 
+### `-c --clear`
+
+Clear existing EXIF metadata from the image file.
+
 ## Config
 
 CameraHub Tagger needs some basic connection details to connect to CameraHub.
 On first run, it will ask for credentials for CameraHub and save them for future use.
 
 If you need multiple profiles (e.g. if you have multiple users, or you need to connect to
 a development instance of CameraHub) you can configure the extra profiles manually by editing
```

### Comparing `camerahub_tagger-0.3.3/camerahub_tagger/api.py` & `camerahub_tagger-0.4.0/camerahub_tagger/api.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.3/camerahub_tagger/config.py` & `camerahub_tagger-0.4.0/camerahub_tagger/config.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.3/camerahub_tagger/funcs.py` & `camerahub_tagger-0.4.0/camerahub_tagger/funcs.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.3/camerahub_tagger/main.py` & `camerahub_tagger-0.4.0/camerahub_tagger/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     # Read in args
     parser = argparse.ArgumentParser()
     parser.add_argument('-r', '--recursive', help="Search for scans recursively", action='store_true')
     parser.add_argument('-a', '--auto', help="Don't prompt user to identify scans, only guess based on filename", action='store_true')
     parser.add_argument('-y', '--yes', help="Accept all changes without confirmation", action='store_true')
     parser.add_argument('-d', '--dry-run', help="Don't write any tags to image files", action='store_true')
+    parser.add_argument('-c', '--clear', help="Clear existing EXIF metadata from the image file", action='store_true')
     parser.add_argument('-f', '--file', help="Image file to be tagged. If not supplied, tag everything in the current directory.", type=str)
     parser.add_argument('-p', '--profile', help="CameraHub connection profile", default='prod', type=str)
     args = parser.parse_args()
 
     # Determine path to config file
     home = os.path.expanduser("~")
     configpath = os.path.join(home, "camerahub.ini")
@@ -77,28 +78,41 @@
     pyexiv2.set_log_level(4)
 
     # foreach found photo:
     # read exif data, check for camerahub scan tag
     for file in files:
         print(f"Processing image {file}")
 
+        # Before opening the file for reading, check if we're in Clear mode
+        if args.clear:
+            try:
+                img = pyexiv2.Image(file)
+                img.clear_exif()
+            except Exception as err: # pylint: disable=broad-exception-caught
+                cprint(f"{err} when clearing {file}", "red")
+                failed.append(file)
+            else:
+                cprint(f"Cleared metadata from {file}", "yellow")
+                changed.append(file)
+            finally:
+                img.close()
+                continue
+
         # Extract exif data from file
         try:
             img = pyexiv2.Image(file)
         except RuntimeError as err:
             cprint(f"{err} when reading {file}", "red")
             failed.append(file)
             continue
 
         try:
             existing = img.read_exif()
         except UnicodeDecodeError as err:
-            cprint(f"{err} when reading {file}", "red")
-            failed.append(file)
-            continue
+            pass
 
         img.close()
 
         # Example format
         # existing = {'Exif.Image.DateTime': '2019:06:23 19:45:17', 'Exif.Image.Artist': 'TEST', 'Exif.Image.Rating': '4', ...}
 
         if existing is not None and 'Exif.Photo.ImageUniqueID' in existing and is_valid_uuid(existing['Exif.Photo.ImageUniqueID']):
```

### Comparing `camerahub_tagger-0.3.3/pyproject.toml` & `camerahub_tagger-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camerahub-tagger"
-version = "0.3.3"
+version = "0.4.0"
 description = "EXIF tagger for CameraHub"
 authors = ["Jonathan Gazeley <me@jonathangazeley.com>"]
 repository = "https://github.com/camerahub/tagger"
 homepage = "https://camerahub.info/"
 readme = ["README.md"]
 keywords = ["EXIF", "photography", "CameraHub", "metadata"]
```

### Comparing `camerahub_tagger-0.3.3/PKG-INFO` & `camerahub_tagger-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camerahub-tagger
-Version: 0.3.3
+Version: 0.4.0
 Summary: EXIF tagger for CameraHub
 Home-page: https://camerahub.info/
 Keywords: EXIF,photography,CameraHub,metadata
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -77,14 +77,18 @@
 
 Image file to be tagged. If not supplied, tag everything in the current directory.
 
 ### `-p --profile PROFILE`
 
 CameraHub connection profile. Default: `prod`.
 
+### `-c --clear`
+
+Clear existing EXIF metadata from the image file.
+
 ## Config
 
 CameraHub Tagger needs some basic connection details to connect to CameraHub.
 On first run, it will ask for credentials for CameraHub and save them for future use.
 
 If you need multiple profiles (e.g. if you have multiple users, or you need to connect to
 a development instance of CameraHub) you can configure the extra profiles manually by editing
```

