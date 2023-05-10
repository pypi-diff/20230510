# Comparing `tmp/weighted_kdtree-0.1.0.tar.gz` & `tmp/weighted_kdtree-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_kdtree-0.1.0.tar", last modified: Wed May 10 17:45:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

