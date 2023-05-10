# Comparing `tmp/ffmpegcv-0.2.8.tar.gz` & `tmp/ffmpegcv-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ffmpegcv-0.2.8.tar", last modified: Tue Mar 21 09:36:47 2023, max compression
+gzip compressed data, was "ffmpegcv-0.3.0.tar", last modified: Wed May 10 17:08:58 2023, max compression
```

## Comparing `ffmpegcv-0.2.8.tar` & `ffmpegcv-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,16 @@
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5754 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5565 2023-03-21 09:34:01.000000 ffmpegcv-0.2.8/README.md
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/ffmpegcv/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     7555 2022-09-25 09:27:27.000000 ffmpegcv-0.2.8/ffmpegcv/__init__.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5265 2022-05-18 13:48:31.000000 ffmpegcv-0.2.8/ffmpegcv/ffmpeg_framepick.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     9202 2022-10-18 06:28:38.000000 ffmpegcv-0.2.8/ffmpegcv/ffmpeg_reader.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5592 2022-11-01 10:37:23.000000 ffmpegcv-0.2.8/ffmpegcv/ffmpeg_reader_camera.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1685 2022-05-19 12:21:02.000000 ffmpegcv-0.2.8/ffmpegcv/ffmpeg_reader_grey.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     1474 2022-06-04 11:24:12.000000 ffmpegcv-0.2.8/ffmpegcv/ffmpeg_reader_hflip.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2618 2022-05-19 17:30:20.000000 ffmpegcv-0.2.8/ffmpegcv/ffmpeg_reader_laggy.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     3731 2023-03-21 04:52:16.000000 ffmpegcv-0.2.8/ffmpegcv/ffmpeg_writer.py
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     2878 2023-03-18 03:10:07.000000 ffmpegcv-0.2.8/ffmpegcv/video_info.py
-drwxr-xr-x   0 chenxinfeng  (1001) liying_lab  (1002)        0 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/ffmpegcv.egg-info/
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)     5754 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/ffmpegcv.egg-info/PKG-INFO
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      399 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/ffmpegcv.egg-info/SOURCES.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        1 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/ffmpegcv.egg-info/dependency_links.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)        9 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/ffmpegcv.egg-info/top_level.txt
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)       38 2023-03-21 09:36:47.000000 ffmpegcv-0.2.8/setup.cfg
--rw-r--r--   0 chenxinfeng  (1001) liying_lab  (1002)      544 2023-03-21 09:34:12.000000 ffmpegcv-0.2.8/setup.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-05-10 17:08:58.114086 ffmpegcv-0.3.0/
+-rw-r--r--   0 chen       (501) staff       (20)    11532 2023-05-10 17:08:58.113894 ffmpegcv-0.3.0/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)     9166 2023-05-10 17:04:34.000000 ffmpegcv-0.3.0/README.md
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-05-10 17:08:58.112961 ffmpegcv-0.3.0/ffmpegcv/
+-rw-r--r--   0 chen       (501) staff       (20)     7729 2023-05-09 14:16:12.000000 ffmpegcv-0.3.0/ffmpegcv/__init__.py
+-rw-r--r--   0 chen       (501) staff       (20)     9202 2023-05-09 14:16:12.000000 ffmpegcv-0.3.0/ffmpegcv/ffmpeg_reader.py
+-rw-r--r--   0 chen       (501) staff       (20)    14598 2023-05-10 17:05:37.000000 ffmpegcv-0.3.0/ffmpegcv/ffmpeg_reader_camera.py
+-rw-r--r--   0 chen       (501) staff       (20)     3731 2023-05-09 14:16:12.000000 ffmpegcv-0.3.0/ffmpegcv/ffmpeg_writer.py
+-rw-r--r--   0 chen       (501) staff       (20)     2878 2023-05-09 14:16:12.000000 ffmpegcv-0.3.0/ffmpegcv/video_info.py
+drwxr-xr-x   0 chen       (501) staff       (20)        0 2023-05-10 17:08:58.113579 ffmpegcv-0.3.0/ffmpegcv.egg-info/
+-rw-r--r--   0 chen       (501) staff       (20)    11532 2023-05-10 17:08:58.000000 ffmpegcv-0.3.0/ffmpegcv.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (501) staff       (20)      275 2023-05-10 17:08:58.000000 ffmpegcv-0.3.0/ffmpegcv.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (501) staff       (20)        1 2023-05-10 17:08:58.000000 ffmpegcv-0.3.0/ffmpegcv.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (501) staff       (20)        9 2023-05-10 17:08:58.000000 ffmpegcv-0.3.0/ffmpegcv.egg-info/top_level.txt
+-rw-r--r--   0 chen       (501) staff       (20)       38 2023-05-10 17:08:58.114137 ffmpegcv-0.3.0/setup.cfg
+-rw-r--r--   0 chen       (501) staff       (20)      544 2023-05-10 17:08:45.000000 ffmpegcv-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ffmpegcv-0.2.8/ffmpegcv/__init__.py` & `ffmpegcv-0.3.0/ffmpegcv/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,18 +230,23 @@
     """
     `ffmpegcv.VideoWriterNV` is a gpu version for `ffmpegcv.VideoWriter`.
     """
     _check_nvidia()
     return FFmpegWriterNV.VideoWriter(file, codec, fps, frameSize, pix_fmt, gpu)
 
 
-def VideoCaptureCAM(camname="OBS Virtual Camera",
-                    camsize=None,
+def VideoCaptureCAM(camname,
                     pix_fmt='bgr24',
                     crop_xywh=None,
                     resize=None,
                     resize_keepratio=True,
-                    resize_keepratioalign='center'):
-    return FFmpegReaderCAM.VideoReader(camname, camsize, pix_fmt, crop_xywh,
-        resize, resize_keepratio, resize_keepratioalign)
+                    resize_keepratioalign='center',
+                    camsize_wh=None,
+                    camfps=None,
+                    camcodec=None,
+                    campix_fmt=None):
+    return FFmpegReaderCAM.VideoReader(camname, pix_fmt, crop_xywh,
+        resize, resize_keepratio, resize_keepratioalign,
+        camsize_wh=camsize_wh, camfps=camfps, camcodec=camcodec,
+        campix_fmt=campix_fmt)
 
 VideoReaderCAM = VideoCaptureCAM
```

### Comparing `ffmpegcv-0.2.8/ffmpegcv/ffmpeg_reader.py` & `ffmpegcv-0.3.0/ffmpegcv/ffmpeg_reader.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.2.8/ffmpegcv/ffmpeg_writer.py` & `ffmpegcv-0.3.0/ffmpegcv/ffmpeg_writer.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.2.8/ffmpegcv/video_info.py` & `ffmpegcv-0.3.0/ffmpegcv/video_info.py`

 * *Files identical despite different names*

### Comparing `ffmpegcv-0.2.8/setup.py` & `ffmpegcv-0.3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='ffmpegcv', # 应用名
-    version='0.2.8', # 版本号
+    version='0.3.0', # 版本号
     packages=find_packages(include=['ffmpegcv*']), # 包括在安装包内的 Python 包
     author='chenxf',
     author_email='cxf529125853@163.com',
     url='https://pypi.org/project/ffmpegcv/',
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

