# Comparing `tmp/pythonbible_parser-0.0.5.tar.gz` & `tmp/pythonbible_parser-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonbible_parser-0.0.5.tar", last modified: Thu Apr 27 22:34:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

