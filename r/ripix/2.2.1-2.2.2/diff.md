# Comparing `tmp/ripix-2.2.1.tar.gz` & `tmp/ripix-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripix-2.2.1.tar", max compression
+gzip compressed data, was "ripix-2.2.2.tar", max compression
```

## Comparing `ripix-2.2.1.tar` & `ripix-2.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      822 2023-05-09 20:50:18.338843 ripix-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     1958 2023-05-09 19:29:45.957722 ripix-2.2.1/README.md
--rw-r--r--   0        0        0       66 2023-05-09 19:29:45.959722 ripix-2.2.1/ripix/__init__.py
--rw-r--r--   0        0        0      682 2023-05-09 19:52:26.098621 ripix-2.2.1/ripix/functions.py
--rw-r--r--   0        0        0      735 2023-05-09 19:29:45.959722 ripix-2.2.1/ripix/functions.pyi
--rw-r--r--   0        0        0     8832 2023-05-09 20:51:06.347844 ripix-2.2.1/ripix/pixel.py
--rw-r--r--   0        0        0        0 2023-05-09 19:29:45.959722 ripix-2.2.1/ripix/py.typed
--rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 ripix-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      822 2023-05-09 23:23:17.828286 ripix-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1958 2023-05-09 19:29:45.957722 ripix-2.2.2/README.md
+-rw-r--r--   0        0        0       66 2023-05-09 19:29:45.959722 ripix-2.2.2/ripix/__init__.py
+-rw-r--r--   0        0        0      682 2023-05-09 19:52:26.098621 ripix-2.2.2/ripix/functions.py
+-rw-r--r--   0        0        0      735 2023-05-09 19:29:45.959722 ripix-2.2.2/ripix/functions.pyi
+-rw-r--r--   0        0        0     8838 2023-05-09 23:22:37.762875 ripix-2.2.2/ripix/pixel.py
+-rw-r--r--   0        0        0        0 2023-05-09 19:29:45.959722 ripix-2.2.2/ripix/py.typed
+-rw-r--r--   0        0        0     2712 1970-01-01 00:00:00.000000 ripix-2.2.2/PKG-INFO
```

### Comparing `ripix-2.2.1/pyproject.toml` & `ripix-2.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ripix"
-version = "2.2.1"
+version = "2.2.2"
 description = "A Rich-compatible library for writing pixel images and ASCII art to the terminal."
 authors = ["Darren Burns <darrenb900@gmail.com>", "Romanin <semina054@gmail.com>"]
 repository = "https://github.com/romanin-rf/ripix"
 keywords = ["ripix", "rich", "textual", "image", "ascii-art", "rich_pixels"]
 readme = "README.md"
 packages = [{ include = "ripix" }]
 include = ["ripix/py.typed", "ripix/functions.pyi"]
```

### Comparing `ripix-2.2.1/README.md` & `ripix-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ripix-2.2.1/ripix/functions.py` & `ripix-2.2.2/ripix/functions.py`

 * *Files identical despite different names*

### Comparing `ripix-2.2.1/ripix/functions.pyi` & `ripix-2.2.2/ripix/functions.pyi`

 * *Files identical despite different names*

### Comparing `ripix-2.2.1/ripix/pixel.py` & `ripix-2.2.2/ripix/pixel.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         resample: Optional[Resampling] = None,
         loop: Optional[AbstractEventLoop] = None
     ) -> AsyncPixels:
         if loop is None: loop = get_running_loop()
         resample = resample or Resampling.NEAREST
         
         segments = await AsyncPixels._segments_from_image(image, resize, resample, loop)
-        return AsyncPixels.from_segments(segments)
+        return await AsyncPixels.from_segments(segments)
 
     @staticmethod
     async def from_image_path(
         path: Union[PurePath, str],
         resize: Optional[Tuple[int, int]] = None,
         resample: Optional[Resampling] = None,
         loop: Optional[AbstractEventLoop] = None
```

### Comparing `ripix-2.2.1/PKG-INFO` & `ripix-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripix
-Version: 2.2.1
+Version: 2.2.2
 Summary: A Rich-compatible library for writing pixel images and ASCII art to the terminal.
 Home-page: https://github.com/romanin-rf/ripix
 Keywords: ripix,rich,textual,image,ascii-art,rich_pixels
 Author: Darren Burns
 Author-email: darrenb900@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
```

