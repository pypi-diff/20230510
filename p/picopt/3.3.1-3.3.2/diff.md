# Comparing `tmp/picopt-3.3.1.tar.gz` & `tmp/picopt-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picopt-3.3.1.tar", max compression
+gzip compressed data, was "picopt-3.3.2.tar", max compression
```

## Comparing `picopt-3.3.1.tar` & `picopt-3.3.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     7482 2023-05-10 04:15:56.126181 picopt-3.3.1/README.md
--rw-r--r--   0        0        0       64 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/__init__.py
--rw-r--r--   0        0        0     7124 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/cli.py
--rw-r--r--   0        0        0    14506 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/config.py
--rw-r--r--   0        0        0      286 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/config_default.yaml
--rw-r--r--   0        0        0      457 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/configurable.py
--rw-r--r--   0        0        0      501 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/data.py
--rw-r--r--   0        0        0       25 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/__init__.py
--rw-r--r--   0        0        0     3478 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/container.py
--rw-r--r--   0        0        0     5508 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/factory.py
--rw-r--r--   0        0        0     1360 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/gif.py
--rw-r--r--   0        0        0     5667 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/handler.py
--rw-r--r--   0        0        0     2988 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/image.py
--rw-r--r--   0        0        0     1660 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/jpeg.py
--rw-r--r--   0        0        0     1902 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/png.py
--rw-r--r--   0        0        0     4294 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/webp.py
--rw-r--r--   0        0        0     4468 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/webp_animated.py
--rw-r--r--   0        0        0     4042 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/handlers/zip.py
--rw-r--r--   0        0        0     2276 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/old_timestamps.py
--rw-r--r--   0        0        0       22 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/pillow/__init__.py
--rw-r--r--   0        0        0      777 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/pillow/header.py
--rwxr-xr-x   0        0        0     1052 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/pillow/png_bit_depth.py
--rwxr-xr-x   0        0        0      996 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/pillow/webp_lossless.py
--rw-r--r--   0        0        0     2599 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/stats.py
--rw-r--r--   0        0        0    15806 2023-05-10 04:15:56.130181 picopt-3.3.1/picopt/walk.py
--rw-r--r--   0        0        0     4173 2023-05-10 04:15:56.130181 picopt-3.3.1/pyproject.toml
--rw-r--r--   0        0        0      560 2023-05-10 04:15:56.130181 picopt-3.3.1/tests/__init__.py
--rw-r--r--   0        0        0       22 2023-05-10 04:15:56.130181 picopt-3.3.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     2813 2023-05-10 04:15:56.130181 picopt-3.3.1/tests/integration/test_containers.py
--rw-r--r--   0        0        0     4447 2023-05-10 04:15:56.130181 picopt-3.3.1/tests/integration/test_images_dir.py
--rw-r--r--   0        0        0     2454 2023-05-10 04:15:56.130181 picopt-3.3.1/tests/integration/test_old_timestamps.py
--rw-r--r--   0        0        0     1140 2023-05-10 04:15:56.130181 picopt-3.3.1/tests/integration/test_one_container.py
--rw-r--r--   0        0        0     5084 2023-05-10 04:15:56.130181 picopt-3.3.1/tests/integration/test_timestamps.py
--rw-r--r--   0        0        0   292448 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/containers/igp-twss.epub
--rw-r--r--   0        0        0    93725 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/containers/test_cbr.cbr
--rw-r--r--   0        0        0    93408 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/containers/test_cbz.cbz
--rw-r--r--   0        0        0    93675 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/containers/test_rar.rar
--rw-r--r--   0        0        0     2974 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/containers/test_zip.zip
--rw-r--r--   0        0        0    93676 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/images/07themecamplist.pdf
--rw-r--r--   0        0        0    59640 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/images/eight.tif
--rw-r--r--   0        0        0   230578 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/images/mri.tif
--rw-r--r--   0        0        0    16383 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/images/test_animated_gif.gif
--rw-r--r--   0        0        0    63435 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/images/test_animated_png.png
--rw-r--r--   0        0        0    13610 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/images/test_animated_webp.webp
--rw-r--r--   0        0        0   141430 2023-05-10 04:15:56.134181 picopt-3.3.1/tests/test_files/images/test_bmp.bmp
--rw-r--r--   0        0        0   138952 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_gif.gif
--rw-r--r--   0        0        0    97373 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_jpg.jpg
--rw-r--r--   0        0        0     7967 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_png.png
--rw-r--r--   0        0        0     3435 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_png_16rgba.png
--rw-r--r--   0        0        0    27661 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_pnm.pnm
--rw-r--r--   0        0        0    22664 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_pre-optimized_jpg.jpg
--rw-r--r--   0        0        0   256572 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_pre-optimized_png.png
--rw-r--r--   0        0        0        6 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_txt.txt
--rw-r--r--   0        0        0     5334 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_webp_lossless.webp
--rw-r--r--   0        0        0     8914 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_webp_lossless_pre-optimized.webp
--rw-r--r--   0        0        0     2764 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_webp_lossy.webp
--rw-r--r--   0        0        0     1508 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/images/test_webp_lossy_pre-optimized.webp
--rw-r--r--   0        0        0        3 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/invalid/test_invalid_cbr.cbr
--rw-r--r--   0        0        0        3 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/invalid/test_invalid_cbz.cbz
--rw-r--r--   0        0        0        0 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/invalid/test_invalid_gif.gif
--rw-r--r--   0        0        0        0 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/invalid/test_invalid_jpg.jpg
--rw-r--r--   0        0        0        0 2023-05-10 04:15:56.138181 picopt-3.3.1/tests/test_files/invalid/test_invalid_png.png
--rw-r--r--   0        0        0   879952 2023-05-10 04:15:56.142181 picopt-3.3.1/tests/test_files/invalid/test_mpeg.mpeg
--rw-r--r--   0        0        0       80 2023-05-10 04:15:56.142181 picopt-3.3.1/tests/test_files/invalid/test_rar.rar
--rw-r--r--   0        0        0      167 2023-05-10 04:15:56.142181 picopt-3.3.1/tests/test_files/invalid/test_zip.zip
--rw-r--r--   0        0        0       18 2023-05-10 04:15:56.142181 picopt-3.3.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     1923 2023-05-10 04:15:56.142181 picopt-3.3.1/tests/unit/test_cli.py
--rw-r--r--   0        0        0      871 2023-05-10 04:15:56.142181 picopt-3.3.1/tests/unit/test_png_bit_depth.py
--rw-r--r--   0        0        0     9059 1970-01-01 00:00:00.000000 picopt-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     7482 2023-05-10 05:19:33.371107 picopt-3.3.2/README.md
+-rw-r--r--   0        0        0       64 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/__init__.py
+-rw-r--r--   0        0        0     7124 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/cli.py
+-rw-r--r--   0        0        0    14506 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/config.py
+-rw-r--r--   0        0        0      286 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/config_default.yaml
+-rw-r--r--   0        0        0      457 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/configurable.py
+-rw-r--r--   0        0        0      501 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/data.py
+-rw-r--r--   0        0        0       25 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/handlers/__init__.py
+-rw-r--r--   0        0        0     3478 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/handlers/container.py
+-rw-r--r--   0        0        0     5508 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/handlers/factory.py
+-rw-r--r--   0        0        0     1360 2023-05-10 05:19:33.375107 picopt-3.3.2/picopt/handlers/gif.py
+-rw-r--r--   0        0        0     5667 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/handlers/handler.py
+-rw-r--r--   0        0        0     2988 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/handlers/image.py
+-rw-r--r--   0        0        0     1660 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/handlers/jpeg.py
+-rw-r--r--   0        0        0     1902 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/handlers/png.py
+-rw-r--r--   0        0        0     4294 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/handlers/webp.py
+-rw-r--r--   0        0        0     4468 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/handlers/webp_animated.py
+-rw-r--r--   0        0        0     4042 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/handlers/zip.py
+-rw-r--r--   0        0        0     2276 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/old_timestamps.py
+-rw-r--r--   0        0        0       22 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/pillow/__init__.py
+-rw-r--r--   0        0        0      777 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/pillow/header.py
+-rwxr-xr-x   0        0        0     1052 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/pillow/png_bit_depth.py
+-rwxr-xr-x   0        0        0      996 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/pillow/webp_lossless.py
+-rw-r--r--   0        0        0     2599 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/stats.py
+-rw-r--r--   0        0        0    15806 2023-05-10 05:19:33.379107 picopt-3.3.2/picopt/walk.py
+-rw-r--r--   0        0        0     4173 2023-05-10 05:19:33.379107 picopt-3.3.2/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2813 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/integration/test_containers.py
+-rw-r--r--   0        0        0     4447 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/integration/test_images_dir.py
+-rw-r--r--   0        0        0     2454 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/integration/test_old_timestamps.py
+-rw-r--r--   0        0        0     1140 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/integration/test_one_container.py
+-rw-r--r--   0        0        0     5084 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/integration/test_timestamps.py
+-rw-r--r--   0        0        0   292448 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/test_files/containers/igp-twss.epub
+-rw-r--r--   0        0        0    93725 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/test_files/containers/test_cbr.cbr
+-rw-r--r--   0        0        0    93408 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/test_files/containers/test_cbz.cbz
+-rw-r--r--   0        0        0    93675 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/test_files/containers/test_rar.rar
+-rw-r--r--   0        0        0     2974 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/test_files/containers/test_zip.zip
+-rw-r--r--   0        0        0    93676 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/test_files/images/07themecamplist.pdf
+-rw-r--r--   0        0        0    59640 2023-05-10 05:19:33.379107 picopt-3.3.2/tests/test_files/images/eight.tif
+-rw-r--r--   0        0        0   230578 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/mri.tif
+-rw-r--r--   0        0        0    16383 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_animated_gif.gif
+-rw-r--r--   0        0        0    63435 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_animated_png.png
+-rw-r--r--   0        0        0    13610 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_animated_webp.webp
+-rw-r--r--   0        0        0   141430 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_bmp.bmp
+-rw-r--r--   0        0        0   138952 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_gif.gif
+-rw-r--r--   0        0        0    97373 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_jpg.jpg
+-rw-r--r--   0        0        0     7967 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_png.png
+-rw-r--r--   0        0        0     3435 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_png_16rgba.png
+-rw-r--r--   0        0        0    27661 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_pnm.pnm
+-rw-r--r--   0        0        0    22664 2023-05-10 05:19:33.383107 picopt-3.3.2/tests/test_files/images/test_pre-optimized_jpg.jpg
+-rw-r--r--   0        0        0   256572 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/images/test_pre-optimized_png.png
+-rw-r--r--   0        0        0        6 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/images/test_txt.txt
+-rw-r--r--   0        0        0     5334 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/images/test_webp_lossless.webp
+-rw-r--r--   0        0        0     8914 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/images/test_webp_lossless_pre-optimized.webp
+-rw-r--r--   0        0        0     2764 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/images/test_webp_lossy.webp
+-rw-r--r--   0        0        0     1508 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/images/test_webp_lossy_pre-optimized.webp
+-rw-r--r--   0        0        0        3 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/invalid/test_invalid_cbr.cbr
+-rw-r--r--   0        0        0        3 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/invalid/test_invalid_cbz.cbz
+-rw-r--r--   0        0        0        0 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/invalid/test_invalid_gif.gif
+-rw-r--r--   0        0        0        0 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/invalid/test_invalid_jpg.jpg
+-rw-r--r--   0        0        0        0 2023-05-10 05:19:33.387107 picopt-3.3.2/tests/test_files/invalid/test_invalid_png.png
+-rw-r--r--   0        0        0   879952 2023-05-10 05:19:33.391107 picopt-3.3.2/tests/test_files/invalid/test_mpeg.mpeg
+-rw-r--r--   0        0        0       80 2023-05-10 05:19:33.391107 picopt-3.3.2/tests/test_files/invalid/test_rar.rar
+-rw-r--r--   0        0        0      167 2023-05-10 05:19:33.391107 picopt-3.3.2/tests/test_files/invalid/test_zip.zip
+-rw-r--r--   0        0        0       18 2023-05-10 05:19:33.391107 picopt-3.3.2/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1923 2023-05-10 05:19:33.391107 picopt-3.3.2/tests/unit/test_cli.py
+-rw-r--r--   0        0        0      871 2023-05-10 05:19:33.391107 picopt-3.3.2/tests/unit/test_png_bit_depth.py
+-rw-r--r--   0        0        0     9059 1970-01-01 00:00:00.000000 picopt-3.3.2/PKG-INFO
```

### Comparing `picopt-3.3.1/README.md` & `picopt-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/cli.py` & `picopt-3.3.2/picopt/cli.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/config.py` & `picopt-3.3.2/picopt/config.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/container.py` & `picopt-3.3.2/picopt/handlers/container.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/factory.py` & `picopt-3.3.2/picopt/handlers/factory.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/gif.py` & `picopt-3.3.2/picopt/handlers/gif.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/handler.py` & `picopt-3.3.2/picopt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/image.py` & `picopt-3.3.2/picopt/handlers/image.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/jpeg.py` & `picopt-3.3.2/picopt/handlers/jpeg.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/png.py` & `picopt-3.3.2/picopt/handlers/png.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/webp.py` & `picopt-3.3.2/picopt/handlers/webp.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/webp_animated.py` & `picopt-3.3.2/picopt/handlers/webp_animated.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/handlers/zip.py` & `picopt-3.3.2/picopt/handlers/zip.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/old_timestamps.py` & `picopt-3.3.2/picopt/old_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/pillow/header.py` & `picopt-3.3.2/picopt/pillow/header.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/pillow/png_bit_depth.py` & `picopt-3.3.2/picopt/pillow/png_bit_depth.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/pillow/webp_lossless.py` & `picopt-3.3.2/picopt/pillow/webp_lossless.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/stats.py` & `picopt-3.3.2/picopt/stats.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/picopt/walk.py` & `picopt-3.3.2/picopt/walk.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/pyproject.toml` & `picopt-3.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = ["poetry.core.masonry.api"]
 
 [tool.poetry]
 name = "picopt"
-version = "3.3.1"
+version = "3.3.2"
 description = "A multi format lossless image optimizer that uses external tools"
 license = "GPL-3.0-only"
 authors = ["AJ Slater <aj@slater.net>"]
 readme = "README.md"
 homepage = "https://github.com/ajslater/picopt"
 documentation = "https://github.com/ajslater/picopt"
 keywords = ["image", "png", "jpg", "cbz", "cbr"]
@@ -30,15 +30,15 @@
 python = "^3.9"
 confuse = "^2.0.0"
 humanize = "^4.0.0"
 python-dateutil = "^2.8"
 rarfile = "^4.0"
 "ruamel.yaml" = "^0.17.16"
 termcolor = "^2.0.1"
-treestamps = "^0.4.1"
+treestamps = "^0.4.2"
 Pillow = "^9.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 codespell = "^2.1.0"
 coverage = { extras = ["toml"], version = "^7.0" }
 neovim = "^0.3.1"
```

### Comparing `picopt-3.3.1/tests/__init__.py` & `picopt-3.3.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/integration/test_containers.py` & `picopt-3.3.2/tests/integration/test_containers.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/integration/test_images_dir.py` & `picopt-3.3.2/tests/integration/test_images_dir.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/integration/test_old_timestamps.py` & `picopt-3.3.2/tests/integration/test_old_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/integration/test_one_container.py` & `picopt-3.3.2/tests/integration/test_one_container.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/integration/test_timestamps.py` & `picopt-3.3.2/tests/integration/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/containers/igp-twss.epub` & `picopt-3.3.2/tests/test_files/containers/igp-twss.epub`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/containers/test_cbr.cbr` & `picopt-3.3.2/tests/test_files/containers/test_cbr.cbr`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/containers/test_cbz.cbz` & `picopt-3.3.2/tests/test_files/containers/test_cbz.cbz`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/containers/test_rar.rar` & `picopt-3.3.2/tests/test_files/containers/test_rar.rar`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/containers/test_zip.zip` & `picopt-3.3.2/tests/test_files/containers/test_zip.zip`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/07themecamplist.pdf` & `picopt-3.3.2/tests/test_files/images/07themecamplist.pdf`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/eight.tif` & `picopt-3.3.2/tests/test_files/images/eight.tif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/mri.tif` & `picopt-3.3.2/tests/test_files/images/mri.tif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_animated_gif.gif` & `picopt-3.3.2/tests/test_files/images/test_animated_gif.gif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_animated_png.png` & `picopt-3.3.2/tests/test_files/images/test_animated_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_animated_webp.webp` & `picopt-3.3.2/tests/test_files/images/test_animated_webp.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_bmp.bmp` & `picopt-3.3.2/tests/test_files/images/test_bmp.bmp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_gif.gif` & `picopt-3.3.2/tests/test_files/images/test_gif.gif`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_jpg.jpg` & `picopt-3.3.2/tests/test_files/images/test_jpg.jpg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_png.png` & `picopt-3.3.2/tests/test_files/images/test_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_png_16rgba.png` & `picopt-3.3.2/tests/test_files/images/test_png_16rgba.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_pnm.pnm` & `picopt-3.3.2/tests/test_files/images/test_pnm.pnm`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_pre-optimized_jpg.jpg` & `picopt-3.3.2/tests/test_files/images/test_pre-optimized_jpg.jpg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_pre-optimized_png.png` & `picopt-3.3.2/tests/test_files/images/test_pre-optimized_png.png`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_webp_lossless.webp` & `picopt-3.3.2/tests/test_files/images/test_webp_lossless.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_webp_lossless_pre-optimized.webp` & `picopt-3.3.2/tests/test_files/images/test_webp_lossless_pre-optimized.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_webp_lossy.webp` & `picopt-3.3.2/tests/test_files/images/test_webp_lossy.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/images/test_webp_lossy_pre-optimized.webp` & `picopt-3.3.2/tests/test_files/images/test_webp_lossy_pre-optimized.webp`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/test_files/invalid/test_mpeg.mpeg` & `picopt-3.3.2/tests/test_files/invalid/test_mpeg.mpeg`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/unit/test_cli.py` & `picopt-3.3.2/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/tests/unit/test_png_bit_depth.py` & `picopt-3.3.2/tests/unit/test_png_bit_depth.py`

 * *Files identical despite different names*

### Comparing `picopt-3.3.1/PKG-INFO` & `picopt-3.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picopt
-Version: 3.3.1
+Version: 3.3.2
 Summary: A multi format lossless image optimizer that uses external tools
 Home-page: https://github.com/ajslater/picopt
 License: GPL-3.0-only
 Keywords: image,png,jpg,cbz,cbr
 Author: AJ Slater
 Author-email: aj@slater.net
 Requires-Python: >=3.9,<4.0
@@ -25,15 +25,15 @@
 Requires-Dist: Pillow (>=9.0,<10.0)
 Requires-Dist: confuse (>=2.0.0,<3.0.0)
 Requires-Dist: humanize (>=4.0.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8,<3.0)
 Requires-Dist: rarfile (>=4.0,<5.0)
 Requires-Dist: ruamel.yaml (>=0.17.16,<0.18.0)
 Requires-Dist: termcolor (>=2.0.1,<3.0.0)
-Requires-Dist: treestamps (>=0.4.1,<0.5.0)
+Requires-Dist: treestamps (>=0.4.2,<0.5.0)
 Project-URL: Documentation, https://github.com/ajslater/picopt
 Project-URL: Issues, https://github.com/ajslater/picopt/issues
 Project-URL: Source, https://github.com/ajslater/picopt
 Description-Content-Type: text/markdown
 
 # picopt
```

