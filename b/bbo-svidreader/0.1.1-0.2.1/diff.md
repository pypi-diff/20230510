# Comparing `tmp/bbo-svidreader-0.1.1.tar.gz` & `tmp/bbo-svidreader-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbo-svidreader-0.1.1.tar", last modified: Tue Feb 28 14:24:09 2023, max compression
+gzip compressed data, was "bbo-svidreader-0.2.1.tar", last modified: Wed May 10 08:27:43 2023, max compression
```

## Comparing `bbo-svidreader-0.1.1.tar` & `bbo-svidreader-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-02-28 14:24:09.580743 bbo-svidreader-0.1.1/
--rw-rw-r--   0 voit     (86501) voit     (86501)     1064 2023-02-02 10:44:18.000000 bbo-svidreader-0.1.1/LICENSE
--rw-rw-r--   0 voit     (86501) voit     (86501)      718 2023-02-28 14:24:09.580743 bbo-svidreader-0.1.1/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)       79 2023-02-02 10:44:18.000000 bbo-svidreader-0.1.1/README.md
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-02-28 14:24:09.580743 bbo-svidreader-0.1.1/bbo_svidreader.egg-info/
--rw-rw-r--   0 voit     (86501) voit     (86501)      718 2023-02-28 14:24:09.000000 bbo-svidreader-0.1.1/bbo_svidreader.egg-info/PKG-INFO
--rw-rw-r--   0 voit     (86501) voit     (86501)      263 2023-02-28 14:24:09.000000 bbo-svidreader-0.1.1/bbo_svidreader.egg-info/SOURCES.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)        1 2023-02-28 14:24:09.000000 bbo-svidreader-0.1.1/bbo_svidreader.egg-info/dependency_links.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       21 2023-02-28 14:24:09.000000 bbo-svidreader-0.1.1/bbo_svidreader.egg-info/requires.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       11 2023-02-28 14:24:09.000000 bbo-svidreader-0.1.1/bbo_svidreader.egg-info/top_level.txt
--rw-rw-r--   0 voit     (86501) voit     (86501)       38 2023-02-28 14:24:09.580743 bbo-svidreader-0.1.1/setup.cfg
--rw-rw-r--   0 voit     (86501) voit     (86501)     1060 2023-02-28 14:23:42.000000 bbo-svidreader-0.1.1/setup.py
-drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-02-28 14:24:09.580743 bbo-svidreader-0.1.1/svidreader/
--rw-rw-r--   0 voit     (86501) voit     (86501)       45 2023-02-02 14:29:16.000000 bbo-svidreader-0.1.1/svidreader/__init__.py
--rw-rw-r--   0 voit     (86501) voit     (86501)     2896 2023-02-06 15:12:30.000000 bbo-svidreader-0.1.1/svidreader/svidreader.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-05-10 08:27:43.575956 bbo-svidreader-0.2.1/
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1064 2023-02-02 10:44:18.000000 bbo-svidreader-0.2.1/LICENSE
+-rw-rw-r--   0 voit     (86501) voit     (86501)      718 2023-05-10 08:27:43.575956 bbo-svidreader-0.2.1/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)       79 2023-02-02 10:44:18.000000 bbo-svidreader-0.2.1/README.md
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-05-10 08:27:43.575956 bbo-svidreader-0.2.1/bbo_svidreader.egg-info/
+-rw-rw-r--   0 voit     (86501) voit     (86501)      718 2023-05-10 08:27:43.000000 bbo-svidreader-0.2.1/bbo_svidreader.egg-info/PKG-INFO
+-rw-rw-r--   0 voit     (86501) voit     (86501)      288 2023-05-10 08:27:43.000000 bbo-svidreader-0.2.1/bbo_svidreader.egg-info/SOURCES.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)        1 2023-05-10 08:27:43.000000 bbo-svidreader-0.2.1/bbo_svidreader.egg-info/dependency_links.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       21 2023-05-10 08:27:43.000000 bbo-svidreader-0.2.1/bbo_svidreader.egg-info/requires.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       11 2023-05-10 08:27:43.000000 bbo-svidreader-0.2.1/bbo_svidreader.egg-info/top_level.txt
+-rw-rw-r--   0 voit     (86501) voit     (86501)       38 2023-05-10 08:27:43.575956 bbo-svidreader-0.2.1/setup.cfg
+-rw-rw-r--   0 voit     (86501) voit     (86501)     1060 2023-05-10 08:27:30.000000 bbo-svidreader-0.2.1/setup.py
+drwxrwxr-x   0 voit     (86501) voit     (86501)        0 2023-05-10 08:27:43.575956 bbo-svidreader-0.2.1/svidreader/
+-rw-rw-r--   0 voit     (86501) voit     (86501)       45 2023-02-02 14:29:16.000000 bbo-svidreader-0.2.1/svidreader/__init__.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     4308 2023-05-10 08:27:30.000000 bbo-svidreader-0.2.1/svidreader/imagecache.py
+-rw-rw-r--   0 voit     (86501) voit     (86501)     3180 2023-05-10 08:27:30.000000 bbo-svidreader-0.2.1/svidreader/svidreader.py
```

### Comparing `bbo-svidreader-0.1.1/LICENSE` & `bbo-svidreader-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bbo-svidreader-0.1.1/PKG-INFO` & `bbo-svidreader-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-svidreader
-Version: 0.1.1
+Version: 0.2.1
 Summary: Video reader on top of imageio that compares returned frames to a list of hashes
 Home-page: https://github.com/bbo-lab/videoreader
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@caesar.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-svidreader-0.1.1/bbo_svidreader.egg-info/PKG-INFO` & `bbo-svidreader-0.2.1/bbo_svidreader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbo-svidreader
-Version: 0.1.1
+Version: 0.2.1
 Summary: Video reader on top of imageio that compares returned frames to a list of hashes
 Home-page: https://github.com/bbo-lab/videoreader
 Author: BBO-lab @ caesar
 Author-email: kay-michael.voit@caesar.de
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bbo-svidreader-0.1.1/setup.py` & `bbo-svidreader-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="bbo-svidreader",
-    version="0.1.1",
+    version="0.2.1",
     description="Video reader on top of imageio that compares returned frames to a list of hashes",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/bbo-lab/videoreader",
     author="BBO-lab @ caesar",
     author_email="kay-michael.voit@caesar.de",
     license="BSD",
```

### Comparing `bbo-svidreader-0.1.1/svidreader/svidreader.py` & `bbo-svidreader-0.2.1/svidreader/svidreader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 import hashlib
 import imageio.v3 as iio
+from svidreader.imagecache import ImageCache
 from ccvtools import rawio
 
 
 class SVidReader:
-    def __init__(self, video, calc_hashes=False, hash_iterator=iter):
+    def __init__(self, video, calc_hashes=False, hash_iterator=iter, cache=None):
         video = str(video)
 
         self.video = video
         self.vprops = []
         self.hashes = []
         self.last_frame = -1
         self.has_issues = False
         self.plugin = "pyav"
         self.frame_idx = 0
 
         if video[-4:] == '.ccv':
             self.plugin = None
 
         self.vprops = iio.improps(video, plugin=self.plugin)
+        self.mdata = iio.immeta(video, plugin=self.plugin)
         self.n_frames = self.vprops.shape[0]
+        self.mdata['num_frames'] = self.n_frames
 
         self.reader = iio.imopen(video, "r", plugin=self.plugin)
 
         if calc_hashes:
             for img in hash_iterator(iio.imiter(video,
                                                 plugin=self.plugin,
                                                 thread_type="FRAME",
                                                 thread_count=16
                                                 ), total=self.n_frames):
                 self.hashes.append(hashlib.md5(img).hexdigest())
 
+
+        if cache is None:
+            self.reader = ImageCache(self.reader, self.n_frames)
+        elif cache != False:
+            cache.reader = reader
+            self.reader = cache
+
+
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
     def __del__(self):
@@ -75,19 +86,16 @@
             imghash = hashlib.md5(img).hexdigest()
 
         return img
 
     def improps(self):
         return self.vprops
 
-    def get_meta_data(self, fr_idx=0):
-        mdata = {
-            'nFrames': self.n_frames
-        }
-        return mdata
+    def get_meta_data(self):
+        return self.mdata
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if (self.frame_idx + 1) < self.n_frames:
             self.frame_idx += 1
```

