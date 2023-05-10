# Comparing `tmp/types-Pillow-9.5.0.2.tar.gz` & `tmp/types-Pillow-9.5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Pillow-9.5.0.2.tar", last modified: Wed Apr 26 18:18:47 2023, max compression
+gzip compressed data, was "types-Pillow-9.5.0.3.tar", last modified: Wed May 10 09:14:56 2023, max compression
```

## Comparing `types-Pillow-9.5.0.2.tar` & `types-Pillow-9.5.0.3.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-26 18:18:43.000000 types-Pillow-9.5.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 18:18:43.000000 types-Pillow-9.5.0.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/PIL-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/BdfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/BlpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/BmpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/BufrStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ContainerIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/CurImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/DcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/DdsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/EpsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ExifTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FitsStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FliImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FpxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FtexImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GbrImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GdImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GifImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GimpGradientFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GimpPaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GribStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/Hdf5StubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/IcnsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/IcoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/Image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageChops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageCms.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageColor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageDraw2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageEnhance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageFilter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageFont.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageGrab.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageMath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageMode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageMorph.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageOps.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImagePalette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImagePath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageQt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageSequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageShow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageStat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageTk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageTransform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageWin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImtImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/IptcImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/Jpeg2KImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/JpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/JpegPresets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 18:18:43.000000 types-Pillow-9.5.0.2/PIL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/McIdasImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/MicImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/MpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/MpoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/MspImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PSDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PalmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PcdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PcfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PdfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PdfParser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PixarImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PngImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PsdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PyAccess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/SgiImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/SpiderImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/SunImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/TarIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/TgaImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/TiffImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/TiffTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/WalImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/WebPImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/WmfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/XVThumbImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/XbmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/XpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_imaging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_tkinter_finder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/features.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-26 18:18:43.000000 types-Pillow-9.5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/types_Pillow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-26 18:18:46.000000 types-Pillow-9.5.0.2/types_Pillow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-26 18:18:46.000000 types-Pillow-9.5.0.2/types_Pillow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:18:46.000000 types-Pillow-9.5.0.2/types_Pillow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 18:18:46.000000 types-Pillow-9.5.0.2/types_Pillow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:56.146628 types-Pillow-9.5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-10 09:14:55.000000 types-Pillow-9.5.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 09:14:55.000000 types-Pillow-9.5.0.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:56.146628 types-Pillow-9.5.0.3/PIL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/BdfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/BlpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/BmpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/BufrStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ContainerIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/CurImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/DcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/DdsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/EpsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ExifTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/FitsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/FitsStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/FliImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/FontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/FpxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/FtexImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/GbrImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/GdImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/GifImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/GimpGradientFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/GimpPaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/GribStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/Hdf5StubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/IcnsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/IcoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/Image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageChops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageCms.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageColor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageDraw2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageEnhance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageFilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageFont.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageGrab.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageMath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageMode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageMorph.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageOps.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImagePalette.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImagePath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageQt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageSequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageShow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageStat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageTk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageTransform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImageWin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/ImtImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/IptcImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/Jpeg2KImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/JpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/JpegPresets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 09:14:55.000000 types-Pillow-9.5.0.3/PIL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/McIdasImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/MicImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/MpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/MpoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/MspImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PSDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PalmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PcdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PcfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PdfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PdfParser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PixarImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PngImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PsdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/PyAccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/QoiImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/SgiImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/SpiderImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/SunImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/TarIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/TgaImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/TiffImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/TiffTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/WalImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/WebPImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/WmfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/XVThumbImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/XbmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/XpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/_binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/_imaging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/_tkinter_finder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-10 09:14:33.000000 types-Pillow-9.5.0.3/PIL-stubs/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 09:14:56.146628 types-Pillow-9.5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:14:56.146628 types-Pillow-9.5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-10 09:14:55.000000 types-Pillow-9.5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:14:56.146628 types-Pillow-9.5.0.3/types_Pillow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 09:14:56.000000 types-Pillow-9.5.0.3/types_Pillow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-05-10 09:14:56.000000 types-Pillow-9.5.0.3/types_Pillow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:14:56.000000 types-Pillow-9.5.0.3/types_Pillow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 09:14:56.000000 types-Pillow-9.5.0.3/types_Pillow.egg-info/top_level.txt
```

### Comparing `types-Pillow-9.5.0.2/CHANGELOG.md` & `types-Pillow-9.5.0.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 9.5.0.3 (2023-05-10)
+
+[Pillow] Add all missing items (#10114)
+
 ## 9.5.0.2 (2023-04-26)
 
 Add a return type for `PIL.Image.load` (#9466)
 
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
 
 ## 9.5.0.1 (2023-04-17)
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/BlpImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/BlpImagePlugin.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import IntEnum
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
-from .ImageFile import ImageFile, PyDecoder
+from .ImageFile import ImageFile, PyDecoder, PyEncoder
 
 class Format(IntEnum):
     JPEG: int
 
 BLP_FORMAT_JPEG: Literal[Format.JPEG]
 
 class Encoding(IntEnum):
@@ -40,7 +40,10 @@
 
 class _BLPBaseDecoder(PyDecoder):
     magic: Any
     def decode(self, buffer): ...
 
 class BLP1Decoder(_BLPBaseDecoder): ...
 class BLP2Decoder(_BLPBaseDecoder): ...
+
+class BLPEncoder(PyEncoder):
+    def encode(self, bufsize): ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/EpsImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/EpsImagePlugin.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+import sys
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
 from ._imaging import _PixelAccessor
 from .ImageFile import ImageFile
 
 split: Any
 field: Any
-gs_windows_binary: Any
+if sys.platform == "win32":
+    gs_windows_binary: Literal["gswin32c", "gswin64c", "gs", False]
+else:
+    gs_windows_binary: None
 
 def has_ghostscript(): ...
 def Ghostscript(tile, size, fp, scale: int = 1, transparency: bool = False): ...
 
 class PSFile:
     fp: Any
     char: Any
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ExifTags.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ExifTags.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/FpxImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/FpxImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/GifImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/GifImagePlugin.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from _typeshed import Incomplete
+from enum import IntEnum
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
 from .ImageFile import ImageFile
 
+class LoadingStrategy(IntEnum):
+    RGB_AFTER_FIRST = 0
+    RGB_AFTER_DIFFERENT_PALETTE_ONLY = 1
+    RGB_ALWAYS = 2
+
+LOADING_STRATEGY: LoadingStrategy
+
 class GifImageFile(ImageFile):
     format: ClassVar[Literal["GIF"]]
     format_description: ClassVar[str]
     global_palette: Any
     def data(self): ...
     @property
     def n_frames(self): ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/IcnsImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/IcnsImagePlugin.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from _typeshed import Incomplete
 from typing import Any, ClassVar
-from typing_extensions import Literal
+from typing_extensions import Final, Literal
 
 from ._imaging import _PixelAccessor
 from .ImageFile import ImageFile
 
 enable_jpeg2k: Any
-HEADERSIZE: int
+MAGIC: Final = b"icns"
+HEADERSIZE: Final = 8
 
 def nextheader(fobj): ...
 def read_32t(fobj, start_length, size): ...
 def read_32(fobj, start_length, size): ...
 def read_mk(fobj, start_length, size): ...
 def read_png_or_jpeg2000(fobj, start_length, size): ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/IcoImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/IcoImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/Image.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/Image.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,22 @@
 SEQUENCE: Literal[1]  # deprecated
 CONTAINER: Literal[2]  # deprecated
 
 class DecompressionBombWarning(RuntimeWarning): ...
 class DecompressionBombError(Exception): ...
 
 MAX_IMAGE_PIXELS: int | None
+USE_CFFI_ACCESS: Incomplete
 
 LINEAR: Literal[Resampling.BILINEAR]  # deprecated
 CUBIC: Literal[Resampling.BICUBIC]  # deprecated
 ANTIALIAS: Literal[Resampling.LANCZOS]  # deprecated
 
+def isImageType(t): ...
+
 class Transpose(IntEnum):
     FLIP_LEFT_RIGHT: Literal[0]
     FLIP_TOP_BOTTOM: Literal[1]
     ROTATE_90: Literal[2]
     ROTATE_180: Literal[3]
     ROTATE_270: Literal[4]
     TRANSPOSE: Literal[5]
@@ -143,17 +146,25 @@
 def getmodebandnames(mode: _Mode) -> tuple[str, ...]: ...
 def getmodebands(mode: _Mode) -> int: ...
 def preinit() -> None: ...
 def init() -> None: ...
 def coerce_e(value) -> _E: ...
 
 class _E:
+    scale: Incomplete
+    data: Incomplete
     def __init__(self, scale, data) -> None: ...
+    def __neg__(self): ...
     def __add__(self, other) -> _E: ...
+    __radd__ = __add__
+    def __sub__(self, other): ...
+    def __rsub__(self, other): ...
     def __mul__(self, other) -> _E: ...
+    __rmul__ = __mul__
+    def __truediv__(self, other): ...
 
 _ImageState: TypeAlias = tuple[dict[str, Any], str, tuple[int, int], Any, bytes]
 
 class Image:
     format: ClassVar[str | None]
     format_description: ClassVar[str | None]
     im: Any
@@ -172,14 +183,16 @@
     def height(self) -> int: ...
     @property
     def size(self) -> tuple[int, int]: ...
     def __enter__(self) -> Self: ...
     def __exit__(self, *args: Unused) -> None: ...
     def close(self) -> None: ...
     def __eq__(self, other: object) -> bool: ...
+    @property
+    def __array_interface__(self): ...
     def __getstate__(self) -> _ImageState: ...
     def __setstate__(self, state: _ImageState) -> None: ...
     def tobytes(self, encoder_name: str = "raw", *args) -> bytes: ...
     def tobitmap(self, name: str = "image") -> bytes: ...
     def frombytes(self, data: bytes, decoder_name: str = "raw", *args) -> None: ...
     def load(self) -> _PixelAccessor: ...
     def verify(self) -> None: ...
@@ -209,14 +222,15 @@
     def getcolors(self, maxcolors: int = 256) -> list[tuple[int, int]]: ...
     def getdata(self, band: int | None = None): ...
     def getextrema(self): ...
     def getexif(self) -> Exif: ...
     def get_child_images(self) -> list[Image]: ...
     def getim(self): ...
     def getpalette(self, rawmode: str | None = "RGB") -> list[int] | None: ...
+    def apply_transparency(self) -> None: ...
     def getpixel(self, xy: tuple[int, int]): ...
     def getprojection(self) -> tuple[list[int], list[int]]: ...
     def histogram(self, mask: Image | None = None, extrema: tuple[int, int] | tuple[float, float] | None = None) -> list[int]: ...
     def entropy(self, mask: Image | None = None, extrema: tuple[int, int] | tuple[float, float] | None = None) -> float: ...
     def paste(self, im: Image | _Color, box: tuple[int, int] | _Box | None = None, mask: Image | None = None) -> None: ...
     def alpha_composite(self, im: Image, dest: tuple[int, int] = (0, 0), source: tuple[int, int] = (0, 0)) -> None: ...
     def point(self, lut, mode: _Mode | None = None) -> Image: ...
@@ -300,15 +314,18 @@
 def register_encoder(name: str, encoder) -> None: ...
 def effect_mandelbrot(size: tuple[int, int], extent: tuple[float, float, float, float], quality: int) -> Image: ...
 def effect_noise(size: tuple[int, int], sigma: float) -> Image: ...
 def linear_gradient(mode: _Mode) -> Image: ...
 def radial_gradient(mode: _Mode) -> Image: ...
 
 class Exif(MutableMapping[int, Any]):
+    endian: Incomplete
+    bigtiff: bool
     def load(self, data: bytes) -> None: ...
+    def load_from_fp(self, fp, offset: Incomplete | None = None) -> None: ...
     def tobytes(self, offset: int = 8) -> bytes: ...
     def get_ifd(self, tag: int): ...
     def hide_offsets(self) -> None: ...
     def __len__(self) -> int: ...
     def __getitem__(self, tag: int) -> Any: ...
     def __contains__(self, tag: object) -> bool: ...
     def __setitem__(self, tag: int, value: Any) -> None: ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageChops.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageChops.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageCms.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageCms.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from _typeshed import Incomplete
+import sys
+from _typeshed import Incomplete, Unused
 from enum import IntEnum
 from typing import Any
 from typing_extensions import Literal
 
 from .Image import ImagePointHandler
 
 DESCRIPTION: str
@@ -51,15 +52,19 @@
         proof_intent=...,
         flags: int = 0,
     ) -> None: ...
     def point(self, im): ...
     def apply(self, im, imOut: Incomplete | None = None): ...
     def apply_in_place(self, im): ...
 
-def get_display_profile(handle: Incomplete | None = None): ...
+if sys.platform == "win32":
+    def get_display_profile(handle: Incomplete | None = None) -> ImageCmsProfile | None: ...
+
+else:
+    def get_display_profile(handle: Unused = None) -> None: ...
 
 class PyCMSError(Exception): ...
 
 def profileToProfile(
     im,
     inputProfile,
     outputProfile,
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageDraw.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageDraw.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 from .ImageColor import _Ink
 from .ImageFont import _Font
 
 _XY: TypeAlias = Sequence[float | tuple[float, float]]
 _Outline: TypeAlias = Any
 
 class ImageDraw:
+    font: Incomplete
+    palette: Incomplete
+    im: Incomplete
+    draw: Incomplete
+    mode: Incomplete
+    ink: Incomplete
+    fontmode: str
+    fill: bool
     def __init__(self, im: Image, mode: str | None = None) -> None: ...
     def getfont(self): ...
     def arc(self, xy: _XY, start: float, end: float, fill: _Ink | None = None, width: float = 1) -> None: ...
     def bitmap(self, xy: _XY, bitmap: Image, fill: _Ink | None = None) -> None: ...
     def chord(
         self, xy: _XY, start: float, end: float, fill: _Ink | None = None, outline: _Ink | None = None, width: float = 1
     ) -> None: ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageDraw2.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageDraw2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -28,7 +28,9 @@
     def ellipse(self, xy, *options) -> None: ...
     def line(self, xy, *options) -> None: ...
     def pieslice(self, xy, start, end, *options) -> None: ...
     def polygon(self, xy, *options) -> None: ...
     def rectangle(self, xy, *options) -> None: ...
     def text(self, xy, text, font) -> None: ...
     def textsize(self, text, font): ...
+    def textbbox(self, xy, text, font): ...
+    def textlength(self, text, font): ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageEnhance.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageEnhance.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageFile.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageFile.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,26 @@
 class PyCodecState:
     xsize: int
     ysize: int
     xoff: int
     yoff: int
     def extents(self) -> tuple[int, int, int, int]: ...
 
+class PyCodec:
+    im: Incomplete
+    state: Incomplete
+    fd: Incomplete
+    mode: Incomplete
+    def __init__(self, mode, *args) -> None: ...
+    args: Incomplete
+    def init(self, args) -> None: ...
+    def cleanup(self) -> None: ...
+    def setfd(self, fd) -> None: ...
+    def setimage(self, im, extents: Incomplete | None = None) -> None: ...
+
 class PyDecoder:
     im: Any
     state: Any
     fd: Any
     mode: Any
     def __init__(self, mode, *args) -> None: ...
     args: Any
@@ -64,7 +76,14 @@
     @property
     def pulls_fd(self): ...
     def decode(self, buffer) -> None: ...
     def cleanup(self) -> None: ...
     def setfd(self, fd) -> None: ...
     def setimage(self, im, extents: Incomplete | None = None) -> None: ...
     def set_as_raw(self, data, rawmode: Incomplete | None = None) -> None: ...
+
+class PyEncoder(PyCodec):
+    @property
+    def pushes_fd(self): ...
+    def encode(self, bufsize) -> None: ...
+    def encode_to_pyfd(self): ...
+    def encode_to_file(self, fh, bufsize): ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageFilter.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageFilter.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageFont.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageFont.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,25 @@
 
 class _Font(Protocol):
     def getmask(self, text: str | bytes, mode: str = ..., direction=..., features=...): ...
 
 class ImageFont:
     def getsize(self, text: str | bytes, *args, **kwargs) -> tuple[int, int]: ...
     def getmask(self, text: str | bytes, mode: str = "", direction=..., features=...): ...
+    def getbbox(self, text, *args, **kwargs): ...
+    def getlength(self, text, *args, **kwargs): ...
 
 class FreeTypeFont:
     path: str | bytes | SupportsRead[bytes] | None
     size: int
     index: int
     encoding: str
     layout_engine: Layout
+    font_bytes: Incomplete
+    font: Incomplete
     def __init__(
         self,
         font: str | bytes | SupportsRead[bytes] | None = None,
         size: int = 10,
         index: int = 0,
         encoding: str = "",
         layout_engine: Layout | None = None,
@@ -106,17 +110,21 @@
     ) -> FreeTypeFont: ...
     def get_variation_names(self): ...
     def set_variation_by_name(self, name): ...
     def get_variation_axes(self): ...
     def set_variation_by_axes(self, axes): ...
 
 class TransposedFont:
+    font: Incomplete
+    orientation: Incomplete
     def __init__(self, font: _Font, orientation: int | None = None) -> None: ...
     def getsize(self, text: str | bytes, *args, **kwargs) -> tuple[int, int]: ...
     def getmask(self, text: str | bytes, mode: str = "", *args, **kwargs): ...
+    def getbbox(self, text, *args, **kwargs): ...
+    def getlength(self, text, *args, **kwargs): ...
 
 def load(filename: FileDescriptorOrPath) -> ImageFont: ...
 def truetype(
     font: str | bytes | SupportsRead[bytes] | None = None,
     size: int = 10,
     index: int = 0,
     encoding: str = "",
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageMath.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageMath.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageMorph.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageMorph.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageOps.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageOps.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImagePalette.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImagePalette.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageQt.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageQt.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageShow.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageShow.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageTk.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageTk.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/ImageWin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/ImageWin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/JpegImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/JpegImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/MicImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/MicImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/PSDraw.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/PSDraw.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/PdfParser.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/PdfParser.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/PngImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/PngImagePlugin.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from enum import IntEnum
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
 from ._binary import o8 as o8
 from .ImageFile import ImageFile
 
-logger: Any
 is_cid: Any
 MAX_TEXT_CHUNK: Any
 MAX_TEXT_MEMORY: Any
 
 class Disposal(IntEnum):
     OP_NONE: int
     OP_BACKGROUND: int
@@ -100,14 +99,15 @@
     decoderconfig: Any
     def load_prepare(self) -> None: ...
     def load_read(self, read_bytes): ...
     png: Any
     im: Any
     def load_end(self) -> None: ...
     def getexif(self): ...
+    def getxmp(self): ...
 
 def putchunk(fp, cid, *data) -> None: ...
 
 class _idat:
     fp: Any
     chunk: Any
     def __init__(self, fp, chunk) -> None: ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/PyAccess.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/PyAccess.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from logging import Logger
 from typing import Any
 
 from PIL._imaging import _PixelAccessor
 
 ffi: Any
-logger: Logger
 
 class PyAccess(_PixelAccessor):
     readonly: Any
     image8: Any
     image32: Any
     image: Any
     def __init__(self, img, readonly: bool = False) -> None: ...
```

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/SpiderImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/SpiderImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/WmfImagePlugin.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/WmfImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/_imaging.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/_imaging.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PIL-stubs/features.pyi` & `types-Pillow-9.5.0.3/PIL-stubs/features.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.2/PKG-INFO` & `types-Pillow-9.5.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.5.0.2
+Version: 9.5.0.3
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f7443a748e87e1bf4ab675b3d0a56f0ba44a21ce`.
+This package was generated from typeshed commit `1221b4711818d3c5e17c56619fc049e5dbc2fd00`.
```

### Comparing `types-Pillow-9.5.0.2/setup.py` & `types-Pillow-9.5.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f7443a748e87e1bf4ab675b3d0a56f0ba44a21ce`.
+This package was generated from typeshed commit `1221b4711818d3c5e17c56619fc049e5dbc2fd00`.
 '''.lstrip()
 
 setup(name=name,
-      version="9.5.0.2",
+      version="9.5.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['PIL-stubs'],
-      package_data={'PIL-stubs': ['BdfFontFile.pyi', 'BlpImagePlugin.pyi', 'BmpImagePlugin.pyi', 'BufrStubImagePlugin.pyi', 'ContainerIO.pyi', 'CurImagePlugin.pyi', 'DcxImagePlugin.pyi', 'DdsImagePlugin.pyi', 'EpsImagePlugin.pyi', 'ExifTags.pyi', 'FitsStubImagePlugin.pyi', 'FliImagePlugin.pyi', 'FontFile.pyi', 'FpxImagePlugin.pyi', 'FtexImagePlugin.pyi', 'GbrImagePlugin.pyi', 'GdImageFile.pyi', 'GifImagePlugin.pyi', 'GimpGradientFile.pyi', 'GimpPaletteFile.pyi', 'GribStubImagePlugin.pyi', 'Hdf5StubImagePlugin.pyi', 'IcnsImagePlugin.pyi', 'IcoImagePlugin.pyi', 'ImImagePlugin.pyi', 'Image.pyi', 'ImageChops.pyi', 'ImageCms.pyi', 'ImageColor.pyi', 'ImageDraw.pyi', 'ImageDraw2.pyi', 'ImageEnhance.pyi', 'ImageFile.pyi', 'ImageFilter.pyi', 'ImageFont.pyi', 'ImageGrab.pyi', 'ImageMath.pyi', 'ImageMode.pyi', 'ImageMorph.pyi', 'ImageOps.pyi', 'ImagePalette.pyi', 'ImagePath.pyi', 'ImageQt.pyi', 'ImageSequence.pyi', 'ImageShow.pyi', 'ImageStat.pyi', 'ImageTk.pyi', 'ImageTransform.pyi', 'ImageWin.pyi', 'ImtImagePlugin.pyi', 'IptcImagePlugin.pyi', 'Jpeg2KImagePlugin.pyi', 'JpegImagePlugin.pyi', 'JpegPresets.pyi', 'McIdasImagePlugin.pyi', 'MicImagePlugin.pyi', 'MpegImagePlugin.pyi', 'MpoImagePlugin.pyi', 'MspImagePlugin.pyi', 'PSDraw.pyi', 'PaletteFile.pyi', 'PalmImagePlugin.pyi', 'PcdImagePlugin.pyi', 'PcfFontFile.pyi', 'PcxImagePlugin.pyi', 'PdfImagePlugin.pyi', 'PdfParser.pyi', 'PixarImagePlugin.pyi', 'PngImagePlugin.pyi', 'PpmImagePlugin.pyi', 'PsdImagePlugin.pyi', 'PyAccess.pyi', 'SgiImagePlugin.pyi', 'SpiderImagePlugin.pyi', 'SunImagePlugin.pyi', 'TarIO.pyi', 'TgaImagePlugin.pyi', 'TiffImagePlugin.pyi', 'TiffTags.pyi', 'WalImageFile.pyi', 'WebPImagePlugin.pyi', 'WmfImagePlugin.pyi', 'XVThumbImagePlugin.pyi', 'XbmImagePlugin.pyi', 'XpmImagePlugin.pyi', '__init__.pyi', '_binary.pyi', '_imaging.pyi', '_tkinter_finder.pyi', '_util.pyi', '_version.pyi', 'features.pyi', 'METADATA.toml']},
+      package_data={'PIL-stubs': ['BdfFontFile.pyi', 'BlpImagePlugin.pyi', 'BmpImagePlugin.pyi', 'BufrStubImagePlugin.pyi', 'ContainerIO.pyi', 'CurImagePlugin.pyi', 'DcxImagePlugin.pyi', 'DdsImagePlugin.pyi', 'EpsImagePlugin.pyi', 'ExifTags.pyi', 'FitsImagePlugin.pyi', 'FitsStubImagePlugin.pyi', 'FliImagePlugin.pyi', 'FontFile.pyi', 'FpxImagePlugin.pyi', 'FtexImagePlugin.pyi', 'GbrImagePlugin.pyi', 'GdImageFile.pyi', 'GifImagePlugin.pyi', 'GimpGradientFile.pyi', 'GimpPaletteFile.pyi', 'GribStubImagePlugin.pyi', 'Hdf5StubImagePlugin.pyi', 'IcnsImagePlugin.pyi', 'IcoImagePlugin.pyi', 'ImImagePlugin.pyi', 'Image.pyi', 'ImageChops.pyi', 'ImageCms.pyi', 'ImageColor.pyi', 'ImageDraw.pyi', 'ImageDraw2.pyi', 'ImageEnhance.pyi', 'ImageFile.pyi', 'ImageFilter.pyi', 'ImageFont.pyi', 'ImageGrab.pyi', 'ImageMath.pyi', 'ImageMode.pyi', 'ImageMorph.pyi', 'ImageOps.pyi', 'ImagePalette.pyi', 'ImagePath.pyi', 'ImageQt.pyi', 'ImageSequence.pyi', 'ImageShow.pyi', 'ImageStat.pyi', 'ImageTk.pyi', 'ImageTransform.pyi', 'ImageWin.pyi', 'ImtImagePlugin.pyi', 'IptcImagePlugin.pyi', 'Jpeg2KImagePlugin.pyi', 'JpegImagePlugin.pyi', 'JpegPresets.pyi', 'McIdasImagePlugin.pyi', 'MicImagePlugin.pyi', 'MpegImagePlugin.pyi', 'MpoImagePlugin.pyi', 'MspImagePlugin.pyi', 'PSDraw.pyi', 'PaletteFile.pyi', 'PalmImagePlugin.pyi', 'PcdImagePlugin.pyi', 'PcfFontFile.pyi', 'PcxImagePlugin.pyi', 'PdfImagePlugin.pyi', 'PdfParser.pyi', 'PixarImagePlugin.pyi', 'PngImagePlugin.pyi', 'PpmImagePlugin.pyi', 'PsdImagePlugin.pyi', 'PyAccess.pyi', 'QoiImagePlugin.pyi', 'SgiImagePlugin.pyi', 'SpiderImagePlugin.pyi', 'SunImagePlugin.pyi', 'TarIO.pyi', 'TgaImagePlugin.pyi', 'TiffImagePlugin.pyi', 'TiffTags.pyi', 'WalImageFile.pyi', 'WebPImagePlugin.pyi', 'WmfImagePlugin.pyi', 'XVThumbImagePlugin.pyi', 'XbmImagePlugin.pyi', 'XpmImagePlugin.pyi', '__init__.pyi', '_binary.pyi', '_imaging.pyi', '_tkinter_finder.pyi', '_version.pyi', 'features.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-Pillow-9.5.0.2/types_Pillow.egg-info/PKG-INFO` & `types-Pillow-9.5.0.3/types_Pillow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.5.0.2
+Version: 9.5.0.3
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f7443a748e87e1bf4ab675b3d0a56f0ba44a21ce`.
+This package was generated from typeshed commit `1221b4711818d3c5e17c56619fc049e5dbc2fd00`.
```

### Comparing `types-Pillow-9.5.0.2/types_Pillow.egg-info/SOURCES.txt` & `types-Pillow-9.5.0.3/types_Pillow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 PIL-stubs/BufrStubImagePlugin.pyi
 PIL-stubs/ContainerIO.pyi
 PIL-stubs/CurImagePlugin.pyi
 PIL-stubs/DcxImagePlugin.pyi
 PIL-stubs/DdsImagePlugin.pyi
 PIL-stubs/EpsImagePlugin.pyi
 PIL-stubs/ExifTags.pyi
+PIL-stubs/FitsImagePlugin.pyi
 PIL-stubs/FitsStubImagePlugin.pyi
 PIL-stubs/FliImagePlugin.pyi
 PIL-stubs/FontFile.pyi
 PIL-stubs/FpxImagePlugin.pyi
 PIL-stubs/FtexImagePlugin.pyi
 PIL-stubs/GbrImagePlugin.pyi
 PIL-stubs/GdImageFile.pyi
@@ -70,14 +71,15 @@
 PIL-stubs/PdfImagePlugin.pyi
 PIL-stubs/PdfParser.pyi
 PIL-stubs/PixarImagePlugin.pyi
 PIL-stubs/PngImagePlugin.pyi
 PIL-stubs/PpmImagePlugin.pyi
 PIL-stubs/PsdImagePlugin.pyi
 PIL-stubs/PyAccess.pyi
+PIL-stubs/QoiImagePlugin.pyi
 PIL-stubs/SgiImagePlugin.pyi
 PIL-stubs/SpiderImagePlugin.pyi
 PIL-stubs/SunImagePlugin.pyi
 PIL-stubs/TarIO.pyi
 PIL-stubs/TgaImagePlugin.pyi
 PIL-stubs/TiffImagePlugin.pyi
 PIL-stubs/TiffTags.pyi
@@ -87,14 +89,13 @@
 PIL-stubs/XVThumbImagePlugin.pyi
 PIL-stubs/XbmImagePlugin.pyi
 PIL-stubs/XpmImagePlugin.pyi
 PIL-stubs/__init__.pyi
 PIL-stubs/_binary.pyi
 PIL-stubs/_imaging.pyi
 PIL-stubs/_tkinter_finder.pyi
-PIL-stubs/_util.pyi
 PIL-stubs/_version.pyi
 PIL-stubs/features.pyi
 types_Pillow.egg-info/PKG-INFO
 types_Pillow.egg-info/SOURCES.txt
 types_Pillow.egg-info/dependency_links.txt
 types_Pillow.egg-info/top_level.txt
```

