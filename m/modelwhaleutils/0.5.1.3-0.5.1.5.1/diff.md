# Comparing `tmp/modelwhaleutils-0.5.1.3.tar.gz` & `tmp/modelwhaleutils-0.5.1.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/YiranTao/kesci/modelwhaleutils/dist/.tmp-oq2lr9vi/modelwhaleutils-0.5.1.3.tar", last modified: Tue Dec 27 12:06:56 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

