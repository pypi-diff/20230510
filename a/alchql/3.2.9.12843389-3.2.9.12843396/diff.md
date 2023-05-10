# Comparing `tmp/alchql-3.2.9.12843389.tar.gz` & `tmp/alchql-3.2.9.12843396-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchql-3.2.9.12843389.tar", last modified: Fri Jan 13 13:13:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

