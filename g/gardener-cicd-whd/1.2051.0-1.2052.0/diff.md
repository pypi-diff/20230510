# Comparing `tmp/gardener-cicd-whd-1.2051.0.tar.gz` & `tmp/gardener_cicd_whd-1.2052.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-whd-1.2051.0.tar", last modified: Mon May  8 12:32:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

