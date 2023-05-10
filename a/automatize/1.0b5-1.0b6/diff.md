# Comparing `tmp/automatize-1.0b5.tar.gz` & `tmp/automatize-1.0b6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatize-1.0b5.tar", last modified: Mon May  1 02:57:39 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

