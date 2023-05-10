# Comparing `tmp/kite-1.5.6.tar.gz` & `tmp/kite-1.5.7-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kite-1.5.6.tar", last modified: Thu Apr  6 10:33:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

