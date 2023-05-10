# Comparing `tmp/alchql-3.3.0.22936877.tar.gz` & `tmp/alchql-3.3.0.22936884-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchql-3.3.0.22936877.tar", last modified: Wed May 10 08:58:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

