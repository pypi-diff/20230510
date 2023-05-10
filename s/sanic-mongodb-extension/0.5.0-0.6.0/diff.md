# Comparing `tmp/sanic-mongodb-extension-0.5.0.tar.gz` & `tmp/sanic_mongodb_extension-0.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanic-mongodb-extension-0.5.0.tar", last modified: Mon Dec 12 21:12:32 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

