# Comparing `tmp/vk_urls_validator-0.0.2.tar.gz` & `tmp/vk_urls_validator-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vk_urls_validator-0.0.2.tar", last modified: Sat May  6 12:51:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

