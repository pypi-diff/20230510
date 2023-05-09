# Comparing `tmp/reportbro-fpdf2-0.9.1.tar.gz` & `tmp/reportbro_fpdf2-2.7.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportbro-fpdf2-0.9.1.tar", last modified: Tue Aug  9 22:36:11 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

