# Comparing `tmp/PyLEMS-0.6.0.tar.gz` & `tmp/PyLEMS-0.6.1-py3.10.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyLEMS-0.6.0.tar", last modified: Mon Oct 17 14:23:11 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

