# Comparing `tmp/hhnk-threedi-tools-0.9.2.tar.gz` & `tmp/hhnk_threedi_tools-2023.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhnk-threedi-tools-0.9.2.tar", last modified: Wed Aug 17 15:12:02 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

