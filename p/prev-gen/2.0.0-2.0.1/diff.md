# Comparing `tmp/prev_gen-2.0.0-py3-none-any.whl.zip` & `tmp/prev_gen-2.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
 Zip file size: 70969 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      102 b- defN 23-May-10 10:44 prev_gen/__init__.py
 -rw-rw-rw-  2.0 fat     1340 b- defN 23-Feb-11 16:01 prev_gen/example.txt
--rw-rw-rw-  2.0 fat    46673 b- defN 23-May-10 13:17 prev_gen/main.py
+-rw-rw-rw-  2.0 fat    46673 b- defN 23-May-10 13:37 prev_gen/main.py
 -rw-rw-rw-  2.0 fat   125452 b- defN 22-Sep-22 05:27 prev_gen/nunito.ttf
--rw-rw-rw-  2.0 fat     2471 b- defN 23-May-10 13:19 prev_gen-2.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-10 13:19 prev_gen-2.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-10 13:19 prev_gen-2.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      606 b- defN 23-May-10 13:19 prev_gen-2.0.0.dist-info/RECORD
+-rw-rw-rw-  2.0 fat     2471 b- defN 23-May-10 13:43 prev_gen-2.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-10 13:43 prev_gen-2.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-10 13:43 prev_gen-2.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      606 b- defN 23-May-10 13:43 prev_gen-2.0.1.dist-info/RECORD
 8 files, 176745 bytes uncompressed, 69925 bytes compressed:  60.4%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: prev_gen/main.py
 Comment: 
 
 Filename: prev_gen/nunito.ttf
 Comment: 
 
-Filename: prev_gen-2.0.0.dist-info/METADATA
+Filename: prev_gen-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: prev_gen-2.0.0.dist-info/WHEEL
+Filename: prev_gen-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: prev_gen-2.0.0.dist-info/top_level.txt
+Filename: prev_gen-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: prev_gen-2.0.0.dist-info/RECORD
+Filename: prev_gen-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `prev_gen-2.0.0.dist-info/METADATA` & `prev_gen-2.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prev-gen
-Version: 2.0.0
+Version: 2.0.1
 Summary: Create a palette preview image by using a simple config file
 Home-page: https://github.com/Aonodensetsu/prev_gen
 Author: Remigiusz Dończyk
 Author-email: aonodensetsu@aonodensetsu.me
 License: GPL-3.0
 Keywords: palette,preview,generator,image
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 Requires-Dist: pillow
 Requires-Dist: drawsvg (~=2.0)
 
 ## Create a palette preview image by using a simple config file
 
 ![size](https://img.shields.io/github/repo-size/aonodensetsu/prev_gen?label=size) ![files](https://img.shields.io/github/directory-file-count/aonodensetsu/prev_gen) ![lines](https://img.shields.io/tokei/lines/github/aonodensetsu/prev_gen)   
-![py dep](https://img.shields.io/pypi/pyversions/prev-gen) [![version](https://img.shields.io/pypi/v/prev-gen)](https://pypi.org/project/prev-gen/2.0.0/)  
+![py dep](https://img.shields.io/pypi/pyversions/prev-gen) [![version](https://img.shields.io/pypi/v/prev-gen)](https://pypi.org/project/prev-gen/2.0.1/)  
 ![license](https://img.shields.io/pypi/l/prev-gen) [![downloads](https://img.shields.io/badge/releases-here-green?logo=pypi)](https://pypi.org/project/prev-gen/#history)  
 [![downloads](https://img.shields.io/badge/wiki-here-pink)](https://github.com/Aonodensetsu/prev_gen/blob/main/WIKI.md) [![downloads](https://img.shields.io/badge/changelog-here-pink)](https://github.com/Aonodensetsu/prev_gen/blob/main/CHANGELOG.md)  
 
 # Usage:
 1. `pip install prev_gen`
 2. Open up [the wiki](https://github.com/Aonodensetsu/prev_gen/blob/main/WIKI.md) to see how everything works
 3. Create a file based on instructions (or just edit [the example](https://github.com/Aonodensetsu/prev_gen/blob/main/example.py))
@@ -36,8 +36,8 @@
    from prev_gen import Preview
    Preview(palette)
    ```
 
 # Example:
 Inspired by the great [Gruvbox](https://github.com/morhetz/gruvbox) theme, where even the preview is impressive  
 And so, below is the Gruvbox palette preview recreated with this app  
-[![example](https://raw.githubusercontent.com/Aonodensetsu/prev_gen/main/gruvbox.png)](https://github.com/Aonodensetsu/prev_gen/blob/main/gruvbox.png)
+[![example](https://raw.githubusercontent.com/Aonodensetsu/prev_gen/main/gruvbox.svg)](https://github.com/Aonodensetsu/prev_gen/blob/main/gruvbox.svg)
```

