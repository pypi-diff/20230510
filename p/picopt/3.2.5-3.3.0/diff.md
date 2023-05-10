# Comparing `tmp/picopt-3.2.5.tar.gz` & `tmp/picopt-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopt-3.2.5.tar", max compression
+gzip compressed data, was "picopt-3.3.0.tar", max compression
```

## Comparing `picopt-3.2.5.tar` & `picopt-3.3.0.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0     7482 2022-12-30 00:39:44.979506 picopt-3.2.5/README.md
--rw-r--r--   0        0        0       64 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/__init__.py
--rw-r--r--   0        0        0     6503 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/cli.py
--rw-r--r--   0        0        0    11663 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/config.py
--rw-r--r--   0        0        0      254 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/config_default.yaml
--rw-r--r--   0        0        0      511 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/configurable.py
--rw-r--r--   0        0        0       25 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/__init__.py
--rw-r--r--   0        0        0     3235 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/container.py
--rw-r--r--   0        0        0     4480 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/factory.py
--rw-r--r--   0        0        0     1338 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/gif.py
--rw-r--r--   0        0        0     5554 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/handler.py
--rw-r--r--   0        0        0     2862 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/image.py
--rw-r--r--   0        0        0     1643 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/jpeg.py
--rw-r--r--   0        0        0     1892 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/png.py
--rw-r--r--   0        0        0     4284 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/webp.py
--rw-r--r--   0        0        0     4441 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/webp_animated.py
--rw-r--r--   0        0        0     3966 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/handlers/zip.py
--rw-r--r--   0        0        0     2228 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/old_timestamps.py
--rw-r--r--   0        0        0      754 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/pillow/header.py
--rwxr-xr-x   0        0        0     1042 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/pillow/png_bit_depth.py
--rwxr-xr-x   0        0        0      985 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/pillow/webp_lossless.py
--rw-r--r--   0        0        0     2950 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/stats.py
--rw-r--r--   0        0        0    14575 2022-12-30 00:39:44.983506 picopt-3.2.5/picopt/walk.py
--rw-r--r--   0        0        0     3614 2022-12-30 00:39:44.983506 picopt-3.2.5/pyproject.toml
--rw-r--r--   0        0        0      554 2022-12-30 00:39:44.983506 picopt-3.2.5/tests/__init__.py
--rw-r--r--   0        0        0       22 2022-12-30 00:39:44.983506 picopt-3.2.5/tests/integration/__init__.py
--rw-r--r--   0        0        0     2582 2022-12-30 00:39:44.983506 picopt-3.2.5/tests/integration/test_containers.py
--rw-r--r--   0        0        0     4257 2022-12-30 00:39:44.983506 picopt-3.2.5/tests/integration/test_images_dir.py
--rw-r--r--   0        0        0     2178 2022-12-30 00:39:44.983506 picopt-3.2.5/tests/integration/test_old_timestamps.py
--rw-r--r--   0        0        0     1053 2022-12-30 00:39:44.983506 picopt-3.2.5/tests/integration/test_one_container.py
--rw-r--r--   0        0        0     4183 2022-12-30 00:39:44.983506 picopt-3.2.5/tests/integration/test_timestamps.py
--rw-r--r--   0        0        0   292448 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/containers/igp-twss.epub
--rw-r--r--   0        0        0    93725 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/containers/test_cbr.cbr
--rw-r--r--   0        0        0    93408 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/containers/test_cbz.cbz
--rw-r--r--   0        0        0    93675 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/containers/test_rar.rar
--rw-r--r--   0        0        0     2974 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/containers/test_zip.zip
--rw-r--r--   0        0        0    93676 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/images/07themecamplist.pdf
--rw-r--r--   0        0        0    59640 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/images/eight.tif
--rw-r--r--   0        0        0   230578 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/images/mri.tif
--rw-r--r--   0        0        0    16383 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/images/test_animated_gif.gif
--rw-r--r--   0        0        0    63435 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/images/test_animated_png.png
--rw-r--r--   0        0        0    13610 2022-12-30 00:39:44.987506 picopt-3.2.5/tests/test_files/images/test_animated_webp.webp
--rw-r--r--   0        0        0   141430 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_bmp.bmp
--rw-r--r--   0        0        0   138952 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_gif.gif
--rw-r--r--   0        0        0    97373 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_jpg.jpg
--rw-r--r--   0        0        0     7967 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_png.png
--rw-r--r--   0        0        0     3435 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_png_16rgba.png
--rw-r--r--   0        0        0    27661 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_pnm.pnm
--rw-r--r--   0        0        0    22664 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_pre-optimized_jpg.jpg
--rw-r--r--   0        0        0   256572 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_pre-optimized_png.png
--rw-r--r--   0        0        0        6 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_txt.txt
--rw-r--r--   0        0        0     5334 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_webp_lossless.webp
--rw-r--r--   0        0        0     8914 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_webp_lossless_pre-optimized.webp
--rw-r--r--   0        0        0     2764 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_webp_lossy.webp
--rw-r--r--   0        0        0     1508 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/images/test_webp_lossy_pre-optimized.webp
--rw-r--r--   0        0        0        3 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/invalid/test_invalid_cbr.cbr
--rw-r--r--   0        0        0        3 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/invalid/test_invalid_cbz.cbz
--rw-r--r--   0        0        0        0 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/invalid/test_invalid_gif.gif
--rw-r--r--   0        0        0        0 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/invalid/test_invalid_jpg.jpg
--rw-r--r--   0        0        0        0 2022-12-30 00:39:44.991506 picopt-3.2.5/tests/test_files/invalid/test_invalid_png.png
--rw-r--r--   0        0        0   879952 2022-12-30 00:39:44.995507 picopt-3.2.5/tests/test_files/invalid/test_mpeg.mpeg
--rw-r--r--   0        0        0       80 2022-12-30 00:39:44.995507 picopt-3.2.5/tests/test_files/invalid/test_rar.rar
--rw-r--r--   0        0        0      167 2022-12-30 00:39:44.995507 picopt-3.2.5/tests/test_files/invalid/test_zip.zip
--rw-r--r--   0        0        0     1681 2022-12-30 00:39:44.995507 picopt-3.2.5/tests/unit/test_cli.py
--rw-r--r--   0        0        0      718 2022-12-30 00:39:44.995507 picopt-3.2.5/tests/unit/test_png_bit_depth.py
--rw-r--r--   0        0        0     8818 1970-01-01 00:00:00.000000 picopt-3.2.5/setup.py
--rw-r--r--   0        0        0     9059 1970-01-01 00:00:00.000000 picopt-3.2.5/PKG-INFO
+-rw-r--r--   0        0        0     7482 2023-05-10 02:40:39.342893 picopt-3.3.0/README.md
+-rw-r--r--   0        0        0       64 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/__init__.py
+-rw-r--r--   0        0        0     7124 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/cli.py
+-rw-r--r--   0        0        0    14506 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/config.py
+-rw-r--r--   0        0        0      286 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/config_default.yaml
+-rw-r--r--   0        0        0      457 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/configurable.py
+-rw-r--r--   0        0        0      501 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/data.py
+-rw-r--r--   0        0        0       25 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/__init__.py
+-rw-r--r--   0        0        0     3478 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/container.py
+-rw-r--r--   0        0        0     5508 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/factory.py
+-rw-r--r--   0        0        0     1360 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/gif.py
+-rw-r--r--   0        0        0     5667 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/handler.py
+-rw-r--r--   0        0        0     2988 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/image.py
+-rw-r--r--   0        0        0     1660 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/jpeg.py
+-rw-r--r--   0        0        0     1902 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/png.py
+-rw-r--r--   0        0        0     4294 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/webp.py
+-rw-r--r--   0        0        0     4468 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/webp_animated.py
+-rw-r--r--   0        0        0     4042 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/handlers/zip.py
+-rw-r--r--   0        0        0     2276 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/old_timestamps.py
+-rw-r--r--   0        0        0       22 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/pillow/__init__.py
+-rw-r--r--   0        0        0      777 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/pillow/header.py
+-rwxr-xr-x   0        0        0     1052 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/pillow/png_bit_depth.py
+-rwxr-xr-x   0        0        0      996 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/pillow/webp_lossless.py
+-rw-r--r--   0        0        0     2599 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/stats.py
+-rw-r--r--   0        0        0    15806 2023-05-10 02:40:39.346893 picopt-3.3.0/picopt/walk.py
+-rw-r--r--   0        0        0     4173 2023-05-10 02:40:39.346893 picopt-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-05-10 02:40:39.346893 picopt-3.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-10 02:40:39.346893 picopt-3.3.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2813 2023-05-10 02:40:39.346893 picopt-3.3.0/tests/integration/test_containers.py
+-rw-r--r--   0        0        0     4447 2023-05-10 02:40:39.346893 picopt-3.3.0/tests/integration/test_images_dir.py
+-rw-r--r--   0        0        0     2454 2023-05-10 02:40:39.346893 picopt-3.3.0/tests/integration/test_old_timestamps.py
+-rw-r--r--   0        0        0     1140 2023-05-10 02:40:39.346893 picopt-3.3.0/tests/integration/test_one_container.py
+-rw-r--r--   0        0        0     4884 2023-05-10 02:40:39.346893 picopt-3.3.0/tests/integration/test_timestamps.py
+-rw-r--r--   0        0        0   292448 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/containers/igp-twss.epub
+-rw-r--r--   0        0        0    93725 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/containers/test_cbr.cbr
+-rw-r--r--   0        0        0    93408 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/containers/test_cbz.cbz
+-rw-r--r--   0        0        0    93675 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/containers/test_rar.rar
+-rw-r--r--   0        0        0     2974 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/containers/test_zip.zip
+-rw-r--r--   0        0        0    93676 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/images/07themecamplist.pdf
+-rw-r--r--   0        0        0    59640 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/images/eight.tif
+-rw-r--r--   0        0        0   230578 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/images/mri.tif
+-rw-r--r--   0        0        0    16383 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/images/test_animated_gif.gif
+-rw-r--r--   0        0        0    63435 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/images/test_animated_png.png
+-rw-r--r--   0        0        0    13610 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/images/test_animated_webp.webp
+-rw-r--r--   0        0        0   141430 2023-05-10 02:40:39.350893 picopt-3.3.0/tests/test_files/images/test_bmp.bmp
+-rw-r--r--   0        0        0   138952 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_gif.gif
+-rw-r--r--   0        0        0    97373 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_jpg.jpg
+-rw-r--r--   0        0        0     7967 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_png.png
+-rw-r--r--   0        0        0     3435 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_png_16rgba.png
+-rw-r--r--   0        0        0    27661 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_pnm.pnm
+-rw-r--r--   0        0        0    22664 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_pre-optimized_jpg.jpg
+-rw-r--r--   0        0        0   256572 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_pre-optimized_png.png
+-rw-r--r--   0        0        0        6 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_txt.txt
+-rw-r--r--   0        0        0     5334 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_webp_lossless.webp
+-rw-r--r--   0        0        0     8914 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_webp_lossless_pre-optimized.webp
+-rw-r--r--   0        0        0     2764 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_webp_lossy.webp
+-rw-r--r--   0        0        0     1508 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/images/test_webp_lossy_pre-optimized.webp
+-rw-r--r--   0        0        0        3 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/invalid/test_invalid_cbr.cbr
+-rw-r--r--   0        0        0        3 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/invalid/test_invalid_cbz.cbz
+-rw-r--r--   0        0        0        0 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/invalid/test_invalid_gif.gif
+-rw-r--r--   0        0        0        0 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/invalid/test_invalid_jpg.jpg
+-rw-r--r--   0        0        0        0 2023-05-10 02:40:39.354893 picopt-3.3.0/tests/test_files/invalid/test_invalid_png.png
+-rw-r--r--   0        0        0   879952 2023-05-10 02:40:39.358893 picopt-3.3.0/tests/test_files/invalid/test_mpeg.mpeg
+-rw-r--r--   0        0        0       80 2023-05-10 02:40:39.358893 picopt-3.3.0/tests/test_files/invalid/test_rar.rar
+-rw-r--r--   0        0        0      167 2023-05-10 02:40:39.358893 picopt-3.3.0/tests/test_files/invalid/test_zip.zip
+-rw-r--r--   0        0        0       18 2023-05-10 02:40:39.358893 picopt-3.3.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1923 2023-05-10 02:40:39.358893 picopt-3.3.0/tests/unit/test_cli.py
+-rw-r--r--   0        0        0      871 2023-05-10 02:40:39.358893 picopt-3.3.0/tests/unit/test_png_bit_depth.py
+-rw-r--r--   0        0        0     9059 1970-01-01 00:00:00.000000 picopt-3.3.0/PKG-INFO
```

### Comparing `picopt-3.2.5/README.md` & `picopt-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/picopt/cli.py` & `picopt-3.3.0/picopt/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-#!/usr/bin/env python3
 """Run pictures through image specific external optimizers."""
 import argparse
-
+import sys
 from argparse import Action, Namespace, RawDescriptionHelpFormatter
 from importlib.metadata import PackageNotFoundError, version
 from typing import Optional
 
-from termcolor import colored
+from termcolor import colored, cprint
 
 from picopt import PROGRAM_NAME, walk
-from picopt.config import ALL_FORMATS, DEFAULT_HANDLERS, get_config
+from picopt.config import ALL_FORMAT_STRS, DEFAULT_HANDLERS, get_config
 from picopt.handlers.png import Png
 from picopt.handlers.webp import WebP
 from picopt.handlers.zip import CBZ, Zip
 
-
-DEFAULT_FORMATS = frozenset(
-    [handler_cls.OUTPUT_FORMAT for handler_cls in DEFAULT_HANDLERS]
+DEFAULT_FORMAT_STRS = frozenset(
+    [handler_cls.OUTPUT_FORMAT_STR for handler_cls in DEFAULT_HANDLERS]
 )
-EXTRA_FORMATS = ALL_FORMATS - DEFAULT_FORMATS
+EXTRA_FORMAT_STRS = ALL_FORMAT_STRS - DEFAULT_FORMAT_STRS
 FORMAT_DELIMETER = ","
 try:
     VERSION = version(PROGRAM_NAME)
 except PackageNotFoundError:
     VERSION = "test"
 
 
 class SplitArgsAction(Action):
     """Convert csv string from argparse to a list."""
 
-    def __call__(self, parser, namespace, values, _option_string=None):
+    def __call__(self, _parser, namespace, values, _option_string=None):
         """Split values string into list."""
         if isinstance(values, str):
             values = tuple(sorted(values.strip().split(FORMAT_DELIMETER)))
         setattr(namespace, self.dest, values)
 
 
 def _comma_join(formats: frozenset[str]) -> str:
@@ -88,33 +86,34 @@
     )
     parser.add_argument(
         "-f",
         "--formats",
         action=SplitArgsAction,
         dest="formats",
         help="Only optimize images of the specified "
-        f"'{FORMAT_DELIMETER}' delimited formats from: {_comma_join(ALL_FORMATS)}. "
-        f"Defaults to {_comma_join(DEFAULT_FORMATS)}",
+        f"'{FORMAT_DELIMETER}' delimited formats from: {_comma_join(ALL_FORMAT_STRS)}. "
+        f"Defaults to {_comma_join(DEFAULT_FORMAT_STRS)}",
     )
     parser.add_argument(
         "-x",
         "--extra-formats",
         action=SplitArgsAction,
-        dest="_extra_formats",
+        dest="extra_formats",
         help="Append additional formats to the default formats.",
     )
     parser.add_argument(
         "-c",
         "--convert-to",
         action=SplitArgsAction,
         dest="convert_to",
-        help="A list of formats to convert to. Lossless images may convert to "
-        f"{Png.OUTPUT_FORMAT} or {WebP.OUTPUT_FORMAT}. {Zip.INPUT_FORMAT_RAR} archives "
-        f"may convert to {Zip.OUTPUT_FORMAT} or {CBZ.OUTPUT_FORMAT}. "
-        "By default formats are not converted to other formats.",
+        help="A list of formats to convert to. Lossless images may convert to"
+        f" {Png.OUTPUT_FORMAT_STR} or {WebP.OUTPUT_FORMAT_STR}."
+        f" {Zip.INPUT_FORMAT_STR_RAR} archives"
+        f" may convert to {Zip.OUTPUT_FORMAT_STR} or {CBZ.OUTPUT_FORMAT_STR}."
+        " By default formats are not converted to other formats.",
     )
     parser.add_argument(
         "-S",
         "--no-symlinks",
         action="store_false",
         dest="symlinks",
         help="Do not follow symlinks for files and directories",
@@ -138,14 +137,22 @@
         "--timestamps",
         action="store_true",
         dest="timestamps",
         help="Record the optimization time in a timestamps file. "
         "Do not optimize files that are older than their timestamp record.",
     )
     parser.add_argument(
+        "-N",
+        "--timestamps-no-check-config",
+        dest="timestamps_check_config",
+        action="store_false",
+        default=True,
+        help="Do not compare program config options with loaded timestamps.",
+    )
+    parser.add_argument(
         "-A",
         "--after",
         action="store",
         dest="after",
         help="Only optimize files after the specified timestamp. "
         "Supersedes recorded timestamp files. Can be an epoch number or "
         "datetime string",
@@ -208,23 +215,33 @@
         help="File or directory paths to optimize",
     )
 
     if params is not None:
         params = params[1:]
 
     pns = parser.parse_args(params)
+
+    # Move extra_formats to computed namespace
+    pns.computed = Namespace(extra_formats=pns.extra_formats)
+    delattr(pns, "extra_formats")
+
+    # increment verbose
     if pns.verbose is not None and pns.verbose > 0:
         pns.verbose += 1
+
     return Namespace(picopt=pns)
 
 
 def main(args: Optional[tuple[str, ...]] = None) -> bool:
     """Process command line arguments and walk inputs."""
-    arguments = get_arguments(args)
-
-    config = get_config(arguments)
-    wob = walk.Walk(config)
-    return wob.run()
+    try:
+        arguments = get_arguments(args)
 
+        config = get_config(arguments)
+        wob = walk.Walk(config)
+        return wob.run()
+    except Exception as exc:
+        cprint(f"ERROR: {exc}", "red")
+        import traceback
 
-if __name__ == "__main__":
-    main()
+        traceback.print_exception(exc)
+        sys.exit(1)
```

### Comparing `picopt-3.2.5/picopt/handlers/container.py` & `picopt-3.3.0/picopt/handlers/container.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,110 @@
 """Optimize comic archives."""
 import shutil
-
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from typing import Optional, Union
 
 from confuse.templates import AttrDict
+from termcolor import cprint
 
-from picopt.handlers.handler import Format, Handler, Metadata
+from picopt.data import PathInfo, ReportInfo
+from picopt.handlers.handler import FileFormat, Handler, Metadata
 from picopt.stats import ReportStats
 
 
 class ContainerHandler(Handler, metaclass=ABCMeta):
     """Comic format class."""
 
     CONTAINER_DIR_SUFFIX: str = ".dir"
     CONVERT: bool = True
 
     @classmethod
     @abstractmethod
-    def identify_format(cls, path: Path) -> Optional[Format]:
+    def identify_format(cls, path: Path) -> Optional[FileFormat]:
         """Return the format if this handler can handle this path."""
-        pass
 
     @abstractmethod
     def unpack_into(self) -> None:
         """Unpack a container into a tmp dir to work on it's contents."""
-        pass
 
     @abstractmethod
     def pack_into(self, working_path: Path) -> None:
         """Create a container from a tmp dir's contents."""
-        pass
 
     def __init__(
         self,
         config: AttrDict,
-        original_path: Path,
-        format: Format,
+        path_info: PathInfo,
+        file_format: FileFormat,
         metadata: Metadata,
-        is_case_sensitive: bool,
     ):
         """Unpack a container with a subclass's unpacker."""
-        super().__init__(config, original_path, format, metadata, is_case_sensitive)
+        super().__init__(
+            config,
+            path_info,
+            file_format,
+            metadata,
+        )
         self.comment: Optional[bytes] = None
         self.tmp_container_dir: Path = Path(
             str(self.get_working_path()) + self.CONTAINER_DIR_SUFFIX
         )
 
     def unpack(self) -> Union[Handler, ReportStats]:
         """Create directory and unpack container."""
         try:
             if self.config.verbose:
-                print(f"Unpacking {self.original_path}...", end="")
+                cprint(f"Unpacking {self.original_path}...", end="")
 
             # create a clean tmpdir
             if self.tmp_container_dir.exists():
                 shutil.rmtree(self.tmp_container_dir)
             self.tmp_container_dir.mkdir(parents=True)
 
             # extract archive into the tmpdir
             self.unpack_into()
 
             if self.config.verbose:
-                print("done")
-            return self
+                cprint("done")
         except Exception as exc:
             return self.error(exc)
+        return self
 
     def cleanup_after_optimize(self, working_path: Path) -> tuple[int, int]:
         """Clean up the temp dir as well as the old container."""
         if self.config.verbose:
-            print(".", end="")
+            cprint(".", end="")
         shutil.rmtree(self.tmp_container_dir)
 
         if self.config.verbose:
-            print(".", end="")
+            cprint(".", end="")
         bytes_count = super().cleanup_after_optimize(working_path)
 
         if self.config.verbose:
-            print("done.")
+            cprint("done.")
         return bytes_count
 
     def repack(self) -> ReportStats:
         """Create a new container and clean up the tmp dir."""
+        new_path = self.get_working_path()
         try:
             # archive into new filename
-            new_path = self.get_working_path()
             if self.config.verbose:
-                print(f"Repacking {self.final_path}", end="")
+                cprint(f"Repacking {self.final_path}", end="")
             self.pack_into(new_path)
 
             bytes_count = self.cleanup_after_optimize(new_path)
-            report_stats = ReportStats(
-                self.final_path, bytes_count, self.config.test, self.convert
+            info = ReportInfo(
+                self.final_path,
+                self.convert,
+                self.config.test,
+                bytes_count[0],
+                bytes_count[1],
             )
+            report_stats = ReportStats(info)
             if self.config.verbose:
                 report_stats.report()
-            return report_stats
         except Exception as exc:
+            shutil.rmtree(self.tmp_container_dir, ignore_errors=True)
             return self.error(exc)
+        return report_stats
```

### Comparing `picopt-3.2.5/picopt/handlers/factory.py` & `picopt-3.3.0/picopt/handlers/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,130 +1,158 @@
 """Return a handler for a path."""
 from pathlib import Path
-from typing import Optional, Type
+from typing import Optional
 
 from confuse.templates import AttrDict
 from PIL import Image, UnidentifiedImageError
 from termcolor import cprint
 
-from picopt.config import WEBP_CONVERTABLE_FORMATS
+from picopt.config import WEBP_CONVERTABLE_FORMAT_STRS
+from picopt.data import PathInfo
 from picopt.handlers.container import ContainerHandler
-from picopt.handlers.handler import Format, Handler, Metadata
-from picopt.handlers.image import TIFF_FORMAT
+from picopt.handlers.handler import FileFormat, Handler, Metadata
+from picopt.handlers.image import TIFF_FORMAT_STR
 from picopt.handlers.webp import WebPLossless
 from picopt.handlers.zip import CBZ, EPub, Zip
 from picopt.pillow.webp_lossless import is_lossless
 
-
-_ALWAYS_LOSSLESS_FORMATS = WEBP_CONVERTABLE_FORMATS - set([TIFF_FORMAT])
-_CONTAINER_HANDLERS: tuple[Type[ContainerHandler], ...] = (CBZ, Zip, EPub)
+_ALWAYS_LOSSLESS_FORMAT_STRS = WEBP_CONVERTABLE_FORMAT_STRS - {TIFF_FORMAT_STR}
+_CONTAINER_HANDLERS: tuple[type[ContainerHandler], ...] = (CBZ, Zip, EPub)
 
 
 def _is_lossless(image_format: str, path: Path, info: dict) -> bool:
     """Determine if image format is lossless."""
-    if image_format in _ALWAYS_LOSSLESS_FORMATS:
+    if image_format in _ALWAYS_LOSSLESS_FORMAT_STRS:
         lossless = True
-    elif image_format == WebPLossless.OUTPUT_FORMAT:
+    elif image_format == WebPLossless.OUTPUT_FORMAT_STR:
         lossless = is_lossless(str(path))
-    elif image_format == TIFF_FORMAT:
+    elif image_format == TIFF_FORMAT_STR:
         lossless = info.get("compression") != "jpeg"
     else:
         lossless = False
     return lossless
 
 
-def _get_image_format(
-    path: Path, keep_metadata: bool
-) -> tuple[Optional[Format], Metadata]:
-    """Construct the image format with PIL."""
-    format = None
-    metadata = Metadata()
+def _extract_image_info(path, keep_metadata):
+    """Get image format and info from a file."""
+    image_format_str = None
+    info = {}
     n_frames = 1
+    animated = False
     try:
         with Image.open(path, mode="r") as image:
             image.verify()
         image.close()  # for animated images
         with Image.open(path, mode="r") as image:
-            image_format = image.format
-            if image_format is None:
-                raise UnidentifiedImageError("No image format")
-            animated = getattr(image, "is_animated", False)
-            info = image.info
-            if keep_metadata and animated:
-                n_frames = getattr(image, "n_frames", 1)
+            image_format_str = image.format
+            if image_format_str:
+                animated = getattr(image, "is_animated", False)
+                info = image.info
+                if keep_metadata and animated:
+                    n_frames = getattr(image, "n_frames", 1)
         image.close()  # for animated images
+    except UnidentifiedImageError:
+        pass
+    return image_format_str, info, n_frames, animated
+
+
+def _get_image_format(
+    path: Path, keep_metadata: bool
+) -> tuple[Optional[FileFormat], Metadata]:
+    """Construct the image format with PIL."""
+    image_format_str, info, n_frames, animated = _extract_image_info(
+        path, keep_metadata
+    )
+
+    file_format = None
+    metadata = Metadata()
+    if image_format_str:
         if keep_metadata:
             exif = info.get("exif", b"")
             icc = info.get("icc_profile", "")
             metadata = Metadata(exif, icc, n_frames)
-        lossless = _is_lossless(image_format, path, info)
-        format = Format(image_format, lossless, animated)
-    except UnidentifiedImageError:
-        pass
-    return format, metadata
+        lossless = _is_lossless(image_format_str, path, info)
+        file_format = FileFormat(image_format_str, lossless, animated)
+    return file_format, metadata
 
 
-def _get_container_format(path: Path) -> Optional[Format]:
+def _get_container_format(path: Path) -> Optional[FileFormat]:
     """Get the container format by querying each handler."""
-    format = None
+    file_format = None
     for container_handler in _CONTAINER_HANDLERS:
-        format = container_handler.identify_format(path)
-        if format is not None:
+        file_format = container_handler.identify_format(path)
+        if file_format is not None:
             break
-    return format
+    return file_format
 
 
 def _get_handler_class(
-    config: AttrDict, key: str, format: Format
-) -> Optional[Type[Handler]]:
-    handler_classes = config._format_handlers.get(format)
-    if handler_classes:
-        handler_cls = handler_classes.get(key)
-    else:
-        handler_cls = None
+    config: AttrDict, key: str, file_format: FileFormat
+) -> Optional[type[Handler]]:
+    handler_classes = config.computed.format_handlers.get(file_format)
+    return handler_classes.get(key) if handler_classes else None
+
+
+def _create_handler_get_format(
+    config: AttrDict, path: Path
+) -> tuple[Optional[FileFormat], Metadata]:
+    file_format, metadata = _get_image_format(path, config.keep_metadata)
+    if not file_format:
+        file_format = _get_container_format(path)
+    return file_format, metadata
+
+
+def _create_handler_get_handler_class(
+    config: AttrDict, convert: bool, file_format: Optional[FileFormat]
+) -> Optional[type[Handler]]:
+    handler_cls: Optional[type[Handler]] = None
+    if not file_format:
+        return handler_cls
+    if convert:
+        handler_cls = _get_handler_class(config, "convert", file_format)
+    if not handler_cls:
+        handler_cls = _get_handler_class(config, "native", file_format)
     return handler_cls
 
 
-def create_handler(
-    config: AttrDict, path: Path, is_case_sensitive: bool, convert: bool = True
-) -> Optional[Handler]:
+def _create_handler_no_handler_class(
+    config: AttrDict, path: Path, file_format: Optional[FileFormat]
+) -> None:
+    if config.verbose > 1 and not config.list_only:
+        if file_format:
+            fmt = file_format.format_str
+            if file_format.lossless:
+                fmt += " lossless"
+            else:
+                fmt += " lossy"
+            if file_format.animated:
+                fmt += " animated"
+        else:
+            fmt = "unknown"
+        cprint(
+            f"Skipped {path}: ({fmt}) is not an enabled image or container.",
+            "white",
+            attrs=["dark"],
+        )
+    else:
+        cprint(".", "white", attrs=["dark"], end="")
+
+
+def create_handler(config: AttrDict, path_info: PathInfo) -> Optional[Handler]:
     """Get the image format."""
     # This is the consumer of config._format_handlers
-    format: Optional[Format] = None
+    file_format: Optional[FileFormat] = None
     metadata: Metadata = Metadata()
-    handler_cls: Optional[Type[Handler]] = None
+    handler_cls: Optional[type[Handler]] = None
     try:
-        format, metadata = _get_image_format(path, config.keep_metadata)
-        if not format:
-            format = _get_container_format(path)
-
-        if format:
-            if convert:
-                handler_cls = _get_handler_class(config, "convert", format)
-            if not handler_cls:
-                handler_cls = _get_handler_class(config, "native", format)
+        file_format, metadata = _create_handler_get_format(config, path_info.path)
+        handler_cls = _create_handler_get_handler_class(
+            config, path_info.convert, file_format
+        )
     except OSError as exc:
-        cprint("WARNING: getting handler", str(exc), "yellow")
+        cprint(f"WARNING: getting handler {exc}", "yellow")
 
-    if handler_cls and format is not None:
-        handler = handler_cls(config, path, format, metadata, is_case_sensitive)
+    if handler_cls and file_format is not None:
+        handler = handler_cls(config, path_info, file_format, metadata)
     else:
-        if config.verbose > 1 and not config.list_only:
-            if format:
-                fmt = format.format
-                if format.lossless:
-                    fmt += " lossless"
-                else:
-                    fmt += " lossy"
-                if format.animated:
-                    fmt += " animated"
-            else:
-                fmt = "unknown"
-            cprint(
-                f"Skipped {path}: ({fmt}) is not an enabled image or container.",
-                "white",
-                attrs=["dark"],
-            )
-        else:
-            cprint(".", "white", attrs=["dark"], end="")
-        handler = None
+        handler = _create_handler_no_handler_class(config, path_info.path, file_format)
     return handler
```

### Comparing `picopt-3.2.5/picopt/handlers/gif.py` & `picopt-3.3.0/picopt/handlers/jpeg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-"""Gif format."""
-import shutil
-
+"""JPEG format."""
+from copy import copy
 from pathlib import Path
 from typing import Optional
 
-from PIL import Image
-from PIL.GifImagePlugin import GifImageFile
+from PIL.JpegImagePlugin import JpegImageFile
 
-from picopt.handlers.handler import Format
+from picopt.handlers.handler import FileFormat
 from picopt.handlers.image import ImageHandler
 
 
-class Gif(ImageHandler):
-    """GIF handler."""
+class Jpeg(ImageHandler):
+    """JPEG format class."""
 
-    OUTPUT_FORMAT = GifImageFile.format
-    OUTPUT_FORMAT_OBJ = Format(OUTPUT_FORMAT, True, False)
+    OUTPUT_FORMAT_STR = JpegImageFile.format
+    OUTPUT_FILE_FORMAT = FileFormat(OUTPUT_FORMAT_STR, False, False)
     PROGRAMS: dict[str, Optional[str]] = ImageHandler.init_programs(
-        ("gifsicle", "pil2gif")
+        ("mozjpeg", "jpegtran")
     )
-    _ARGS_PREFIX = [
-        PROGRAMS["gifsicle"],
-        "--optimize=3",
-        "--batch",
-    ]
-
-    def gifsicle(self, old_path: Path, new_path: Path) -> Path:
-        """Return gifsicle args."""
-        if not self._ARGS_PREFIX[0]:
+    _ARGS_PREFIX = ["-optimize", "-progressive", "-copy"]
+    _MOZJPEG_ARGS_PREFIX = [PROGRAMS["mozjpeg"], *_ARGS_PREFIX]
+    _JPEGTRAN_ARGS_PREFIX = [PROGRAMS["jpegtran"], *_ARGS_PREFIX]
+
+    @classmethod
+    def _output_suffix(cls) -> str:
+        """JPEG suffix does not match format."""
+        return "jpg"
+
+    def _jpegtran(self, args: list[str], old_path: Path, new_path: Path) -> Path:
+        """Run the jpegtran type program."""
+        args = copy(args)
+        if not bin:
             return old_path
-
-        shutil.copy2(old_path, new_path)
-        args = tuple(self._ARGS_PREFIX + [str(new_path)])
-        self.run_ext(args)
-        return new_path
-
-    def pil2gif(self, old_path: Path, new_path: Path) -> Path:
-        """Pillow gif optimization."""
-        with Image.open(old_path) as image:
-            image.save(new_path, self.OUTPUT_FORMAT, optimize=True, save_all=True)
-        image.close()  # for animated images
+        if self.config.keep_metadata:
+            args += ["all"]
+        else:
+            args += ["none"]
+        args += ["-outfile", str(new_path), str(old_path)]
+        args_t = tuple(args)
+        self.run_ext(args_t)
         return new_path
 
-
-class AnimatedGif(Gif):
-    """Animated GIF handler."""
-
-    OUTPUT_FORMAT_OBJ = Format(Gif.OUTPUT_FORMAT, True, True)
+    def mozjpeg(self, old_path: Path, new_path: Path) -> Path:
+        """Create argument list for mozjpeg."""
+        return self._jpegtran(self._MOZJPEG_ARGS_PREFIX, old_path, new_path)
+
+    def jpegtran(self, old_path: Path, new_path: Path) -> Path:
+        """Create argument list for jpegtran."""
+        return self._jpegtran(self._JPEGTRAN_ARGS_PREFIX, old_path, new_path)
```

### Comparing `picopt-3.2.5/picopt/handlers/handler.py` & `picopt-3.3.0/picopt/handlers/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """FileType abstract class for image and container formats."""
 import shutil
 import subprocess
-
 from abc import ABC
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 
 from confuse.templates import AttrDict
 from termcolor import cprint
 
 from picopt import PROGRAM_NAME
+from picopt.data import PathInfo, ReportInfo
 from picopt.stats import ReportStats
 
 
 @dataclass(eq=True, frozen=True)
-class Format:
+class FileFormat:
     """A file format, with image attributes."""
 
-    format: str
+    format_str: str
     lossless: bool = True
     animated: bool = False
 
 
 @dataclass(eq=True, frozen=True)
 class Metadata:
     """Image metadata class."""
@@ -32,16 +32,16 @@
     n_frames: int = 1
 
 
 class Handler(ABC):
     """FileType superclass for image and container formats."""
 
     BEST_ONLY: bool = True
-    OUTPUT_FORMAT: str = "unimplemented"
-    OUTPUT_FORMAT_OBJ: Format = Format(OUTPUT_FORMAT, False, False)
+    OUTPUT_FORMAT_STR: str = "unimplemented"
+    OUTPUT_FILE_FORMAT: FileFormat = FileFormat(OUTPUT_FORMAT_STR, False, False)
     INTERNAL: str = "python_internal"
     PROGRAMS: dict[str, Optional[str]] = {}
     WORKING_SUFFIX: str = f"{PROGRAM_NAME}__tmp"
 
     @classmethod
     def init_programs(cls, programs: tuple[str, ...]) -> dict[str, Optional[str]]:
         """Initialize the PROGRAM map."""
@@ -53,70 +53,70 @@
             program_dict[program] = bin_path
         return program_dict
 
     @staticmethod
     def run_ext(args: tuple[str, ...]) -> None:
         """Run EXTERNAL program."""
         if not args[0]:
-            raise ValueError(f"{args}")
+            msg = f"{args}"
+            raise ValueError(msg)
         subprocess.run(
-            args,
+            args,  # noqa S603
             check=True,
             text=True,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.PIPE,
         )
 
     @classmethod
-    def native_input_format_objs(cls) -> set[Format]:
+    def native_input_file_formats(cls) -> set[FileFormat]:
         """Return input formats handled without conversion."""
-        return set([cls.OUTPUT_FORMAT_OBJ])
+        return {cls.OUTPUT_FILE_FORMAT}
 
     @classmethod
     def _output_suffix(cls) -> str:
         """Return the suffix without a leading dot."""
-        return cls.OUTPUT_FORMAT.lower()
+        return cls.OUTPUT_FORMAT_STR.lower()
 
     @classmethod
     def output_suffix(cls) -> str:
         """Generate the output suffix for the handler."""
         return "." + cls._output_suffix()
 
     @classmethod
     def is_handler_available(
         cls,
         convert_handlers: dict,
         available_programs: set,
-        format_obj: Format,
+        file_format: FileFormat,
     ):
         """Can this handler run with available programs."""
-        handled_format_objs = cls.native_input_format_objs() | convert_handlers.get(
+        handled_file_formats = cls.native_input_file_formats() | convert_handlers.get(
             cls, set()
         )
-        return format_obj in handled_format_objs and bool(
+        return file_format in handled_file_formats and bool(
             available_programs & set(cls.PROGRAMS.keys())
         )
 
     def __init__(
         self,
         config: AttrDict,
-        original_path: Path,
-        input_format_obj: Format,
+        path_info: PathInfo,
+        input_file_format: FileFormat,
         metadata: Metadata,
-        is_case_sensitive: bool,
     ):
         """Initialize handler."""
         self.config: AttrDict = config
-        self.original_path: Path = original_path
+        self.original_path: Path = path_info.path
         self.working_paths: set[Path] = set()
         self.final_path: Path = self.original_path.with_suffix(self.output_suffix())
-        self.input_format_obj: Format = input_format_obj
+        self.input_file_format: FileFormat = input_file_format
         self.metadata = metadata
-        self.convert = input_format_obj != self.OUTPUT_FORMAT_OBJ
-        self.is_case_sensitive = is_case_sensitive
+        self.convert = input_file_format != self.OUTPUT_FILE_FORMAT
+        self.is_case_sensitive = path_info.is_case_sensitive
 
     def get_working_path(self, identifier: str = "") -> Path:
         """Return a working path with a custom suffix."""
         suffixes = [self.original_path.suffix, self.WORKING_SUFFIX]
         if identifier:
             suffixes += [identifier]
         suffixes += [self._output_suffix()]
@@ -156,10 +156,9 @@
             cprint(f"ERROR: cleanup_after_optimize: {exc}", "red")
             raise
 
         return (bytes_in, bytes_out)
 
     def error(self, exc: Exception) -> ReportStats:
         """Return an error result."""
-        return ReportStats(
-            self.original_path, None, self.config.test, self.convert, exc=exc
-        )
+        info = ReportInfo(self.original_path, self.convert, self.config.test, exc=exc)
+        return ReportStats(info)
```

### Comparing `picopt-3.2.5/picopt/handlers/image.py` & `picopt-3.3.0/picopt/handlers/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,89 @@
-"""Format Superclass."""
+"""FileFormat Superclass."""
 from abc import ABCMeta
 from pathlib import Path
 from typing import Any
 
 from PIL import Image
 from PIL.BmpImagePlugin import BmpImageFile
 from PIL.PngImagePlugin import PngImageFile
 from PIL.PpmImagePlugin import PpmImageFile
 from PIL.TiffImagePlugin import TiffImageFile
 
-from picopt.handlers.handler import Format, Handler
+from picopt.data import ReportInfo
+from picopt.handlers.handler import FileFormat, Handler
 from picopt.stats import ReportStats
 
-
-PPM_FORMAT_OBJ = Format(PpmImageFile.format, True, False)
-BPM_FORMAT_OBJ = Format(BmpImageFile.format, True, False)
-CONVERTABLE_FORMAT_OBJS = set((BPM_FORMAT_OBJ, PPM_FORMAT_OBJ))
-CONVERTABLE_FORMATS = set([format.format for format in CONVERTABLE_FORMAT_OBJS])
-PNG_ANIMATED_FORMAT_OBJ = Format(PngImageFile.format, True, True)
-TIFF_FORMAT = TiffImageFile.format
-TIFF_FORMAT_OBJ = Format(TIFF_FORMAT, True, False)
-TIFF_ANIMATED_FORMAT_OBJ = Format(TIFF_FORMAT, True, True)
-_NATIVE_ONLY_FORMATS = set(
-    (PNG_ANIMATED_FORMAT_OBJ, TIFF_ANIMATED_FORMAT_OBJ, TIFF_FORMAT_OBJ)
-)
+PPM_FILE_FORMAT = FileFormat(PpmImageFile.format, True, False)
+BPM_FILE_FORMAT = FileFormat(BmpImageFile.format, True, False)
+CONVERTABLE_FILE_FORMATS = {BPM_FILE_FORMAT, PPM_FILE_FORMAT}
+CONVERTABLE_FORMAT_STRS = {
+    img_format.format_str for img_format in CONVERTABLE_FILE_FORMATS
+}
+PNG_ANIMATED_FILE_FORMAT = FileFormat(PngImageFile.format, True, True)
+TIFF_FORMAT_STR = TiffImageFile.format
+TIFF_FILE_FORMAT = FileFormat(TIFF_FORMAT_STR, True, False)
+TIFF_ANIMATED_FILE_FORMAT = FileFormat(TIFF_FORMAT_STR, True, True)
+_NATIVE_ONLY_FILE_FORMATS = {
+    PNG_ANIMATED_FILE_FORMAT,
+    TIFF_ANIMATED_FILE_FORMAT,
+    TIFF_FILE_FORMAT,
+}
 
 
 class ImageHandler(Handler, metaclass=ABCMeta):
-    """Format superclass."""
+    """Image Handler superclass."""
 
     PIL2_ARGS: dict[str, Any] = {}
     PREFERRED_PROGRAM: str = "unimplemented"
 
     def _optimize_with_progs(self) -> ReportStats:
-        """
-        Use the correct optimizing functions in sequence.
+        """Use the correct optimizing functions in sequence.
 
         And report back statistics.
         """
         path = self.original_path
-        for func in self.PROGRAMS.keys():
+        for func in self.PROGRAMS:
             if path != self.original_path:
                 self.working_paths.add(path)
             new_path = self.get_working_path(func)
             path = getattr(self, func)(path, new_path)
             if self.BEST_ONLY:
                 break
 
         bytes_count = self.cleanup_after_optimize(path)
-        report_stats = ReportStats(
-            self.final_path, bytes_count, self.config.test, self.convert
+        info = ReportInfo(
+            self.final_path,
+            self.convert,
+            self.config.test,
+            bytes_count[0],
+            bytes_count[1],
         )
-
-        return report_stats
+        return ReportStats(info)
 
     def optimize_image(self) -> ReportStats:
         """Optimize a given image from a filename."""
         try:
             report_stats = self._optimize_with_progs()
             if self.config.verbose:
                 report_stats.report()
         except Exception as exc:
             report_stats = self.error(exc)
         return report_stats
 
     def pil2native(self, old_path: Path, new_path: Path) -> Path:
         """Use PIL to save the image."""
         if (
-            self.input_format_obj in _NATIVE_ONLY_FORMATS
-            or self.PREFERRED_PROGRAM not in self.config._available_programs
+            self.input_file_format not in _NATIVE_ONLY_FILE_FORMATS
+            and self.PREFERRED_PROGRAM in self.config.computed.available_programs
         ):
-            with Image.open(old_path) as image:
-                image.save(
-                    new_path,
-                    self.OUTPUT_FORMAT,
-                    exif=self.metadata.exif,
-                    icc_profile=self.metadata.icc_profile,
-                    **self.PIL2_ARGS,
-                )
-            image.close()  # for animated images
-        else:
-            new_path = old_path
+            return old_path
+        with Image.open(old_path) as image:
+            image.save(
+                new_path,
+                self.OUTPUT_FORMAT_STR,
+                exif=self.metadata.exif,
+                icc_profile=self.metadata.icc_profile,
+                **self.PIL2_ARGS,
+            )
+        image.close()  # for animated images
         return new_path
```

### Comparing `picopt-3.2.5/picopt/handlers/png.py` & `picopt-3.3.0/picopt/handlers/png.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from copy import copy
 from pathlib import Path
 from typing import Optional
 
 from PIL.PngImagePlugin import PngImageFile
 from termcolor import cprint
 
-from picopt.handlers.handler import Format
+from picopt.handlers.handler import FileFormat
 from picopt.handlers.image import ImageHandler
 from picopt.pillow.png_bit_depth import png_bit_depth
 
 
 class Png(ImageHandler):
     """PNG format class."""
 
     BEST_ONLY: bool = False
-    OUTPUT_FORMAT = PngImageFile.format
-    OUTPUT_FORMAT_OBJ = Format(OUTPUT_FORMAT, True, False)
+    OUTPUT_FORMAT_STR = PngImageFile.format
+    OUTPUT_FILE_FORMAT = FileFormat(OUTPUT_FORMAT_STR, True, False)
     PIL2_ARGS: dict[str, bool] = {"optimize": True}
     PROGRAMS: dict[str, Optional[str]] = ImageHandler.init_programs(
         ("pil2png", "optipng", "pngout")
     )
     PREFERRED_PROGRAM: str = "optipng"
     _OPTIPNG_ARGS = [PROGRAMS["optipng"], "-o5", "-fix", "-force"]
     _PNGOUT_ARGS = [PROGRAMS["pngout"], "-force", "-y"]
@@ -45,11 +45,11 @@
             cprint(
                 f"Skipped pngout for {depth} bit PNG: {old_path}",
                 "white",
                 attrs=["dark"],
             )
             result = old_path
         else:
-            args = tuple(self._PNGOUT_ARGS + [str(old_path), str(new_path)])
+            args = (*self._PNGOUT_ARGS, str(old_path), str(new_path))
             self.run_ext(args)
             result = new_path
         return result
```

### Comparing `picopt-3.2.5/picopt/handlers/webp.py` & `picopt-3.3.0/picopt/handlers/webp.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 from abc import ABC
 from pathlib import Path
 from typing import Any, Optional
 
 from PIL import Image
 from PIL.WebPImagePlugin import WebPImageFile
 
-from picopt.handlers.handler import Format
-from picopt.handlers.image import CONVERTABLE_FORMAT_OBJS, TIFF_FORMAT_OBJ, ImageHandler
+from picopt.handlers.handler import FileFormat
+from picopt.handlers.image import (
+    CONVERTABLE_FILE_FORMATS,
+    TIFF_FILE_FORMAT,
+    ImageHandler,
+)
 from picopt.handlers.png import Png
 
 
 class WebPBase(ImageHandler, ABC):
     """Base for handlers that use WebP utility commands."""
 
     PIL2WEBP_KWARGS: dict[str, Any] = {"lossless": True, "quality": 100, "method": 6}
@@ -30,15 +34,15 @@
         """Pillow webp optimization."""
         return self.pil2native(old_path, new_path)
 
 
 class WebP(WebPBase, ABC):
     """WebP format class."""
 
-    OUTPUT_FORMAT = WebPImageFile.format
+    OUTPUT_FORMAT_STR = WebPImageFile.format
     PROGRAMS: dict[str, Optional[str]] = WebPBase.init_programs(("cwebp",))
     ARGS_PREFIX = [
         PROGRAMS["cwebp"],
         "-mt",
         "-sharp_yuv",
         "-af",
         "-alpha_filter",
@@ -56,72 +60,62 @@
         return new_path
 
 
 class WebPLossless(WebP):
     """Handle lossless webp images and images that convert to lossless webp."""
 
     BEST_ONLY: bool = False
-    OUTPUT_FORMAT_OBJ = Format(WebP.OUTPUT_FORMAT, True, False)
+    OUTPUT_FILE_FORMAT = FileFormat(WebP.OUTPUT_FORMAT_STR, True, False)
     PREFERRED_PROGRAM: str = "cwebp"
     PROGRAMS: dict[str, Optional[str]] = {
         "pil2png": None,
         **WebP.PROGRAMS,
         "pil2webp": None,
     }
-    ARGS_PREFIX = WebP.ARGS_PREFIX + [
-        "-lossless",
-        "-z",
-        "9",
-    ]
-    _PIL2PNG_FORMATS = CONVERTABLE_FORMAT_OBJS | set([TIFF_FORMAT_OBJ])
+    ARGS_PREFIX = [*WebP.ARGS_PREFIX, "-lossless", "-z", "9"]
+    _PIL2PNG_FILE_FORMATS = CONVERTABLE_FILE_FORMATS | {TIFF_FILE_FORMAT}
 
     def pil2png(self, old_path: Path, new_path: Path) -> Path:
         """Internally convert unhandled formats to uncompressed png for cwebp."""
         if (
-            self.input_format_obj in self._PIL2PNG_FORMATS
-            and self.PREFERRED_PROGRAM in self.config._available_programs
+            self.input_file_format in self._PIL2PNG_FILE_FORMATS
+            and self.PREFERRED_PROGRAM in self.config.computed.available_programs
         ):
             new_path = new_path.with_suffix(Png.output_suffix())
             with Image.open(old_path) as image:
                 image.save(
                     new_path,
-                    Png.OUTPUT_FORMAT,
+                    Png.OUTPUT_FORMAT_STR,
                     compress_level=0,
                     exif=self.metadata.exif,
                     icc_profile=self.metadata.icc_profile,
                 )
             image.close()
-            self.input_format_obj = Png.OUTPUT_FORMAT_OBJ
+            self.input_file_format = Png.OUTPUT_FILE_FORMAT
         else:
             new_path = old_path
         return new_path
 
 
 class WebPLossy(WebP):
     """Handle lossy webp images."""
 
-    OUTPUT_FORMAT_OBJ = Format(WebP.OUTPUT_FORMAT, False, False)
-    ARGS_PREFIX = WebP.ARGS_PREFIX + [
-        "-m",
-        "6",
-        "-pass",
-        "10",
-    ]
+    OUTPUT_FILE_FORMAT = FileFormat(WebP.OUTPUT_FORMAT_STR, False, False)
+    ARGS_PREFIX = [*WebP.ARGS_PREFIX, "-m", "6", "-pass", "10"]
 
 
 class Gif2WebP(WebPBase):
-    """
-    Animated WebP format class.
+    """Animated WebP format class.
 
     There are no easy animated WebP optimization tools. So this only
     converts animated gifs.
     """
 
-    OUTPUT_FORMAT = WebP.OUTPUT_FORMAT
-    OUTPUT_FORMAT_OBJ = Format(WebP.OUTPUT_FORMAT, True, True)
+    OUTPUT_FORMAT_STR = WebP.OUTPUT_FORMAT_STR
+    OUTPUT_FILE_FORMAT = FileFormat(WebP.OUTPUT_FORMAT_STR, True, True)
     PIL2WEBP_KWARGS: dict[str, Any] = {
         **WebPLossless.PIL2WEBP_KWARGS,
         "minimize_size": True,
     }
     PREFERRED_PROGRAM = "gif2webp"
     PROGRAMS: dict[str, Optional[str]] = WebPBase.init_programs(
         ("gif2webp", "pil2webp")
@@ -132,15 +126,15 @@
         "-min_size",
         "-m",
         "6",
         "-mt",
     ]
 
     @classmethod
-    def native_input_format_objs(cls):
+    def native_input_file_formats(cls):
         """No native formats."""
         return set()
 
     def gif2webp(self, old_path: Path, new_path: Path) -> Path:
         """Convert animated gif to animated webp."""
         args = tuple(
             self._ARGS_PREFIX
```

### Comparing `picopt-3.2.5/picopt/handlers/webp_animated.py` & `picopt-3.3.0/picopt/handlers/webp_animated.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 """WebP Animated images are treated like containers."""
 from pathlib import Path
 from typing import Optional
 
 from PIL import Image, ImageSequence
 
 from picopt.handlers.container import ContainerHandler
-from picopt.handlers.handler import Format
-from picopt.handlers.image import PNG_ANIMATED_FORMAT_OBJ, TIFF_ANIMATED_FORMAT_OBJ
+from picopt.handlers.handler import FileFormat
+from picopt.handlers.image import PNG_ANIMATED_FILE_FORMAT, TIFF_ANIMATED_FILE_FORMAT
 from picopt.handlers.webp import WebP
 
 
 class WebPAnimatedBase(ContainerHandler):
     """Animated WebP container."""
 
-    OUTPUT_FORMAT: str = WebP.OUTPUT_FORMAT
+    OUTPUT_FORMAT_STR: str = WebP.OUTPUT_FORMAT_STR
     PROGRAMS = ContainerHandler.init_programs(("webpmux", "img2webp"))
-    _OPEN_WITH_PIL_FORMAT_OBJS = set(
-        [PNG_ANIMATED_FORMAT_OBJ, TIFF_ANIMATED_FORMAT_OBJ]
-    )
+    _OPEN_WITH_PIL_FILE_FORMATS = {PNG_ANIMATED_FILE_FORMAT, TIFF_ANIMATED_FILE_FORMAT}
     _IMG2WEBP_ARGS_PREFIX = (PROGRAMS["img2webp"], "-min_size")
     _WEBPMUX_ARGS_PREFIX = (PROGRAMS["webpmux"], "-get", "frame")
     _LOSSLESS = True
 
     @classmethod
-    def identify_format(cls, _path: Path) -> Optional[Format]:
+    def identify_format(cls, _path: Path) -> Optional[FileFormat]:
         """Return the format if this handler can handle this path."""
-        return cls.OUTPUT_FORMAT_OBJ
+        return cls.OUTPUT_FILE_FORMAT
 
     def _get_frame_path(self, frame_index: int) -> Path:
         """Return a frame path for an index."""
         return self.tmp_container_dir / f"frame-{frame_index:08d}.webp"
 
     def unpack_into(self) -> None:
         """Unpack webp into temp dir."""
-        if self.input_format_obj in self._OPEN_WITH_PIL_FORMAT_OBJS:
+        if self.input_file_format in self._OPEN_WITH_PIL_FILE_FORMATS:
             with Image.open(self.original_path) as image:
                 frame_index = 0
                 for frame in ImageSequence.Iterator(image):
                     frame_path = self._get_frame_path(frame_index)
                     frame.save(
                         frame_path,
-                        self.OUTPUT_FORMAT,
+                        self.OUTPUT_FORMAT_STR,
                         lossless=self._LOSSLESS,
                         quality=100,
                         method=0,
                     )
                     frame_index += 1
             image.close()
         else:
@@ -111,15 +109,15 @@
             self._set_metadata(working_path)
 
 
 class WebPAnimatedLossless(WebPAnimatedBase):
     """Animated Lossless WebP Handler."""
 
     _LOSSLESS = True
-    OUTPUT_FORMAT_OBJ = Format(WebPAnimatedBase.OUTPUT_FORMAT, _LOSSLESS, True)
+    OUTPUT_FILE_FORMAT = FileFormat(WebPAnimatedBase.OUTPUT_FORMAT_STR, _LOSSLESS, True)
 
 
 class WebPAnimatedLossy(WebPAnimatedBase):
     """Animated Lossy WebP Handler."""
 
     _LOSSLESS = False
-    OUTPUT_FORMAT_OBJ = Format(WebPAnimatedBase.OUTPUT_FORMAT, _LOSSLESS, True)
+    OUTPUT_FILE_FORMAT = FileFormat(WebPAnimatedBase.OUTPUT_FORMAT_STR, _LOSSLESS, True)
```

### Comparing `picopt-3.2.5/picopt/handlers/zip.py` & `picopt-3.3.0/picopt/handlers/zip.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 """Handler for zip files."""
 import os
-
 from pathlib import Path
 from typing import Optional, Union
 from zipfile import ZIP_DEFLATED, ZipFile, is_zipfile
 
 from PIL import Image, UnidentifiedImageError
 from rarfile import RarFile, is_rarfile
+from termcolor import cprint
 
 from picopt.handlers.container import ContainerHandler
-from picopt.handlers.handler import Format
+from picopt.handlers.handler import FileFormat
 
 
 class Zip(ContainerHandler):
     """Ziplike container."""
 
-    OUTPUT_FORMAT: str = "ZIP"
-    OUTPUT_FORMAT_OBJ: Format = Format(OUTPUT_FORMAT)
-    INPUT_FORMAT_RAR: str = "RAR"
-    INPUT_FORMAT_OBJ_RAR: Format = Format(INPUT_FORMAT_RAR)
-    RAR_SUFFIX: str = "." + INPUT_FORMAT_RAR.lower()
+    OUTPUT_FORMAT_STR: str = "ZIP"
+    OUTPUT_FILE_FORMAT: FileFormat = FileFormat(OUTPUT_FORMAT_STR)
+    INPUT_FORMAT_STR_RAR: str = "RAR"
+    INPUT_FILE_FORMAT_RAR: FileFormat = FileFormat(INPUT_FORMAT_STR_RAR)
+    RAR_SUFFIX: str = "." + INPUT_FORMAT_STR_RAR.lower()
     PROGRAMS: dict[str, Optional[str]] = {ContainerHandler.INTERNAL: None}
 
     @classmethod
-    def identify_format(cls, path: Path) -> Optional[Format]:
+    def identify_format(cls, path: Path) -> Optional[FileFormat]:
         """Return the format if this handler can handle this path."""
-        format = None
+        file_format = None
         suffix = path.suffix.lower()
         if is_zipfile(path) and suffix == cls.output_suffix():
-            format = cls.OUTPUT_FORMAT_OBJ
+            file_format = cls.OUTPUT_FILE_FORMAT
         elif is_rarfile(path) and suffix == cls.RAR_SUFFIX:
-            format = cls.INPUT_FORMAT_OBJ_RAR
-        return format
+            file_format = cls.INPUT_FILE_FORMAT_RAR
+        return file_format
 
     def _get_archive(self) -> Union[ZipFile, RarFile]:
         """Use the zipfile builtin for this archive."""
         if is_zipfile(self.original_path):
             archive = ZipFile(self.original_path, "r")
         elif is_rarfile(self.original_path):
             archive = RarFile(self.original_path, "r")
         else:
-            raise ValueError(f"Unknown archive type: {self.original_path}")
+            msg = f"Unknown archive type: {self.original_path}"
+            raise ValueError(msg)
         return archive
 
     def _set_comment(self, comment: Union[str, bytes, None]) -> None:
         """Set the comment from the archive."""
         if type(comment) is str:
             self.comment = comment.encode()
         elif type(comment) is bytes:
@@ -74,38 +75,35 @@
         with ZipFile(
             working_path, "w", compression=ZIP_DEFLATED, compresslevel=9
         ) as new_zf:
             for root, _, filenames in os.walk(self.tmp_container_dir):
                 root_path = Path(root)
                 for fname in sorted(filenames):
                     if self.config.verbose:
-                        print(".", end="")
+                        cprint(".", end="")
                     full_path = root_path / fname
-                    if self._is_image(full_path):
-                        # Do not deflate images in zipfile.
-                        # Picopte should have already achieved maximum
-                        # compression over deflate.
-                        compress_type = None
-                    else:
-                        compress_type = ZIP_DEFLATED
+                    # Do not deflate images in zipfile.
+                    # Picopte should have already achieved maximum
+                    # compression over deflate.
+                    compress_type = None if self._is_image(full_path) else ZIP_DEFLATED
                     archive_path = full_path.relative_to(self.tmp_container_dir)
                     new_zf.write(full_path, archive_path, compress_type)
             if self.comment:
                 new_zf.comment = self.comment
 
 
 class CBZ(Zip):
     """CBZ Container."""
 
-    OUTPUT_FORMAT: str = "CBZ"
-    OUTPUT_FORMAT_OBJ: Format = Format(OUTPUT_FORMAT)
-    INPUT_FORMAT_RAR: str = "CBR"
-    INPUT_FORMAT_OBJ_RAR: Format = Format(INPUT_FORMAT_RAR)
-    RAR_SUFFIX: str = "." + INPUT_FORMAT_RAR.lower()
+    OUTPUT_FORMAT_STR: str = "CBZ"
+    OUTPUT_FILE_FORMAT: FileFormat = FileFormat(OUTPUT_FORMAT_STR)
+    INPUT_FORMAT_STR_RAR: str = "CBR"
+    INPUT_FILE_FORMAT_RAR: FileFormat = FileFormat(INPUT_FORMAT_STR_RAR)
+    RAR_SUFFIX: str = "." + INPUT_FORMAT_STR_RAR.lower()
 
 
 class EPub(Zip):
     """Epub Container."""
 
-    OUTPUT_FORMAT: str = "EPUB"
-    OUTPUT_FORMAT_OBJ: Format = Format(OUTPUT_FORMAT)
+    OUTPUT_FORMAT_STR: str = "EPUB"
+    OUTPUT_FILE_FORMAT: FileFormat = FileFormat(OUTPUT_FORMAT_STR)
     CONVERT: bool = False
```

### Comparing `picopt-3.2.5/picopt/old_timestamps.py` & `picopt-3.3.0/picopt/old_timestamps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """import picopt 2.0 timestamps to Treestamps."""
 import os
-
 from pathlib import Path
 
 from confuse.templates import AttrDict
 from treestamps import Treestamps
 
-from picopt import PROGRAM_NAME
 from picopt.configurable import Configurable
 
-
-_OLD_TIMESTAMPS_NAME = f".{PROGRAM_NAME}_timestamp"
+OLD_TIMESTAMPS_NAME = ".picopt_timestamp"
 
 
 class OldTimestamps(Configurable):
     """Old timestamps importer."""
 
     def _add_old_timestamp(self, old_timestamp_path: Path) -> None:
         """Get the timestamp from a old style timestamp file."""
@@ -27,37 +24,38 @@
 
     def _import_old_parent_timestamps(self, path: Path) -> None:
         """Walk up to the root eating old style timestamps."""
         if self.is_path_ignored(path) or (
             not self._config.symlinks and path.is_symlink()
         ):
             return
-        old_timestamp_path = path / _OLD_TIMESTAMPS_NAME
+        old_timestamp_path = path / OLD_TIMESTAMPS_NAME
         self._add_old_timestamp(old_timestamp_path)
         if path.parent != path:
             self._import_old_parent_timestamps(path.parent)
 
     def _import_old_child_timestamps(self, path: Path) -> None:
         if (
             self.is_path_ignored(path)
             or not self._config.symlinks
             and path.is_symlink()
         ):
             return
         for root, dirnames, filenames in os.walk(path):
             root_path = Path(root)
-            if _OLD_TIMESTAMPS_NAME in filenames:
-                old_timestamp_path = root_path / _OLD_TIMESTAMPS_NAME
+            if OLD_TIMESTAMPS_NAME in filenames:
+                old_timestamp_path = root_path / OLD_TIMESTAMPS_NAME
                 self._add_old_timestamp(old_timestamp_path)
-                self._timestamps._consumed_paths.add(old_timestamp_path)
+                # Picopt is the only program that used old treestamps
+                self._timestamps._consumed_paths.add(old_timestamp_path)  # noqa SLF001
             for dirname in dirnames:
                 self._import_old_child_timestamps(root_path / dirname)
 
     def import_old_timestamps(self) -> None:
         """Import all old timestamps."""
-        self._import_old_parent_timestamps(self._timestamps.dir)
-        self._import_old_child_timestamps(self._timestamps.dir)
+        self._import_old_parent_timestamps(self._timestamps.root_dir)
+        self._import_old_child_timestamps(self._timestamps.root_dir)
 
     def __init__(self, config: AttrDict, timestamps: Treestamps):
         """Hold new timestamp object."""
         super().__init__(config)
         self._timestamps = timestamps
```

### Comparing `picopt-3.2.5/picopt/pillow/header.py` & `picopt-3.3.0/picopt/pillow/header.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Unpack items from a file descriptor."""
 import struct
-
 from dataclasses import dataclass
 from typing import BinaryIO, Union
 
 
 def unpack(
     fmt_type: str, length: int, file_desc: BinaryIO
 ) -> Union[tuple[bytes, ...], tuple[int]]:
@@ -13,14 +12,14 @@
 
 
 @dataclass
 class ImageHeader:
     """The seek location and value of a byte header."""
 
     offset: int
-    bytes: tuple[bytes, ...]
+    compare_bytes: tuple[bytes, ...]
 
     def compare(self, img: BinaryIO) -> bool:
         """Seek to a spot in a binary file and compare a byte array."""
         img.seek(self.offset)
-        compare = unpack("c", len(self.bytes), img)
-        return compare == self.bytes
+        compare = unpack("c", len(self.compare_bytes), img)
+        return compare == self.compare_bytes
```

### Comparing `picopt-3.2.5/picopt/pillow/png_bit_depth.py` & `picopt-3.3.0/picopt/pillow/png_bit_depth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 #!/usr/bin/env python3
-"""
-Get the bit depth of a png image manually.
+"""Get the bit depth of a png image manually.
 
 https://www.w3.org/TR/PNG-Chunks.html
 This should be a part of Pillow
 """
 from pathlib import Path
 from typing import Optional
 
 from termcolor import cprint
 
 from picopt.pillow.header import ImageHeader, unpack
 
-
 PNG_HEADER = ImageHeader(0, (b"\x89", b"P", b"N", b"G", b"\r", b"\n", b"\x1a", b"\n"))
 BIT_DEPTH_OFFSET = 24
 
 
 def png_bit_depth(path: Path) -> Optional[int]:
     """If a file is a png, get the bit depth from the standard position."""
     result = None
     with path.open("rb") as img:
         if PNG_HEADER.compare(img):
-
             img.seek(BIT_DEPTH_OFFSET)  # bit depth offset
             depth = unpack("b", 1, img)[0]
             result = int(depth)
         else:
             cprint(f"WARNING: {path} is not a png!", "yellow")
     return result
 
 
 def main() -> None:
     """Stand alone cli tool for getting png bit depth."""
     import sys
 
     bit_depth = png_bit_depth(Path(sys.argv[1]))
-    print(bit_depth)
+    print(bit_depth)  # noqa T201
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `picopt-3.2.5/picopt/pillow/webp_lossless.py` & `picopt-3.3.0/picopt/pillow/webp_lossless.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
-"""
-Determine if a webp is lossless.
+"""Determine if a webp is lossless.
 
 This should be a part of Pillow
 https://developers.google.com/speed/webp/docs/webp_lossless_bitstream_specification
 """
 from pathlib import Path
 
 from picopt.pillow.header import ImageHeader
 
-
 RIFF_HEADER = ImageHeader(0, (b"R", b"I", b"F", b"F"))
 WEBP_HEADER = ImageHeader(8, (b"W", b"E", b"B", b"P"))
 VP8L_HEADER = ImageHeader(12, (b"V", b"P", b"8", b"L"))
 
 HEADERS = (RIFF_HEADER, WEBP_HEADER, VP8L_HEADER)
 
 
@@ -30,12 +28,12 @@
 
 
 def main() -> None:
     """Stand alone cli tool for getting lossless status."""
     import sys
 
     lossless = is_lossless(sys.argv[1])
-    print(lossless)
+    print(lossless)  # noqa T201
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `picopt-3.2.5/picopt/stats.py` & `picopt-3.3.0/picopt/stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,42 @@
 """Statistics for the optimization operations."""
 from dataclasses import dataclass, field
-from pathlib import Path
 from subprocess import CalledProcessError
-from typing import Optional
 
 from humanize import naturalsize
 from termcolor import cprint
 
+from picopt.data import ReportInfo
+
 
 class ReportStats:
     """Container for reported stats from optimization operations."""
 
     _TAB = " " * 4
 
     def __init__(
         self,
-        path: Path,
-        bytes_count: Optional[tuple[int, int]],
-        test: bool,
-        convert: bool,
-        exc: Optional[Exception] = None,
+        info: ReportInfo,
     ) -> None:
         """Initialize required instance variables."""
-        self.path = path
-        self.test = test
-        self.convert = convert
-        self.exc = exc
-        if bytes_count:
-            self.bytes_in = bytes_count[0]
-            self.bytes_out = bytes_count[1]
-        else:
-            self.bytes_in = 0
-            self.bytes_out = 0
+        self.path = info.path
+        self.test = info.test
+        self.convert = info.convert
+        self.exc = info.exc
+        self.bytes_in = info.bytes_in
+        self.bytes_out = info.bytes_out
         self.saved = self.bytes_in - self.bytes_out
 
     def _new_percent_saved(self) -> str:
         """Spit out how much space the optimization saved."""
-        if self.bytes_in <= 0:
-            ratio = 1.0
-        else:
-            ratio = self.bytes_out / self.bytes_in
+        ratio = 1.0 if self.bytes_in <= 0 else self.bytes_out / self.bytes_in
         saved = naturalsize(self.saved)
         percent_saved = (1 - ratio) * 100
 
-        result = "{:.{prec}f}% ({})".format(percent_saved, saved, prec=2)
-        return result
+        return "{:.{prec}f}% ({})".format(percent_saved, saved, prec=2)
 
     def _report_saved(self) -> str:
         """Return the percent saved."""
         report = ""
 
         report += f"{self.path}: "
         report += self._new_percent_saved()
@@ -76,18 +64,15 @@
         """Record the percent saved & print it."""
         attrs = []
         if self.exc:
             report = self._report_error()
             color = "red"
         else:
             report = self._report_saved()
-            if self.convert:
-                color = "cyan"
-            else:
-                color = "white"
+            color = "cyan" if self.convert else "white"
 
             if self.saved <= 0:
                 color = "blue"
                 attrs = ["bold"]
 
         cprint(report, color, attrs=attrs)
```

### Comparing `picopt-3.2.5/picopt/walk.py` & `picopt-3.3.0/picopt/walk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,149 +1,171 @@
 """Walk the directory trees and files and call the optimizers."""
 import os
 import shutil
 import time
 import traceback
-
 from multiprocessing.pool import ApplyResult, Pool
 from pathlib import Path
-from typing import Optional, Type
+from typing import Optional
 
 from confuse.templates import AttrDict
 from humanize import naturalsize
 from termcolor import cprint
-from treestamps import Treestamps
+from treestamps import Grovestamps, GrovestampsConfig, Treestamps
 
 from picopt import PROGRAM_NAME
 from picopt.config import TIMESTAMPS_CONFIG_KEYS
 from picopt.configurable import Configurable
+from picopt.data import PathInfo, ReportInfo
 from picopt.handlers.container import ContainerHandler
 from picopt.handlers.factory import create_handler
 from picopt.handlers.handler import Handler
 from picopt.handlers.image import ImageHandler
 from picopt.handlers.png import Png
 from picopt.handlers.webp import WebP
 from picopt.handlers.zip import CBZ, Zip
-from picopt.old_timestamps import OldTimestamps
+from picopt.old_timestamps import OLD_TIMESTAMPS_NAME, OldTimestamps
 from picopt.stats import ReportStats, Totals
 
 
 class Walk(Configurable):
     """Walk object for storing state of a walk run."""
 
     TIMESTAMPS_FILENAMES = set(Treestamps.get_filenames(PROGRAM_NAME))
     LOWERCASE_TESTNAME = ".picopt_case_sensitive_test"
     UPPERCASE_TESTNAME = LOWERCASE_TESTNAME.upper()
 
     ########
     # Init #
     ########
     def _convert_message(
-        self, convert_from_formats: frozenset[str], convert_handler: Type[Handler]
+        self, convert_from_formats: frozenset[str], convert_handler: type[Handler]
     ):
         convert_from = ", ".join(
             sorted(convert_from_formats & frozenset(self._config.formats))
         )
-        convert_to = convert_handler.OUTPUT_FORMAT
+        convert_to = convert_handler.OUTPUT_FORMAT_STR
         cprint(f"Converting {convert_from} to {convert_to}", "cyan")
 
+    def _init_run_verbose(self) -> None:
+        """Print verbose init messages."""
+        format_list = ", ".join(sorted(self._config.formats))
+        cprint(f"Optimizing formats: {format_list}")
+        if self._config.convert_to:
+            if WebP.OUTPUT_FORMAT_STR in self._config.convert_to:
+                self._convert_message(
+                    self._config.computed.convertable_formats.webp, WebP
+                )
+            elif Png.OUTPUT_FORMAT_STR in self._config.convert_to:
+                self._convert_message(
+                    self._config.computed.convertable_formats.png, Png
+                )
+            if Zip.OUTPUT_FORMAT_STR in self._config.convert_to:
+                self._convert_message(frozenset([Zip.INPUT_FORMAT_STR_RAR]), Zip)
+            if CBZ.OUTPUT_FORMAT_STR in self._config.convert_to:
+                self._convert_message(frozenset([CBZ.INPUT_FORMAT_STR_RAR]), CBZ)
+        if self._config.after is not None:
+            after = time.ctime(self._config.after)
+            cprint(f"Optimizing after {after}")
+
+    def _init_run_timestamps(self) -> None:
+        """Init timestamps."""
+        config = GrovestampsConfig(
+            paths=self._top_paths,
+            program_name=PROGRAM_NAME,
+            verbose=self._config.verbose,
+            symlinks=self._config.symlinks,
+            ignore=self._config.ignore,
+            check_config=self._config.timestamps_check_config,
+            program_config=self._config,
+            program_config_keys=TIMESTAMPS_CONFIG_KEYS,
+        )
+        self._timestamps = Grovestamps(config)
+        for timestamps in self._timestamps.values():
+            OldTimestamps(self._config, timestamps).import_old_timestamps()
+
     def _init_run(self):
         """Init Run."""
         # Validate top_paths
         if not self._top_paths:
-            raise ValueError("No paths to optimize.")
+            msg = "No paths to optimize."
+            raise ValueError(msg)
         for path in self._top_paths:
             if not path.exists():
-                raise ValueError(f"Path does not exist: {path}")
+                msg = f"Path does not exist: {path}"
+                raise ValueError(msg)
 
         # Tell the user what we're doing
         if self._config.verbose:
-            print("Optimizing formats:", *sorted(self._config.formats))
-            if self._config.convert_to:
-                if WebP.OUTPUT_FORMAT in self._config.convert_to:
-                    self._convert_message(self._config._convertable_formats.webp, WebP)
-                elif Png.OUTPUT_FORMAT in self._config.convert_to:
-                    self._convert_message(self._config._convertable_formats.png, Png)
-                if Zip.OUTPUT_FORMAT in self._config.convert_to:
-                    self._convert_message(frozenset([Zip.INPUT_FORMAT_RAR]), Zip)
-                if CBZ.OUTPUT_FORMAT in self._config.convert_to:
-                    self._convert_message(frozenset([CBZ.INPUT_FORMAT_RAR]), CBZ)
-            if self._config.after is not None:
-                print("Optimizing after", time.ctime(self._config.after))
+            self._init_run_verbose()
 
         # Init timestamps
         if self._config.timestamps:
-            self._timestamps = Treestamps.map_factory(
-                self._top_paths,
-                PROGRAM_NAME,
-                self._config.verbose,
-                self._config.symlinks,
-                self._config.ignore,
-                self._config,
-                TIMESTAMPS_CONFIG_KEYS,
-            )
-            for timestamps in self._timestamps.values():
-                OldTimestamps(self._config, timestamps).import_old_timestamps()
+            self._init_run_timestamps()
 
     ############
     # Checkers #
     ############
-    def _is_skippable(self, path: Path) -> bool:
+    def _is_skippable(self, path: Path) -> bool:  # noqa C901
         """Handle things that are not optimizable files."""
         skip = False
         # File types
         if not self._config.symlinks and path.is_symlink():
             if self._config.verbose > 1:
                 cprint(f"Skip symlink {path}", "white", attrs=["dark"])
             skip = True
         elif path.name in self.TIMESTAMPS_FILENAMES:
             if self._config.verbose > 1:
                 cprint(f"Skip timestamp {path}", "white", attrs=["dark"])
             skip = True
+        elif path.name in OLD_TIMESTAMPS_NAME:
+            if self._config.verbose > 1:
+                cprint(f"Skip legacy timestamp {path}", "white", attrs=["dark"])
+            skip = True
         elif not path.exists():
             if self._config.verbose > 1:
                 cprint(f"WARNING: {path} not found.", "yellow")
             skip = True
         elif self.is_path_ignored(path):
             if self._config.verbose > 1:
                 cprint(f"Skip ignored {path}", "white", attrs=["dark"])
             skip = True
 
         return skip
 
     def _is_older_than_timestamp(
         self,
-        path: Path,
-        top_path: Path,
-        container_mtime: Optional[float],
+        info: PathInfo,
     ) -> bool:
         """Is the file older than the timestamp."""
         # If the file is in an container, use the container time.
         # This helps if you have a new container that you
         # collected from someone who put really old files in it that
         # should still be optimised
-        if container_mtime is not None:
-            mtime = container_mtime
-        else:
-            mtime = path.stat().st_mtime
+        mtime = (
+            info.container_mtime
+            if info.container_mtime is not None
+            else info.path.stat().st_mtime
+        )
 
         # The timestamp or configured walk after time for comparison.
-        walk_after = None
         if self._config.after is not None:
             walk_after = self._config.after
-        elif container_mtime is None:
-            timestamps = self._timestamps.get(top_path, {})
-            walk_after = timestamps.get(path)
+        elif info.container_mtime is None and self._config.timestamps:
+            timestamps = self._timestamps.get(info.top_path, {})
+            walk_after = timestamps.get(info.path)
+        else:
+            walk_after = None
 
         if walk_after is None:
             return False
 
         return bool(mtime <= walk_after)
 
-    def _clean_up_working_files(self, path):
+    def _clean_up_working_files(self, path) -> None:
         """Auto-clean old working temp files if encountered."""
         try:
             if path.is_dir():
                 shutil.rmtree(path, ignore_errors=True)
             else:
                 path.unlink(missing_ok=True)
             if self._config.verbose > 1:
@@ -169,172 +191,192 @@
             else:
                 self._totals.bytes_in += final_result.bytes_in
                 self._totals.bytes_out += final_result.bytes_out
             if self._config.timestamps and not container_mtime:
                 timestamps = self._timestamps[top_path]
                 timestamps.set(final_result.path)
 
-    def walk_dir(
-        self,
-        path: Path,
-        top_path: Path,
-        container_mtime: Optional[float],
-        convert: bool,
-        is_case_sensitive: bool,
-    ) -> None:
+    def walk_dir(self, info: PathInfo) -> None:
         """Recursively optimize a directory."""
+        if not self._config.recurse and info.container_mtime is None:
+            # Skip
+            return
+
         results = []
         files = []
-        for name in sorted(os.listdir(path)):
-            entry_path = path / name
+        for name in sorted(os.listdir(info.path)):
+            entry_path = info.path / name
             if entry_path.is_dir():
-                self.walk_file(
-                    entry_path, top_path, container_mtime, convert, is_case_sensitive
+                path_info = PathInfo(
+                    entry_path,
+                    info.top_path,
+                    info.container_mtime,
+                    info.convert,
+                    info.is_case_sensitive,
                 )
+                self.walk_file(path_info)
             else:
                 files.append(entry_path)
 
         for entry_path in files:
-            result = self.walk_file(
-                entry_path, top_path, container_mtime, convert, is_case_sensitive
+            path_info = PathInfo(
+                entry_path,
+                info.top_path,
+                info.container_mtime,
+                info.convert,
+                info.is_case_sensitive,
             )
+            result = self.walk_file(path_info)
             if result:
                 results.append(result)
 
         self._finish_results(
             results,
-            container_mtime,
-            top_path,
+            info.container_mtime,
+            info.top_path,
         )
 
-        if self._config.timestamps and not container_mtime:
+        if self._config.timestamps and not info.container_mtime:
             # Compact timestamps after every directory completes
-            timestamps = self._timestamps[top_path]
-            timestamps.set(path, compact=True)
+            timestamps = self._timestamps[info.top_path]
+            timestamps.set(info.path, compact=True)
 
     def _walk_container(
         self, top_path: Path, handler: ContainerHandler, is_case_sensitive: bool
     ) -> ApplyResult:
         """Optimize a container."""
         result: ApplyResult
         try:
             handler.unpack()
             container_mtime = handler.original_path.stat().st_mtime
-            self.walk_dir(
+            path_info = PathInfo(
                 handler.tmp_container_dir,
                 top_path,
                 container_mtime,
                 handler.CONVERT,
                 is_case_sensitive,
             )
+
+            self.walk_dir(path_info)
             result = self._pool.apply_async(handler.repack)
         except Exception as exc:
             traceback.print_exc()
-            args = tuple([exc])
+            args = (exc,)
             result = self._pool.apply_async(handler.error, args=args)
         return result
 
-    def walk_file(
+    def _skip_older_than_timestamp(self, path) -> None:
+        """Report on skipping files older than the timestamp."""
+        color = "green"
+        if self._config.verbose == 1:
+            cprint(".", color, end="")
+        elif self._config.verbose > 1:
+            cprint(f"Skip older than timestamp: {path}", color)
+
+    def _is_walk_file_skip(
         self,
-        path: Path,
-        top_path: Path,
-        container_mtime: Optional[float],
-        convert: bool,
-        is_case_sensitive: bool,
-    ) -> Optional[ApplyResult]:
+        info: PathInfo,
+    ) -> bool:
+        """Decide on skip the file or not."""
+        if self._is_skippable(info.path):
+            if self._config.verbose == 1:
+                cprint(".", "white", attrs=["dark"], end="")
+            return True
+
+        if info.path.name.rfind(Handler.WORKING_SUFFIX) > -1:
+            self._clean_up_working_files(info.path)
+            if self._config.verbose == 1:
+                cprint(".", "yellow", end="")
+            return True
+
+        if self._is_older_than_timestamp(info):
+            self._skip_older_than_timestamp(info.path)
+            return True
+
+        return False
+
+    def _handle_file(self, handler, top_path, is_case_sensitive):
+        """Call the correct walk or pool apply for the handler."""
+        if isinstance(handler, ContainerHandler):
+            # Unpack inline, not in the pool, and walk immediately like dirs.
+            result = self._walk_container(top_path, handler, is_case_sensitive)
+        elif isinstance(handler, ImageHandler):
+            result = self._pool.apply_async(handler.optimize_image)
+        else:
+            msg = f"bad handler {handler}"
+            raise TypeError(msg)
+        return result
+
+    def walk_file(self, info: PathInfo) -> Optional[ApplyResult]:
         """Optimize an individual file."""
-        result: Optional[ApplyResult] = None
         try:
-            # START DECIDE
-            if self._is_skippable(path):
-                if self._config.verbose == 1:
-                    cprint(".", "white", attrs=["dark"], end="")
-                return result
-
-            if path.name.rfind(Handler.WORKING_SUFFIX) > -1:
-                self._clean_up_working_files(path)
-                if self._config.verbose == 1:
-                    cprint(".", "yellow", end="")
-                return result
-
-            if path.is_dir():
-                if self._config.recurse or container_mtime is not None:
-                    result = self.walk_dir(
-                        path, top_path, container_mtime, convert, is_case_sensitive
-                    )
-                return result
-
-            if self._is_older_than_timestamp(path, top_path, container_mtime):
-                color = "green"
-                if self._config.verbose == 1:
-                    cprint(".", color, end="")
-                elif self._config.verbose > 1:
-                    cprint(f"Skip older than timestamp: {path}", color)
-                return result
-            # END DECIDE
+            if info.path.is_dir():
+                return self.walk_dir(info)
 
-            handler = create_handler(self._config, path, is_case_sensitive, convert)
+            if self._is_walk_file_skip(info):
+                return None
 
+            handler = create_handler(self._config, info)
             if handler is None:
-                return result
+                return None
 
             if self._config.list_only:
-                print(f"{path}: {handler.__class__.__name__}")
-                return result
+                return None
 
-            if isinstance(handler, ContainerHandler):
-                # Unpack inline, not in the pool, and walk immediately like dirs.
-                result = self._walk_container(top_path, handler, is_case_sensitive)
-            elif isinstance(handler, ImageHandler):
-                result = self._pool.apply_async(handler.optimize_image)
-            else:
-                raise ValueError(f"bad handler {handler}")
+            result = self._handle_file(handler, info.top_path, info.is_case_sensitive)
         except Exception as exc:
             traceback.print_exc()
-            result = self._pool.apply_async(
-                ReportStats, args=(path, None, self._config.test, convert, exc)
+            report_info = ReportInfo(
+                path=info.path,
+                convert=info.convert,
+                test=self._config.test,
+                exc=exc,
             )
+            result = self._pool.apply_async(ReportStats, (report_info,))
         return result
 
     ##########
     # Finish #
     ##########
+    def _report_totals_bytes_in(self) -> None:
+        """Report Totals if there were bytes in."""
+        if not self._config.verbose and not self._config.test:
+            return
+        bytes_saved = self._totals.bytes_in - self._totals.bytes_out
+        percent_bytes_saved = bytes_saved / self._totals.bytes_in * 100
+        msg = ""
+        if self._config.test:
+            if percent_bytes_saved > 0:
+                msg += "Could save"
+            elif percent_bytes_saved == 0:
+                msg += "Could even out for"
+            else:
+                msg += "Could lose"
+        else:
+            if percent_bytes_saved > 0:  # noqa: PLR5501
+                msg += "Saved"
+            elif percent_bytes_saved == 0:
+                msg += "Evened out"
+            else:
+                msg = "Lost"
+        msg += " a total of {} or {:.{prec}f}%".format(
+            naturalsize(bytes_saved), percent_bytes_saved, prec=2
+        )
+        cprint(msg)
+        if self._config.test:
+            cprint("Test run did not change any files.")
+
     def _report_totals(self) -> None:
         """Report the total number and percent of bytes saved."""
         if self._config.verbose == 1:
-            print()
+            cprint("")
         if self._totals.bytes_in:
-            bytes_saved = self._totals.bytes_in - self._totals.bytes_out
-            percent_bytes_saved = bytes_saved / self._totals.bytes_in * 100
-            msg = ""
-            if self._config.test:
-                if percent_bytes_saved > 0:
-                    msg += "Could save"
-                elif percent_bytes_saved == 0:
-                    msg += "Could even out for"
-                else:
-                    msg += "Could lose"
-            else:
-                if percent_bytes_saved > 0:
-                    msg += "Saved"
-                elif percent_bytes_saved == 0:
-                    msg += "Evened out"
-                else:
-                    msg = "Lost"
-            msg += " a total of {} or {:.{prec}f}%".format(
-                naturalsize(bytes_saved), percent_bytes_saved, prec=2
-            )
-            if self._config.verbose:
-                print(msg)
-                if self._config.test:
-                    print("Test run did not change any files.")
-
-        else:
-            if self._config.verbose:
-                print("Didn't optimize any files.")
+            self._report_totals_bytes_in()
+        elif self._config.verbose:
+            cprint("Didn't optimize any files.")
 
         if self._totals.errors:
             cprint("Errors with the following files:", "red")
             for rs in self._totals.errors:
                 rs.report()
 
     ################
@@ -346,23 +388,22 @@
         self._totals = Totals()
         top_paths = []
         for path in sorted(frozenset(self._config.paths)):
             if path.is_symlink() and not self._config.symlinks:
                 continue
             top_paths.append(path)
         self._top_paths: tuple[Path, ...] = tuple(top_paths)
-        self._timestamps: dict[Path, Treestamps] = {}
         if self._config.jobs:
             self._pool = Pool(self._config.jobs)
         else:
             self._pool = Pool()
 
     @classmethod
     def _is_case_sensitive(cls, dirpath: Path) -> bool:
-        """Deterimine if a path is on a case sensitive filesystem."""
+        """Determine if a path is on a case sensitive filesystem."""
         lowercase_path = dirpath / cls.LOWERCASE_TESTNAME
         result = False
         try:
             lowercase_path.touch()
             uppercase_path = dirpath / cls.UPPERCASE_TESTNAME
             result = not uppercase_path.exists()
         finally:
@@ -376,17 +417,18 @@
         except Exception as exc:
             cprint(str(exc), "red")
             return False
 
         # Walk each top file
         top_results = {}
         for top_path in self._top_paths:
-            dirpath = Treestamps.dirpath(top_path)
+            dirpath = Treestamps.get_dir(top_path)
             is_case_sensitive = self._is_case_sensitive(dirpath)
-            result = self.walk_file(top_path, dirpath, None, True, is_case_sensitive)
+            path_info = PathInfo(top_path, dirpath, None, True, is_case_sensitive)
+            result = self.walk_file(path_info)
             if not result:
                 continue
             if dirpath not in top_results:
                 top_results[dirpath] = []
             top_results[dirpath].append(result)
 
         # Finish
@@ -394,15 +436,12 @@
             self._finish_results(results, None, dirpath)
 
         # Shut down multiprocessing
         self._pool.close()
         self._pool.join()
 
         if self._config.timestamps:
-            for top_path, timestamps in self._timestamps.items():
-                if self._config.verbose:
-                    print(f"\nSaving timestamps for {top_path}")
-                timestamps.dump()
+            self._timestamps.dump()
 
         # Finish by reporting totals
         self._report_totals()
         return True
```

### Comparing `picopt-3.2.5/pyproject.toml` & `picopt-3.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = ["poetry.core.masonry.api"]
 
 [tool.poetry]
 name = "picopt"
-version = "3.2.5"
+version = "3.3.0"
 description = "A multi format lossless image optimizer that uses external tools"
 license = "GPL-3.0-only"
 authors = ["AJ Slater <aj@slater.net>"]
 readme = "README.md"
 homepage = "https://github.com/ajslater/picopt"
 documentation = "https://github.com/ajslater/picopt"
 keywords = ["image", "png", "jpg", "cbz", "cbr"]
@@ -30,47 +30,38 @@
 python = "^3.9"
 confuse = "^2.0.0"
 humanize = "^4.0.0"
 python-dateutil = "^2.8"
 rarfile = "^4.0"
 "ruamel.yaml" = "^0.17.16"
 termcolor = "^2.0.1"
-treestamps = "^0.3.3"
+treestamps = "^0.4.0"
 Pillow = "^9.0"
 
 [tool.poetry.group.dev.dependencies]
-bandit = "^1.7.4"
+black = "^23.1.0"
 codespell = "^2.1.0"
 coverage = { extras = ["toml"], version = "^7.0" }
-flake8-black = "^0.3.2"
-flake8-bugbear = "^22.1"
-flake8-docstrings = "^1.5.0"
-flake8-eradicate = "^1.2.1"
-isort = "^5.10.1"
 neovim = "^0.3.1"
-pep8-naming = "^0.13.0"
 pyright = "^1.1.237"
 pytest = "^7.0.0"
 pytest-cov = "^4.0"
 pytest-gitignore = "^1.3"
-radon = "^5.1"
-tomli = "^2.0.1"
+radon = { version = "^6.0.1", extras = ["toml"] }
+ruff = "^0.0.264"
 types-python-dateutil = "^2.8.0"
 vulture = "^2.1"
 
 [tool.poetry.scripts]
 picopt = "picopt.cli:main"
 
 [tool.poetry.urls]
 "Source" = "https://github.com/ajslater/picopt"
 "Issues" = "https://github.com/ajslater/picopt/issues"
 
-[tool.bandit]
-exclude = [".venv", "node_modules", "**/__pycache__"]
-
 [tool.black]
 exclude = "/(.git|.mypy_cache|.pytest_cache|.venv|__pycache__|dist|node_modules|test-results|typings)/"
 
 [tool.codespell]
 skip = ".git,.mypy_cache,.pytest_cache,.venv,*~,./dist,./node_modules,./package-lock.json,./poetry.lock,./test-results"
 builtin = "clear,rare,code"
 check-hidden = true
@@ -91,22 +82,14 @@
   "test-results/*",
   "typings/*"
 ]
 
 [tool.coverage.html]
 directory = "test-results/coverage"
 
-[tool.isort]
-profile = "black"
-lines_after_imports = 2
-lines_between_types = 1
-multi_line_output = 3
-skip = ".git,.mypy_cache,.pytest_cache,.venv,__pycache__,dist,node_modules,test-results,typings"
-color_output = true
-
 [tool.pytest.ini_options]
 junit_family = "xunit2"
 addopts = """
   --junitxml=test-results/pytest/junit.xml
   -ra
   --strict-markers
   --cov
@@ -121,19 +104,14 @@
   --ignore=node_modules
   --ignore=test-results
   --ignore=typings
   --ignore=vulture_whitelist.py
   --ignore-glob=*__pycache__*
 """
 
-[tool.vulture]
-exclude = [".git/", ".mypy_cache/", ".pytest_cache", ".venv", "*__pycache__*"]
-min_confidence = 61
-sort_by_size = true
-
 [tool.pyright]
 exclude = [
   "**/__pycache__",
   "**/node_modules",
   ".git",
   ".mypy_cache",
   ".pytest_cache",
@@ -144,7 +122,73 @@
   "test-results",
   "typings",
   "vulture_whitelist.py"
 ]
 useLibraryCodeForTypes = true
 reportMissingImports = true
 reportImportCycles = true
+
+[tool.radon]
+exclude = "*~,.git/*,.mypy_cache/*,.pytest_cache/*,.venv/*,__pycache__/*,dist/*,node_modules/*,test-results/*,typings/*"
+
+[tool.ruff]
+extend-exclude = ["cache", "codex/_vendor_haystack", "frontend", "typings"]
+extend-ignore = ["S101", "D203", "D213"]
+#extend-select = ["B", "B9", "C", "D", "I", "N", "S", "W"]
+extend-select = [
+  "A",
+  "ARG",
+  "B",
+  "B9",
+  "C",
+  "C4",
+  "C90",
+  "D",
+  "DJ",
+  "DTZ",
+  "E",
+  "EM",
+  "EXE",
+  "F",
+  "I",
+  "ICN",
+  "INP",
+  "ISC",
+  "PIE",
+  "PL",
+  "PT",
+  "PTH",
+  "PYI",
+  "Q",
+  "N",
+  "RET",
+  "RSE",
+  "RUF",
+  "S",
+  "SIM",
+  "SLF",
+  "T10",
+  "T20",
+  "TCH",
+  "TID",
+  "TRY",
+  "UP",
+  "W",
+  "YTT"
+  # "ANN", "ERA", "COM"
+]
+external = ["V101"]
+# format = "grouped"
+# show-source = true
+target-version = "py39"
+task-tags = ["TODO", "FIXME", "XXX", "http", "HACK"]
+
+[tool.ruff.per-file-ignores]
+"tests/*" = ["SLF001", "T201", "T203"]
+
+[tool.ruff.pycodestyle]
+ignore-overlong-task-comments = true
+
+[tool.vulture]
+exclude = [".git/", ".mypy_cache/", ".pytest_cache", ".venv", "*__pycache__*"]
+min_confidence = 61
+sort_by_size = true
```

### Comparing `picopt-3.2.5/tests/__init__.py` & `picopt-3.3.0/tests/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Tests init."""
 import inspect
-
 from pathlib import Path
 
-
 TEST_FILES_DIR = Path("tests/test_files")
 IMAGES_DIR = TEST_FILES_DIR / "images"
 INVALID_DIR = TEST_FILES_DIR / "invalid"
 CONTAINER_DIR = TEST_FILES_DIR / "containers"
-TMP_ROOT = "/tmp"
+TMP_ROOT = "/tmp"  # noqa
 
 
 def get_test_dir():
     """Return a module specific tmpdir."""
     frame = inspect.currentframe()
     if frame and frame.f_back:
         caller = frame.f_back
```

### Comparing `picopt-3.2.5/tests/integration/test_containers.py` & `picopt-3.3.0/tests/integration/test_containers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Test comic format."""
 import shutil
-
 from platform import system
 from zipfile import ZipFile
 
 from picopt import PROGRAM_NAME, cli
 from tests import CONTAINER_DIR, get_test_dir
 
-
 __all__ = ()
 TMP_ROOT = get_test_dir()
 SRC_CBZ = CONTAINER_DIR / "test_cbz.cbz"
 
 if system() == "Darwin":
     FNS = {
         "test_cbz.cbz": (93408, 84493, ("cbz", 93408)),
@@ -25,52 +23,62 @@
         "test_cbz.cbz": (93408, 84481, ("cbz", 93408)),
         "test_cbr.cbr": (93725, 93725, ("cbz", 84494)),
         "test_rar.rar": (93675, 93675, ("zip", 84481)),
         "test_zip.zip": (2974, 1917, ("zip", 2974)),
         "igp-twss.epub": (292448, 280700, ("epub", 292448)),
     }
 
+EPUB_FN = "igp-twss.epub"
+BMP_FN = "OPS/test_bmp.bmp"
+
 
 class TestContainersDir:
+    """Test containers dirs."""
+
     def setup_method(self) -> None:
+        """Set up method."""
         self.teardown_method()
         shutil.copytree(CONTAINER_DIR, TMP_ROOT)
         for name, sizes in FNS.items():
             path = TMP_ROOT / name
             assert path.stat().st_size == sizes[0]
 
     def teardown_method(self) -> None:
+        """Tear down method."""
         if TMP_ROOT.exists():
             shutil.rmtree(TMP_ROOT)
 
     def test_containers_noop(self) -> None:
+        """Test containers noop."""
         args = (PROGRAM_NAME, "-r", str(TMP_ROOT))
         res = cli.main(args)
         assert res
         for name, sizes in FNS.items():
-            if name == "igp-twss.epub":
+            if name == EPUB_FN:
                 path = TMP_ROOT / name
                 with ZipFile(path, "r") as zf:
                     namelist = zf.namelist()
-                assert "OPS/test_bmp.bmp" in namelist
+                assert BMP_FN in namelist
             path = TMP_ROOT / name
             assert path.stat().st_size == sizes[0]
 
     def test_containers_no_convert(self) -> None:
+        """Test containers no convert."""
         args = (PROGRAM_NAME, "-rx", "CBZ,ZIP,EPUB", "-c WEBP", str(TMP_ROOT))
         res = cli.main(args)
         assert res
         for name, sizes in FNS.items():
             path = TMP_ROOT / name
-            if name == "igp-twss.epub":
+            if name == EPUB_FN:
                 with ZipFile(path, "r") as zf:
                     namelist = zf.namelist()
-                assert "OPS/test_bmp.bmp" in namelist
+                assert BMP_FN in namelist
             assert path.stat().st_size == sizes[1]
 
     def test_containers_convert_to_zip(self) -> None:
+        """Test containers convert to zip."""
         args = (PROGRAM_NAME, "-rc", "ZIP,CBZ", str(TMP_ROOT))
         res = cli.main(args)
         assert res
         for name, sizes in FNS.items():
             path = (TMP_ROOT / name).with_suffix("." + sizes[2][0])
             assert path.stat().st_size == sizes[2][1]
```

### Comparing `picopt-3.2.5/tests/integration/test_images_dir.py` & `picopt-3.3.0/tests/integration/test_images_dir.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Test comic format."""
 import platform
 import shutil
 
 from picopt import PROGRAM_NAME, cli
 from tests import IMAGES_DIR, get_test_dir
 
-
 __all__ = ()
 TMP_ROOT = get_test_dir()
 FNS = {
     "07themecamplist.pdf": (93676, 93676, ("pdf", 93676), ("pdf", 93676)),
     "test_animated_gif.gif": (16383, 16358, ("gif", 16358), ("webp", 11846)),
     "test_animated_png.png": (63435, 63435, ("png", 63435), ("webp", 54324)),
     "test_animated_webp.webp": (13610, 11854, ("webp", 11854), ("webp", 11854)),
@@ -77,41 +76,48 @@
             ),
             "eight.tif": (59640, 59640, ("png", 30564), ("webp", 24982)),
         }
     )
 
 
 class TestImagesDir:
+    """Test images dir."""
+
     def setup_method(self) -> None:
+        """Set up method."""
         self.teardown_method()
         shutil.copytree(IMAGES_DIR, TMP_ROOT)
         for name, sizes in FNS.items():
             path = TMP_ROOT / name
             assert path.stat().st_size == sizes[0]
 
     def teardown_method(self) -> None:
+        """Tear down method."""
         if TMP_ROOT.exists():
             shutil.rmtree(TMP_ROOT)
 
     def test_no_convert(self) -> None:
+        """Test no convert."""
         args = (PROGRAM_NAME, "-rvv", str(TMP_ROOT))
         res = cli.main(args)
         assert res
         for name, sizes in FNS.items():
             path = TMP_ROOT / name
             assert path.stat().st_size == sizes[1]
 
     def test_convert_to_png(self) -> None:
+        """Test convert to PNG."""
         args = (PROGRAM_NAME, "-rvvx", "TIFF", "-c", "PNG", str(TMP_ROOT))
         res = cli.main(args)
         assert res
         for name, sizes in FNS.items():
             path = (TMP_ROOT / name).with_suffix("." + sizes[2][0])
             assert path.stat().st_size == sizes[2][1]
 
     def test_convert_to_webp(self) -> None:
+        """Test convert to WEBP."""
         args = (PROGRAM_NAME, "-rvvx", "TIFF", "-c", "WEBP", str(TMP_ROOT))
         res = cli.main(args)
         assert res
         for name, sizes in FNS.items():
             path = (TMP_ROOT / name).with_suffix("." + sizes[3][0])
             assert path.stat().st_size == sizes[3][1]
```

### Comparing `picopt-3.2.5/tests/integration/test_old_timestamps.py` & `picopt-3.3.0/tests/integration/test_old_timestamps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Test comic format."""
 import shutil
 
 from picopt import PROGRAM_NAME, cli
-from picopt.old_timestamps import _OLD_TIMESTAMPS_NAME
+from picopt.old_timestamps import OLD_TIMESTAMPS_NAME
 from tests import IMAGES_DIR, get_test_dir
 
-
 __all__ = ()
 TMP_ROOT = get_test_dir()
 FN = "test_jpg.jpg"
 SRC_JPG = IMAGES_DIR / FN
 TMP_FN = str(TMP_ROOT / FN)
 FNS = {
     FN: (97373, 87913),
@@ -23,55 +22,62 @@
     "ignore": [],
     "recurse": True,
     "symlinks": True,
 }
 
 
 class TestContainersDir:
+    """Test containers dir."""
+
     @staticmethod
     def _assert_sizes(index, root=TMP_ROOT):
+        """Assert sizes."""
         for name, sizes in FNS.items():
             path = root / name
             assert path.stat().st_size == sizes[index]
 
     def setup_method(self) -> None:
+        """Set up method."""
         self.teardown_method()
         TMP_ROOT.mkdir(exist_ok=True)
         shutil.copy(SRC_JPG, TMP_ROOT)
         self._assert_sizes(0)
 
     def teardown_method(self) -> None:
-        if TMP_ROOT.exists():
-            shutil.rmtree(TMP_ROOT)
+        """Tear down method."""
+        shutil.rmtree(TMP_ROOT, ignore_errors=True)
 
     def test_old_timestamp_same_dir(self) -> None:
-        old_ts_path = TMP_ROOT / _OLD_TIMESTAMPS_NAME
+        """Test old timestamp in same dir."""
+        old_ts_path = TMP_ROOT / OLD_TIMESTAMPS_NAME
         old_ts_path.touch()
         args = (PROGRAM_NAME, "-rtvv", str(TMP_ROOT))
         res = cli.main(args)
         assert res
         assert not old_ts_path.exists()
         self._assert_sizes(0)
 
     def test_old_timestamp_child(self) -> None:
+        """Test old timestamp child."""
         child_root = TMP_ROOT / "child"
         child_root.mkdir(exist_ok=True)
-        shutil.copy(SRC_JPG, child_root)
-        old_ts_path = child_root / _OLD_TIMESTAMPS_NAME
+        shutil.move(TMP_ROOT / FN, child_root)
+        old_ts_path = child_root / OLD_TIMESTAMPS_NAME
         old_ts_path.touch()
-        args = (PROGRAM_NAME, "-rtvv", str(child_root))
+        args = (PROGRAM_NAME, "-rtvv", str(TMP_ROOT))
         res = cli.main(args)
         assert res
         assert not old_ts_path.exists()
-        self._assert_sizes(0)
+        self._assert_sizes(0, root=child_root)
 
     def test_old_timestamp_parent(self) -> None:
+        """Test old timestamp in parent."""
         child_root = TMP_ROOT / "child"
         child_root.mkdir(exist_ok=True)
-        shutil.copy(SRC_JPG, child_root)
-        old_ts_path = TMP_ROOT / _OLD_TIMESTAMPS_NAME
+        shutil.move(TMP_ROOT / FN, child_root)
+        old_ts_path = TMP_ROOT / OLD_TIMESTAMPS_NAME
         old_ts_path.touch()
         args = (PROGRAM_NAME, "-rtvv", str(child_root))
         res = cli.main(args)
         assert res
         assert old_ts_path.exists()
-        self._assert_sizes(0)
+        self._assert_sizes(0, root=child_root)
```

### Comparing `picopt-3.2.5/tests/integration/test_one_container.py` & `picopt-3.3.0/tests/integration/test_one_container.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 """Test comic format."""
 import shutil
-
 from platform import system
 
 from picopt import PROGRAM_NAME, cli
 from tests import CONTAINER_DIR, get_test_dir
 
-
 __all__ = ()
 TMP_ROOT = get_test_dir()
 FN = "test_zip.zip"
 SRC_CBZ = CONTAINER_DIR / FN
 
-if system() == "Darwin":
-    FNS = {
-        FN: (2974, 1871),
-    }
-else:
-    FNS = {
-        FN: (2974, 1917),
-    }
+FNS = {FN: (2974, 1871)} if system() == "Darwin" else {FN: (2974, 1917)}
 
 
 class TestContainersDir:
+    """Test containers dir."""
+
     def setup_method(self) -> None:
+        """Set up method."""
         self.teardown_method()
         TMP_ROOT.mkdir(exist_ok=True)
         shutil.copy(SRC_CBZ, TMP_ROOT)
         for name, sizes in FNS.items():
             path = TMP_ROOT / name
             assert path.stat().st_size == sizes[0]
 
     def teardown_method(self) -> None:
+        """Tear down method."""
         if TMP_ROOT.exists():
             shutil.rmtree(TMP_ROOT)
 
     def test_containers_no_convert(self) -> None:
+        """Test containers no convert."""
         args = (PROGRAM_NAME, "-x", "ZIP", str(TMP_ROOT / FN))
         res = cli.main(args)
         assert res
         for name, sizes in FNS.items():
             path = TMP_ROOT / name
             assert path.stat().st_size == sizes[1]
```

### Comparing `picopt-3.2.5/tests/test_files/containers/igp-twss.epub` & `picopt-3.3.0/tests/test_files/containers/igp-twss.epub`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/containers/test_cbr.cbr` & `picopt-3.3.0/tests/test_files/containers/test_cbr.cbr`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/containers/test_cbz.cbz` & `picopt-3.3.0/tests/test_files/containers/test_cbz.cbz`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/containers/test_rar.rar` & `picopt-3.3.0/tests/test_files/containers/test_rar.rar`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/containers/test_zip.zip` & `picopt-3.3.0/tests/test_files/containers/test_zip.zip`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/07themecamplist.pdf` & `picopt-3.3.0/tests/test_files/images/07themecamplist.pdf`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/eight.tif` & `picopt-3.3.0/tests/test_files/images/eight.tif`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/mri.tif` & `picopt-3.3.0/tests/test_files/images/mri.tif`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_animated_gif.gif` & `picopt-3.3.0/tests/test_files/images/test_animated_gif.gif`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_animated_png.png` & `picopt-3.3.0/tests/test_files/images/test_animated_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_animated_webp.webp` & `picopt-3.3.0/tests/test_files/images/test_animated_webp.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_bmp.bmp` & `picopt-3.3.0/tests/test_files/images/test_bmp.bmp`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_gif.gif` & `picopt-3.3.0/tests/test_files/images/test_gif.gif`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_jpg.jpg` & `picopt-3.3.0/tests/test_files/images/test_jpg.jpg`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_png.png` & `picopt-3.3.0/tests/test_files/images/test_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_png_16rgba.png` & `picopt-3.3.0/tests/test_files/images/test_png_16rgba.png`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_pnm.pnm` & `picopt-3.3.0/tests/test_files/images/test_pnm.pnm`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_pre-optimized_jpg.jpg` & `picopt-3.3.0/tests/test_files/images/test_pre-optimized_jpg.jpg`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_pre-optimized_png.png` & `picopt-3.3.0/tests/test_files/images/test_pre-optimized_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_webp_lossless.webp` & `picopt-3.3.0/tests/test_files/images/test_webp_lossless.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_webp_lossless_pre-optimized.webp` & `picopt-3.3.0/tests/test_files/images/test_webp_lossless_pre-optimized.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_webp_lossy.webp` & `picopt-3.3.0/tests/test_files/images/test_webp_lossy.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/images/test_webp_lossy_pre-optimized.webp` & `picopt-3.3.0/tests/test_files/images/test_webp_lossy_pre-optimized.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/test_files/invalid/test_mpeg.mpeg` & `picopt-3.3.0/tests/test_files/invalid/test_mpeg.mpeg`

 * *Files identical despite different names*

### Comparing `picopt-3.2.5/tests/unit/test_cli.py` & `picopt-3.3.0/tests/unit/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,54 +2,63 @@
 import shutil
 import sys
 
 from picopt import cli
 from picopt.handlers.zip import CBZ, Zip
 from tests import IMAGES_DIR, get_test_dir
 
-
 __all__ = ()  # hides module from pydocstring
 TYPE_NAME = "png"
 TMP_ROOT = get_test_dir()
 JPEG_SRC = IMAGES_DIR / "test_jpg.jpg"
 
 
 class TestCLI:
+    """Test CLI."""
+
     OLD_PATH = TMP_ROOT / "old.jpg"
 
     def setup_method(self) -> None:
+        """Set up method."""
         TMP_ROOT.mkdir(exist_ok=True)
 
     def teardown_method(self) -> None:
+        """Tear down method."""
         if TMP_ROOT.exists():
             shutil.rmtree(TMP_ROOT)
 
     def test_get_arguments(self) -> None:
+        """Test get arguments."""
         args = ("picopt", "-rqc", "PNG,WEBP", "-x", "CBZ,ZIP", "-bTLM", str(TMP_ROOT))
         arguments = cli.get_arguments(args)
         arguments = arguments.picopt
         assert arguments.verbose == 0
-        assert ("PNG", "WEBP") == arguments.convert_to
+        assert arguments.convert_to == ("PNG", "WEBP")
         assert arguments.formats is None
-        assert arguments._extra_formats == (CBZ.OUTPUT_FORMAT, Zip.OUTPUT_FORMAT)
+        assert arguments.computed.extra_formats == (
+            CBZ.OUTPUT_FORMAT_STR,
+            Zip.OUTPUT_FORMAT_STR,
+        )
         assert arguments.symlinks
         assert arguments.bigger
         assert not arguments.timestamps
         assert arguments.test
         assert arguments.list_only
         assert not arguments.keep_metadata
         assert arguments.paths[0] == str(TMP_ROOT)
 
     def test_main(self) -> None:
+        """Test main method."""
         shutil.copy(JPEG_SRC, self.OLD_PATH)
         old_size = self.OLD_PATH.stat().st_size
         sys.argv = ["picopt", str(self.OLD_PATH)]
         cli.main()
         assert self.OLD_PATH.is_file()
         assert self.OLD_PATH.stat().st_size < old_size
 
     def test_main_err(self) -> None:
+        """Test main errs."""
         sys.argv = ["picopt", "XXX"]
         try:
             cli.main()
         except SystemExit as exc:
-            assert exc.code == 1
+            assert exc.code == 1  # noqa PT017
```

### Comparing `picopt-3.2.5/tests/unit/test_png_bit_depth.py` & `picopt-3.3.0/tests/unit/test_png_bit_depth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """Test png bit depth utility module."""
 import sys
 
 from picopt.pillow.png_bit_depth import main, png_bit_depth
 from tests import IMAGES_DIR
 
-
 __all__ = ()  # hides module from pydocstring
 TEST_SRC_PATH = IMAGES_DIR / "test_png.png"
 TEST_SRC_PATH_16 = IMAGES_DIR / "test_png_16rgba.png"
 TEST_SRC_PATH_JPG = IMAGES_DIR / "test_jpg.jpg"
 
 
 def test_png_bit_depth() -> None:
+    """Test PNG bit depth."""
     res = png_bit_depth(TEST_SRC_PATH)
-    assert res == 8
+    assert res == 8  # noqa PLR2004
 
 
 def test_png_bit_depth_16() -> None:
+    """Test PNG bit depth 16."""
     res = png_bit_depth(TEST_SRC_PATH_16)
-    assert res == 16
+    assert res == 16  # noqa PLR2004
 
 
 def test_png_bit_depth_invalid() -> None:
+    """Test PNG bit depth invalid."""
     res = png_bit_depth(TEST_SRC_PATH_JPG)
     assert res is None
 
 
 def test_main() -> None:
+    """Test main."""
     sys.argv[1] = str(TEST_SRC_PATH)
     main()
```

### Comparing `picopt-3.2.5/setup.py` & `picopt-3.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,203 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: picopt
+Version: 3.3.0
+Summary: A multi format lossless image optimizer that uses external tools
+Home-page: https://github.com/ajslater/picopt
+License: GPL-3.0-only
+Keywords: image,png,jpg,cbz,cbr
+Author: AJ Slater
+Author-email: aj@slater.net
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
+Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
+Classifier: Typing :: Typed
+Requires-Dist: Pillow (>=9.0,<10.0)
+Requires-Dist: confuse (>=2.0.0,<3.0.0)
+Requires-Dist: humanize (>=4.0.0,<5.0.0)
+Requires-Dist: python-dateutil (>=2.8,<3.0)
+Requires-Dist: rarfile (>=4.0,<5.0)
+Requires-Dist: ruamel.yaml (>=0.17.16,<0.18.0)
+Requires-Dist: termcolor (>=2.0.1,<3.0.0)
+Requires-Dist: treestamps (>=0.4.0,<0.5.0)
+Project-URL: Documentation, https://github.com/ajslater/picopt
+Project-URL: Issues, https://github.com/ajslater/picopt/issues
+Project-URL: Source, https://github.com/ajslater/picopt
+Description-Content-Type: text/markdown
 
-packages = \
-['picopt',
- 'picopt.handlers',
- 'picopt.pillow',
- 'tests',
- 'tests.integration',
- 'tests.unit']
-
-package_data = \
-{'': ['*'],
- 'tests': ['test_files/containers/*',
-           'test_files/images/*',
-           'test_files/invalid/*']}
-
-install_requires = \
-['Pillow>=9.0,<10.0',
- 'confuse>=2.0.0,<3.0.0',
- 'humanize>=4.0.0,<5.0.0',
- 'python-dateutil>=2.8,<3.0',
- 'rarfile>=4.0,<5.0',
- 'ruamel.yaml>=0.17.16,<0.18.0',
- 'termcolor>=2.0.1,<3.0.0',
- 'treestamps>=0.3.3,<0.4.0']
-
-entry_points = \
-{'console_scripts': ['picopt = picopt.cli:main']}
-
-setup_kwargs = {
-    'name': 'picopt',
-    'version': '3.2.5',
-    'description': 'A multi format lossless image optimizer that uses external tools',
-    'long_description': '# picopt\n\nA multi-format, recursive, multiprocessor aware, command line lossless image optimizer utility that uses external tools to do the optimizing.\n\nPicopt depends on Python [PIL](http://www.pythonware.com/products/pil/) to identify files and Python [rarfile](https://pypi.python.org/pypi/rarfile) to open CBRs.\n\nPicopt will optionally drop hidden timestamps at the root of your image directories to avoid reoptimizing images picopt has already optimized.\n\nThe actual image optimization is best accomplished by external programs.\n\n## <a name="philosophy">Conversion Philosophy</a>\n\n### Lossy Images\n\nJPEG & Lossy WebP images are likely the best and most practical lossy image formats. Converting lossy images rarely makes sense and so picopt only optimizes them in their current format.\n\n### Lossless Images\n\nLossless WebP images are smaller than PNG, much smaller than GIF and, of course, a great deal smaller thein uncompressed bitmaps like BMP. As such the best practice is probably to convert all lossless images to WebP Lossless as now all major browsers support it. The only downside is that decoding WebP Lossless takes on average 50% more CPU than PNG.\n\n### Sequenced Images\n\nSequenced Images, like animated GIFs and WebP, most of the time, should be converted to a compressed video format like HEVC or VP9. There are several situations where this is impractical and so Animated WebP is now a good substitute.\n\n### Conversion\n\nBy default picopt does not convert images between formats. You must turn on conversion to PNG or WebP explicitly.\n\n## <a name="formats">Formats</a>\n\n- By default picopt will optimize GIF, JPEG, PNG and WEBP images.\n- Picopt can optionally optimize ZIP, ePub, and CBZ containers.\n- Picopt can be told to convert lossless images such as BPM, PPM, GIF, TIFF into PNG, and all of the mentioned lossless formats into WebP.\n- Picopt can convert Animated GIFs into Animated WebP files.\n- Picopt can convert Animated PNGs (APNG) into Animated WebP files, but does not optimize APNG as APNG.\n- Picopt can convert RAR files into Zipfiles and CBR files into CBZ files.\n\n## <a name="programs">External Programs</a>\n\nPicopt will perform some minor optimization on most formats natively without using external programs, but this is not very good compared to the optimizations external programs can provide.\n\n### JPEG\n\nTo optimize JPEG images. Picopt needs one of [mozjpeg](https://github.com/mozilla/mozjpeg) or [jpegtran](http://jpegclub.org/jpegtran/) on the path. in order of preference.\n\n### PNG\n\nTo optimize PNG images or convert other lossless formats to PNG picopt requires either [optipng](http://optipng.sourceforge.net/) or [pngout](http://advsys.net/ken/utils.htm) be on the path. Optipng provides the most advantage, but best results will be had by using pngout as well.\n\n### Animated GIF\n\nAnimated GIFs are optimized with [gifsicle](http://www.lcdf.org/gifsicle/) if it is available.\n\n### WebP\n\nWebP lossless & lossy formats are optimized with [cwebp](https://developers.google.com/speed/webp/docs/cwebp).\n\n### EPub\n\nEPub Books are zip files that often contain images and picopt unpacks and repacks this format natively. Images within the epub are handled by other programs. EPub optimization is not turned on by default.\nEPub contents are never converted to other formats because it would break internal references to them.\n\n### CBZ & CBR\n\nPicopt uncompresses, optimizes and rezips [comic book archive files](https://en.wikipedia.org/wiki/Comic_book_archive). Be aware that CBR rar archives may only be rezipped into CBZs instead of CBR. Comic book archive optimization is not turned on by default to prevent surprises.\n\n## <a name="install">Install</a>\n\n### System Dependencies\n\npicopt requires several external system dependencies to run. We must install these first\n\n#### macOS\n\n    brew install webp mozjpeg optipng jonof/kenutils/pngout gifsicle\n\n    ln -s $(brew --prefix)/opt/mozjpeg/bin/jpegtran /usr/local/bin/mozjpeg\n\nUnfortunately hombrew\'s `webp` formula does not yet install the gif2webp tool that picopt uses for converting animated gifs to animated webps.\nYou may manually download it and put it in your path at [Google\'s WebP developer website](https://developers.google.com/speed/webp/download)\n\n#### Debian / Ubuntu\n\n    apt-get install optipng gifsicle python-imaging webp\n\nif you don\'t want to install mozjpeg using the instructions below then use jpegtran:\n\n    apt-get install libjpeg-progs\n\n#### Redhat / Fedora\n\n    yum install optipng gifsicle python-imaging libwebp-tools\n\nif you don\'t want to install mozjpeg using the instructions below then use jpegtran:\n\n    yum install libjpeg-progs\n\n#### MozJPEG\n\nmozjpeg offers better compression than libjpeg-progs jpegtran. It may or\nmay not be packaged for your \\*nix, but even when it is, picopt requires that its separately compiled version of jpegtran be symlinked to \'mozjpeg\' somewhere in the path.\n\nInstructions for installing on macOS are given above.\nSome near recent binaries for Windows and Debian x86 [can be found here](https://mozjpeg.codelove.de/binaries.html).\nMost Linux distributions still require a more manual install as elucidated here on [Casey Hoffer\'s blog](https://www.caseyhofford.com/2019/05/01/improved-image-compression-install-mozjpeg-on-ubuntu-server/)\n\n#### pngout\n\npngout is a useful compression to use after optipng. It is not packaged for linux, but you may find the latest binary version [on JonoF\'s site](http://www.jonof.id.au/kenutils). Picopt looks for the binary to be called `pngout`\n\n### Picopt python package\n\n    pip install picopt\n\n## <a name="usage">Usage Examples</a>\n\nOptimize all JPEG files in a directory:\n\n    picopt *.jpg\n\nOptimize all files and recurse directories:\n\n    picopt -r *\n\nOptimize files, recurse directories, also optimize ePub & CBZ containers, convert lossless images into WEBP, convert CBR into CBZ.\n\n    picopt -rx EPUB,CBR,CBZ -c WEBP,CBZ *\n\nOptimize files and recurse directories AND optimize comic book archives:\n\n    picopt -rx CBZ *\n\nOptimize comic directory recursively. Convert CBRs to CBZ. Convert lossless images, including TIFF, to lossless WEBP. Do not follow symlinks. Set timestamps.\n\n    picopt -rStc CBZ,WEBP -x TIFF,CBR,CBZ /Volumes/Media/Comics\n\nOptimize all files, but only JPEG format files:\n\n    picopt -f JPEG *\n\nOptimize files and containers, but not JPEGS:\n\n    picopt -f GIF,PNG,WEBP,ZIP,CBZ,EPUB *\n\nOptimize files, but not animated gifs:\n\n    picopt -f PNG,WEBP,ZIP,CBZ,EPUB *\n\nJust list files picopt.py would try to optimize:\n\n    picopt -L *\n\nOptimize pictures in my iPhoto library, but only after the last time I did this, skipping symlinks to avoid duplicate work. Also drop a timestamp file so I don\'t have to remember the last time I did this:\n\n    picopt -rSt -D \'2013 June 1 14:00\' \'Pictures/iPhoto Library\'\n\n## <a name="package">Packages</a>\n\n- [PyPI](https://pypi.python.org/pypi/picopt/)\n- [Arch Linux](https://aur.archlinux.org/packages/picopt/)\n\n## <a name="alternatives">Alternatives</a>\n\n[imagemin](https://github.com/imagemin/imagemin-cli) looks to be an all in one cli and gui solution with bundled libraries, so no awkward dependencies.\n[Imageoptim](http://imageoptim.com/) is an all-in-one OS X GUI image optimizer. Imageoptim command line usage is possible with [an external program](https://code.google.com/p/imageoptim/issues/detail?can=2&start=0&num=100&q=&colspec=ID%20Type%20Status%20Priority%20Milestone%20Owner%20Summary%20Stars&groupby=&sort=&id=39).\n',
-    'author': 'AJ Slater',
-    'author_email': 'aj@slater.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ajslater/picopt',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+# picopt
 
+A multi-format, recursive, multiprocessor aware, command line lossless image optimizer utility that uses external tools to do the optimizing.
+
+Picopt depends on Python [PIL](http://www.pythonware.com/products/pil/) to identify files and Python [rarfile](https://pypi.python.org/pypi/rarfile) to open CBRs.
+
+Picopt will optionally drop hidden timestamps at the root of your image directories to avoid reoptimizing images picopt has already optimized.
+
+The actual image optimization is best accomplished by external programs.
+
+## <a name="philosophy">Conversion Philosophy</a>
+
+### Lossy Images
+
+JPEG & Lossy WebP images are likely the best and most practical lossy image formats. Converting lossy images rarely makes sense and so picopt only optimizes them in their current format.
+
+### Lossless Images
+
+Lossless WebP images are smaller than PNG, much smaller than GIF and, of course, a great deal smaller thein uncompressed bitmaps like BMP. As such the best practice is probably to convert all lossless images to WebP Lossless as now all major browsers support it. The only downside is that decoding WebP Lossless takes on average 50% more CPU than PNG.
+
+### Sequenced Images
+
+Sequenced Images, like animated GIFs and WebP, most of the time, should be converted to a compressed video format like HEVC or VP9. There are several situations where this is impractical and so Animated WebP is now a good substitute.
+
+### Conversion
+
+By default picopt does not convert images between formats. You must turn on conversion to PNG or WebP explicitly.
+
+## <a name="formats">Formats</a>
+
+- By default picopt will optimize GIF, JPEG, PNG and WEBP images.
+- Picopt can optionally optimize ZIP, ePub, and CBZ containers.
+- Picopt can be told to convert lossless images such as BPM, PPM, GIF, TIFF into PNG, and all of the mentioned lossless formats into WebP.
+- Picopt can convert Animated GIFs into Animated WebP files.
+- Picopt can convert Animated PNGs (APNG) into Animated WebP files, but does not optimize APNG as APNG.
+- Picopt can convert RAR files into Zipfiles and CBR files into CBZ files.
+
+## <a name="programs">External Programs</a>
+
+Picopt will perform some minor optimization on most formats natively without using external programs, but this is not very good compared to the optimizations external programs can provide.
+
+### JPEG
+
+To optimize JPEG images. Picopt needs one of [mozjpeg](https://github.com/mozilla/mozjpeg) or [jpegtran](http://jpegclub.org/jpegtran/) on the path. in order of preference.
+
+### PNG
+
+To optimize PNG images or convert other lossless formats to PNG picopt requires either [optipng](http://optipng.sourceforge.net/) or [pngout](http://advsys.net/ken/utils.htm) be on the path. Optipng provides the most advantage, but best results will be had by using pngout as well.
+
+### Animated GIF
+
+Animated GIFs are optimized with [gifsicle](http://www.lcdf.org/gifsicle/) if it is available.
+
+### WebP
+
+WebP lossless & lossy formats are optimized with [cwebp](https://developers.google.com/speed/webp/docs/cwebp).
+
+### EPub
+
+EPub Books are zip files that often contain images and picopt unpacks and repacks this format natively. Images within the epub are handled by other programs. EPub optimization is not turned on by default.
+EPub contents are never converted to other formats because it would break internal references to them.
+
+### CBZ & CBR
+
+Picopt uncompresses, optimizes and rezips [comic book archive files](https://en.wikipedia.org/wiki/Comic_book_archive). Be aware that CBR rar archives may only be rezipped into CBZs instead of CBR. Comic book archive optimization is not turned on by default to prevent surprises.
+
+## <a name="install">Install</a>
+
+### System Dependencies
+
+picopt requires several external system dependencies to run. We must install these first
+
+#### macOS
+
+    brew install webp mozjpeg optipng jonof/kenutils/pngout gifsicle
+
+    ln -s $(brew --prefix)/opt/mozjpeg/bin/jpegtran /usr/local/bin/mozjpeg
+
+Unfortunately hombrew's `webp` formula does not yet install the gif2webp tool that picopt uses for converting animated gifs to animated webps.
+You may manually download it and put it in your path at [Google's WebP developer website](https://developers.google.com/speed/webp/download)
+
+#### Debian / Ubuntu
+
+    apt-get install optipng gifsicle python-imaging webp
+
+if you don't want to install mozjpeg using the instructions below then use jpegtran:
+
+    apt-get install libjpeg-progs
+
+#### Redhat / Fedora
+
+    yum install optipng gifsicle python-imaging libwebp-tools
+
+if you don't want to install mozjpeg using the instructions below then use jpegtran:
+
+    yum install libjpeg-progs
+
+#### MozJPEG
+
+mozjpeg offers better compression than libjpeg-progs jpegtran. It may or
+may not be packaged for your \*nix, but even when it is, picopt requires that its separately compiled version of jpegtran be symlinked to 'mozjpeg' somewhere in the path.
+
+Instructions for installing on macOS are given above.
+Some near recent binaries for Windows and Debian x86 [can be found here](https://mozjpeg.codelove.de/binaries.html).
+Most Linux distributions still require a more manual install as elucidated here on [Casey Hoffer's blog](https://www.caseyhofford.com/2019/05/01/improved-image-compression-install-mozjpeg-on-ubuntu-server/)
+
+#### pngout
+
+pngout is a useful compression to use after optipng. It is not packaged for linux, but you may find the latest binary version [on JonoF's site](http://www.jonof.id.au/kenutils). Picopt looks for the binary to be called `pngout`
+
+### Picopt python package
+
+    pip install picopt
+
+## <a name="usage">Usage Examples</a>
+
+Optimize all JPEG files in a directory:
+
+    picopt *.jpg
+
+Optimize all files and recurse directories:
+
+    picopt -r *
+
+Optimize files, recurse directories, also optimize ePub & CBZ containers, convert lossless images into WEBP, convert CBR into CBZ.
+
+    picopt -rx EPUB,CBR,CBZ -c WEBP,CBZ *
+
+Optimize files and recurse directories AND optimize comic book archives:
+
+    picopt -rx CBZ *
+
+Optimize comic directory recursively. Convert CBRs to CBZ. Convert lossless images, including TIFF, to lossless WEBP. Do not follow symlinks. Set timestamps.
+
+    picopt -rStc CBZ,WEBP -x TIFF,CBR,CBZ /Volumes/Media/Comics
+
+Optimize all files, but only JPEG format files:
+
+    picopt -f JPEG *
+
+Optimize files and containers, but not JPEGS:
+
+    picopt -f GIF,PNG,WEBP,ZIP,CBZ,EPUB *
+
+Optimize files, but not animated gifs:
+
+    picopt -f PNG,WEBP,ZIP,CBZ,EPUB *
+
+Just list files picopt.py would try to optimize:
+
+    picopt -L *
+
+Optimize pictures in my iPhoto library, but only after the last time I did this, skipping symlinks to avoid duplicate work. Also drop a timestamp file so I don't have to remember the last time I did this:
+
+    picopt -rSt -D '2013 June 1 14:00' 'Pictures/iPhoto Library'
+
+## <a name="package">Packages</a>
+
+- [PyPI](https://pypi.python.org/pypi/picopt/)
+- [Arch Linux](https://aur.archlinux.org/packages/picopt/)
+
+## <a name="alternatives">Alternatives</a>
+
+[imagemin](https://github.com/imagemin/imagemin-cli) looks to be an all in one cli and gui solution with bundled libraries, so no awkward dependencies.
+[Imageoptim](http://imageoptim.com/) is an all-in-one OS X GUI image optimizer. Imageoptim command line usage is possible with [an external program](https://code.google.com/p/imageoptim/issues/detail?can=2&start=0&num=100&q=&colspec=ID%20Type%20Status%20Priority%20Milestone%20Owner%20Summary%20Stars&groupby=&sort=&id=39).
 
-setup(**setup_kwargs)
```

