# Comparing `tmp/opal-common-0.6.1.tar.gz` & `tmp/opal_common-0.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opal-common-0.6.1.tar", last modified: Mon May  1 17:32:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

