# Comparing `tmp/multimd-0.1.0b0.tar.gz` & `tmp/multimd-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimd-0.1.0b0.tar", max compression
+gzip compressed data, was "multimd-0.2.0b0.tar", max compression
```

## Comparing `multimd-0.1.0b0.tar` & `multimd-0.2.0b0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     2027 2022-12-26 22:59:49.636042 multimd-0.1.0b0/README.md
--rw-r--r--   0        0        0    35121 2022-08-11 10:12:56.182565 multimd-0.1.0b0/multimd/LICENSE.txt
--rw-r--r--   0        0        0     2041 2022-08-11 10:12:56.183017 multimd-0.1.0b0/multimd/README.md
--rwxr-xr-x   0        0        0       88 2022-12-26 22:56:05.896741 multimd-0.1.0b0/multimd/__init__.py
--rwxr-xr-x   0        0        0     2340 2022-12-26 22:56:05.911681 multimd-0.1.0b0/multimd/build.py
--rwxr-xr-x   0        0        0     2440 2022-12-26 22:56:05.936512 multimd-0.1.0b0/multimd/toc.py
--rw-r--r--   0        0        0      612 2022-12-26 23:22:11.590264 multimd-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 multimd-0.1.0b0/setup.py
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 multimd-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     2780 2023-05-10 20:57:34.352203 multimd-0.2.0b0/README.md
+-rw-r--r--   0        0        0    35121 2023-05-10 20:57:34.348455 multimd-0.2.0b0/multimd/LICENSE.txt
+-rw-r--r--   0        0        0     2780 2023-05-10 20:57:34.352793 multimd-0.2.0b0/multimd/README.md
+-rw-r--r--   0        0        0       94 2023-05-10 20:57:34.346350 multimd-0.2.0b0/multimd/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-10 20:57:34.348975 multimd-0.2.0b0/multimd/__main__.py
+-rw-r--r--   0        0        0     1868 2023-05-10 20:57:34.345987 multimd-0.2.0b0/multimd/mmdbuild.py
+-rw-r--r--   0        0        0     2029 2023-05-10 20:57:34.346742 multimd-0.2.0b0/multimd/mmdcli.py
+-rw-r--r--   0        0        0     5043 2023-05-10 20:57:34.344303 multimd-0.2.0b0/multimd/mmdtoc.py
+-rw-r--r--   0        0        0      707 2023-05-10 20:56:54.204845 multimd-0.2.0b0/pyproject.toml
+-rw-r--r--   0        0        0     3790 1970-01-01 00:00:00.000000 multimd-0.2.0b0/setup.py
+-rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 multimd-0.2.0b0/PKG-INFO
```

### Comparing `multimd-0.1.0b0/README.md` & `multimd-0.2.0b0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,94 @@
 The `Python` module `multimd`
 =============================
 
-
 > **I beg your pardon for my english...**
 >
 > English is not my native language, so be nice if you notice misunderstandings, misspellings, or grammatical errors in my documents and codes.
 
 
+This document is a short tutorial showing the most useful features without being exhaustive.
+
+
 About `multimd`
 ---------------
 
-Working with `MD` documents of moderate size in a single file can becomes quickly painful. This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single  `MD` file.
+Working with moderate sized `MD` documents in a single file can quickly become tedious. This project allows you to go through separate small `MD` files to be merged into a final single `MD` file.
+
+
+> *At the moment, resources, such as images, are not managed.*
 
 
 `README.md` part by part
 ------------------------
 
-Thanks to `multimd`, you can write a `MD` document typing small section like parts that are easy to maintain. Let's consider the `README.md` of the `src2prod` project that was written using the following tree structure on August 22, 2021. Just note that there are only `MD` files directly inside the same folder (the purpose of `multimd` is to ease the writting of realtively small documents and not books).
+With `multimd`, you can write a `MD` document by typing small section-like parts which are easy to maintain. Consider the `README.md` file from the `src2prod` project which was written using the following tree on 6 May 2023.
 
 ~~~
 + src2prod
+    * README.md
     + readme
         * about.yaml
+        * about.md
         * build.md
         * cli.md
         * example-used.md
         * only-files.md
         * prologue.md
         * readme-splitted.md
-
-    * README.md
+    + ...
 ~~~
 
-The special file `about.yaml` allows to indicate the order to use to merge the different `MD` files. Its content was the following one.
+
+The special `about.yaml` file is used to specify a specific order in which the different `MD` files are put together (without this file, a "natural" order is used). Its content is as follows: we give the list of the files without their extension.
 
 ~~~yaml
 toc:
   - prologue
+  - about
   - example-used
   - build
   - only-files
   - readme-splitted
   - cli
 ~~~
 
-Here how `README.md` was built. We will suppose the use of the `cd` command to go inside the parent folder of `scr2prod` before launching the following script where we use instances of `Path` from `pathlib`.
+
+> ***WARNING!*** *You can use relative paths but you must use the Unix path separator `/`.*
+
+
+Building the final `README.md` file is done quickly on the command line using `multimd` after using the `cd` command to go into the `src2prod` folder. We use the option `-e` to allow to erase an existing `README.md` file.
+
+~~~bash
+> multimd -e readme README.md
+Successfully built file.
+  + Path given:
+    README.md
+  + Full path used:
+    /full/path/to/README.md
+~~~
+
+
+There is also an easy-to-use `Python` API.
 
 ~~~python
-from multimd import Builder
+from multimd import MMDBuilder, Path
 
-mybuilder = Builder(
-    output  = Path('README.md'),
-    content = Path('readme'),
+mybuilder = MMDBuilder(
+    src   = Path("/full/path/to/readme"),
+    dest  = Path("/full/path/to/README.md"),
+    erase = True
 )
-
 mybuilder.build()
 ~~~
 
 
+> ***NOTE.*** *It is possible to work with subfolders containing `MD` files. In this case, `multimd` will work recursively. In the `about.yaml` file, the path to a subfolder simply ends with the Unix path separator `/` like in `one/sub/folder/`.*
+
+
 Without the special `about.yaml` file
 -------------------------------------
 
-If you don't use the `about.yaml` file, the class `Builder` looks for all the `MD` files and then merges. The ordred used is the one given by `natsorted` from the package `natsort`.
+Without an `about.yaml` file, all the `MD` files will be merged into one after sorting them in a "natural" order.
+
+
+> ***WARNING!*** *Without an `about.yaml` file, it is impossible to work with subfolders containing `MD` files.*
```

### Comparing `multimd-0.1.0b0/multimd/LICENSE.txt` & `multimd-0.2.0b0/multimd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multimd-0.1.0b0/multimd/README.md` & `multimd-0.2.0b0/multimd/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,94 @@
 The `Python` module `multimd`
 =============================
 
-
 > **I beg your pardon for my english...**
 >
 > English is not my native language, so be nice if you notice misunderstandings, misspellings, or grammatical errors in my documents and codes.
 
 
+This document is a short tutorial showing the most useful features without being exhaustive.
+
+
 About `multimd`
 ---------------
 
-Working with `MD` documents of moderate size in a single file can becomes quickly painful. This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single  `MD` file.
+Working with moderate sized `MD` documents in a single file can quickly become tedious. This project allows you to go through separate small `MD` files to be merged into a final single `MD` file.
+
+
+> *At the moment, resources, such as images, are not managed.*
 
 
 `README.md` part by part
 ------------------------
 
-Thanks to `multimd`, you can write a `MD` document typing small section like parts that are easy to maintain. Let's consider the `README.md` of the `src2prod` project that was written using the following tree structure on August 22, 2021. Just note that there are only `MD` files directly inside the same folder (the purpose of `multimd` is to ease the writting of realtively small documents and not books). 
+With `multimd`, you can write a `MD` document by typing small section-like parts which are easy to maintain. Consider the `README.md` file from the `src2prod` project which was written using the following tree on 6 May 2023.
 
 ~~~
 + src2prod
+    * README.md
     + readme
-        * about.peuf
+        * about.yaml
+        * about.md
         * build.md
         * cli.md
         * example-used.md
         * only-files.md
         * prologue.md
         * readme-splitted.md
-    
-    * README.md
+    + ...
 ~~~
 
-The special file `about.peuf` allows to indicate the order to use to merge the different `MD` files. Its content was the following one.
 
+The special `about.yaml` file is used to specify a specific order in which the different `MD` files are put together (without this file, a "natural" order is used). Its content is as follows: we give the list of the files without their extension.
+
+~~~yaml
+toc:
+  - prologue
+  - about
+  - example-used
+  - build
+  - only-files
+  - readme-splitted
+  - cli
 ~~~
-toc::
-    + prologue
-    + example-used
-    + build
-    + only-files
-    + readme-splitted
-    + cli
+
+
+> ***WARNING!*** *You can use relative paths but you must use the Unix path separator `/`.*
+
+
+Building the final `README.md` file is done quickly on the command line using `multimd` after using the `cd` command to go into the `src2prod` folder. We use the option `-e` to allow to erase an existing `README.md` file.
+
+~~~bash
+> multimd -e readme README.md
+Successfully built file.
+  + Path given:
+    README.md
+  + Full path used:
+    /full/path/to/README.md
 ~~~
 
-Here how `README.md` was built. We will suppose the use of the `cd` command to go inside the parent folder of `scr2prod` before launching the following script where we use instances of `Path` from `pathlib`.
+
+There is also an easy-to-use `Python` API.
 
 ~~~python
-from multimd import Builder
+from multimd import MMDBuilder, Path
 
-mybuilder = Builder(
-    output  = Path('README.md'),
-    content = Path('readme'),
+mybuilder = MMDBuilder(
+    src   = Path("/full/path/to/readme"),
+    dest  = Path("/full/path/to/README.md"),
+    erase = True
 )
-
 mybuilder.build()
 ~~~
 
 
-Without the special `about.peuf` file
+> ***NOTE.*** *It is possible to work with subfolders containing `MD` files. In this case, `multimd` will work recursively. In the `about.yaml` file, the path to a subfolder simply ends with the Unix path separator `/` like in `one/sub/folder/`.*
+
+
+Without the special `about.yaml` file
 -------------------------------------
 
-If you don't use the `about.peuf` file, the class `Builder` looks for all the `MD` files and then merges. The ordred used is the one givent by `natsorted` from the package `natsort`.
+Without an `about.yaml` file, all the `MD` files will be merged into one after sorting them in a "natural" order.
+
+
+> ***WARNING!*** *Without an `about.yaml` file, it is impossible to work with subfolders containing `MD` files.*
```

### Comparing `multimd-0.1.0b0/multimd/build.py` & `multimd-0.2.0b0/multimd/mmdbuild.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,103 +2,71 @@
 
 ###
 # This module allows to make a single path::``MD`` file from several single
 # ones (using or not an "automatic" merging).
 ###
 
 
-from typing import *
-
 from pathlib import Path
 
-from natsort import natsorted
-
-from .toc import *
+from .mmdtoc import *
 
 
 # ------------------------------------ #
 # -- SINGLE MD FROM MULTI SINGLE MD -- #
 # ------------------------------------ #
 
 ###
 # This class finds all the single path::``MD`` files and then builds a final
-# single one.
+# single one with all the chunks found.
 ###
-class Builder():
+class MMDBuilder():
 
 ###
 # prototype::
-#     output  : the path of the single final path::``MD`` file.
-#     content : the path of the directory with the path::``MD`` files.
+#     src   : the path of the directory containing the path::``MD`` chunks.
+#     dest  : the path of the single final path::``MD`` file to build.
+#     erase : set to ``True``, this argument allows to erase an existing
+#             final file to build a new one.
 ###
     def __init__(
         self,
-        output : Path,
-        content: Path,
+        src  : Path,
+        dest : Path,
+        erase: bool = False
     ) -> None:
-        self.output  = output
-        self.content = content
-
-        self._lof: List[Path] = []
+        self.src   = src
+        self.dest  = dest
+        self.erase = erase
 
 
 ###
 # prototype::
-#     :action: this method is the great bandleader building the final
-#              path::``MD`` file from several single ones.
+#     :action: this method finds the single path::``MD`` files, and then merges
+#              all the ¨md codes found to build the final path::``MD`` file.
 ###
     def build(self) -> None:
-        for name in [
-            'build_lof',
-            'merge',
-        ]:
-            getattr(self, name)()
-
-
-###
-# prototype::
-#     :action: this method builds the list of the single path::``MD`` files.
-###
-    def build_lof(self) -> None:
-# Do we have an ``about.yaml`` file?
-        if (self.content / ABOUT_FILE_NAME).is_file():
-            self._lof = TOC(self.content).extract()
-
-            return
-
-# Find all the MD files.
-        self._lof = []
-
-        for fileordir in self.content.iterdir():
-            if not fileordir.is_file():
-                continue
-
-            if fileordir.suffix == MD_FILE_SUFFIX:
-                self._lof.append(fileordir)
-
-        self._lof = natsorted(self._lof)
-
-
-###
-# prototype::
-#     :action: this method simply merges all the ¨md codes in
-#              a single path::``MD`` file.
-###
-    def merge(self) -> None:
-# All the MD code.
+# All the MD codes.
         mdcode = []
 
-        for onefile in self._lof:
-            with onefile.open(
-                encoding = 'utf-8',
-                mode     = 'r',
-            ) as f:
-                mdcode.append(f.read().strip())
+        for onefile in MMDTOC(self.src).extract():
+            mdcode.append(
+                onefile.read_text(encoding = 'utf-8')
+                       .strip()
+            )
 
         mdcode = ('\n'*3).join(mdcode)
 
-# We can build the file.
-        with self.output.open(
-            encoding = 'utf-8',
-            mode     = 'w',
-        ) as f:
-            f.write(mdcode)
+# Can we erase an existing final file?
+        if self.dest.is_file() and not self.erase:
+            raise IOError(
+                f"the class {type(self).__name__} is not allowed "
+                 "to erase the final file:"
+                 "\n"
+                f"{self.dest}"
+            )
+
+# We can build the file, so let's do it.
+        self.dest.write_text(
+            data     = mdcode,
+            encoding = 'utf-8'
+        )
```

### Comparing `multimd-0.1.0b0/pyproject.toml` & `multimd-0.2.0b0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 [tool.poetry]
 name         = "multimd"
-version      = "0.1.0-beta"
+version      = "0.2.0-beta"
 description  = 'This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single final `MD` file.'
 readme       = "README.md"
 authors      = ["Christophe BAL"]
 maintainers  = ["Christophe BAL"]
 license      = "GNU License Version 3"
 repository   = "https://github.com/bc-tools/for-dev/tree/main/multimd"
 
+[tool.poetry.scripts]
+multimd = "multimd.__main__:mmd_CLI"
+
 [tool.poetry.dependencies]
 python  = "^3.8"
-natsort = "^7.1.1"
+natsort = "^8.2"
+rich    = "^13.3.5"
+typer   = "^0.9"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires      = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `multimd-0.1.0b0/setup.py` & `multimd-0.2.0b0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 packages = \
 ['multimd']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['natsort>=7.1.1,<8.0.0']
+['natsort>=8.2,<9.0', 'rich>=13.3.5,<14.0.0', 'typer>=0.9,<0.10']
+
+entry_points = \
+{'console_scripts': ['multimd = multimd.__main__:mmd_CLI']}
 
 setup_kwargs = {
     'name': 'multimd',
-    'version': '0.1.0b0',
+    'version': '0.2.0b0',
     'description': 'This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single final `MD` file.',
-    'long_description': "The `Python` module `multimd`\n=============================\n\n\n> **I beg your pardon for my english...**\n>\n> English is not my native language, so be nice if you notice misunderstandings, misspellings, or grammatical errors in my documents and codes.\n\n\nAbout `multimd`\n---------------\n\nWorking with `MD` documents of moderate size in a single file can becomes quickly painful. This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single  `MD` file.\n\n\n`README.md` part by part\n------------------------\n\nThanks to `multimd`, you can write a `MD` document typing small section like parts that are easy to maintain. Let's consider the `README.md` of the `src2prod` project that was written using the following tree structure on August 22, 2021. Just note that there are only `MD` files directly inside the same folder (the purpose of `multimd` is to ease the writting of realtively small documents and not books).\n\n~~~\n+ src2prod\n    + readme\n        * about.yaml\n        * build.md\n        * cli.md\n        * example-used.md\n        * only-files.md\n        * prologue.md\n        * readme-splitted.md\n\n    * README.md\n~~~\n\nThe special file `about.yaml` allows to indicate the order to use to merge the different `MD` files. Its content was the following one.\n\n~~~yaml\ntoc:\n  - prologue\n  - example-used\n  - build\n  - only-files\n  - readme-splitted\n  - cli\n~~~\n\nHere how `README.md` was built. We will suppose the use of the `cd` command to go inside the parent folder of `scr2prod` before launching the following script where we use instances of `Path` from `pathlib`.\n\n~~~python\nfrom multimd import Builder\n\nmybuilder = Builder(\n    output  = Path('README.md'),\n    content = Path('readme'),\n)\n\nmybuilder.build()\n~~~\n\n\nWithout the special `about.yaml` file\n-------------------------------------\n\nIf you don't use the `about.yaml` file, the class `Builder` looks for all the `MD` files and then merges. The ordred used is the one given by `natsorted` from the package `natsort`.\n",
+    'long_description': 'The `Python` module `multimd`\n=============================\n\n> **I beg your pardon for my english...**\n>\n> English is not my native language, so be nice if you notice misunderstandings, misspellings, or grammatical errors in my documents and codes.\n\n\nThis document is a short tutorial showing the most useful features without being exhaustive.\n\n\nAbout `multimd`\n---------------\n\nWorking with moderate sized `MD` documents in a single file can quickly become tedious. This project allows you to go through separate small `MD` files to be merged into a final single `MD` file.\n\n\n> *At the moment, resources, such as images, are not managed.*\n\n\n`README.md` part by part\n------------------------\n\nWith `multimd`, you can write a `MD` document by typing small section-like parts which are easy to maintain. Consider the `README.md` file from the `src2prod` project which was written using the following tree on 6 May 2023.\n\n~~~\n+ src2prod\n    * README.md\n    + readme\n        * about.yaml\n        * about.md\n        * build.md\n        * cli.md\n        * example-used.md\n        * only-files.md\n        * prologue.md\n        * readme-splitted.md\n    + ...\n~~~\n\n\nThe special `about.yaml` file is used to specify a specific order in which the different `MD` files are put together (without this file, a "natural" order is used). Its content is as follows: we give the list of the files without their extension.\n\n~~~yaml\ntoc:\n  - prologue\n  - about\n  - example-used\n  - build\n  - only-files\n  - readme-splitted\n  - cli\n~~~\n\n\n> ***WARNING!*** *You can use relative paths but you must use the Unix path separator `/`.*\n\n\nBuilding the final `README.md` file is done quickly on the command line using `multimd` after using the `cd` command to go into the `src2prod` folder. We use the option `-e` to allow to erase an existing `README.md` file.\n\n~~~bash\n> multimd -e readme README.md\nSuccessfully built file.\n  + Path given:\n    README.md\n  + Full path used:\n    /full/path/to/README.md\n~~~\n\n\nThere is also an easy-to-use `Python` API.\n\n~~~python\nfrom multimd import MMDBuilder, Path\n\nmybuilder = MMDBuilder(\n    src   = Path("/full/path/to/readme"),\n    dest  = Path("/full/path/to/README.md"),\n    erase = True\n)\nmybuilder.build()\n~~~\n\n\n> ***NOTE.*** *It is possible to work with subfolders containing `MD` files. In this case, `multimd` will work recursively. In the `about.yaml` file, the path to a subfolder simply ends with the Unix path separator `/` like in `one/sub/folder/`.*\n\n\nWithout the special `about.yaml` file\n-------------------------------------\n\nWithout an `about.yaml` file, all the `MD` files will be merged into one after sorting them in a "natural" order.\n\n\n> ***WARNING!*** *Without an `about.yaml` file, it is impossible to work with subfolders containing `MD` files.*',
     'author': 'Christophe BAL',
     'author_email': 'None',
     'maintainer': 'Christophe BAL',
     'maintainer_email': 'None',
     'url': 'https://github.com/bc-tools/for-dev/tree/main/multimd',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `multimd-0.1.0b0/PKG-INFO` & `multimd-0.2.0b0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,84 +1,115 @@
 Metadata-Version: 2.1
 Name: multimd
-Version: 0.1.0b0
+Version: 0.2.0b0
 Summary: This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single final `MD` file.
 Home-page: https://github.com/bc-tools/for-dev/tree/main/multimd
 License: GNU License Version 3
 Author: Christophe BAL
 Maintainer: Christophe BAL
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: natsort (>=7.1.1,<8.0.0)
+Requires-Dist: natsort (>=8.2,<9.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: typer (>=0.9,<0.10)
 Project-URL: Repository, https://github.com/bc-tools/for-dev/tree/main/multimd
 Description-Content-Type: text/markdown
 
 The `Python` module `multimd`
 =============================
 
-
 > **I beg your pardon for my english...**
 >
 > English is not my native language, so be nice if you notice misunderstandings, misspellings, or grammatical errors in my documents and codes.
 
 
+This document is a short tutorial showing the most useful features without being exhaustive.
+
+
 About `multimd`
 ---------------
 
-Working with `MD` documents of moderate size in a single file can becomes quickly painful. This project makes it possible to write separated pieces of `MD` files that will be merged to produce one single  `MD` file.
+Working with moderate sized `MD` documents in a single file can quickly become tedious. This project allows you to go through separate small `MD` files to be merged into a final single `MD` file.
+
+
+> *At the moment, resources, such as images, are not managed.*
 
 
 `README.md` part by part
 ------------------------
 
-Thanks to `multimd`, you can write a `MD` document typing small section like parts that are easy to maintain. Let's consider the `README.md` of the `src2prod` project that was written using the following tree structure on August 22, 2021. Just note that there are only `MD` files directly inside the same folder (the purpose of `multimd` is to ease the writting of realtively small documents and not books).
+With `multimd`, you can write a `MD` document by typing small section-like parts which are easy to maintain. Consider the `README.md` file from the `src2prod` project which was written using the following tree on 6 May 2023.
 
 ~~~
 + src2prod
+    * README.md
     + readme
         * about.yaml
+        * about.md
         * build.md
         * cli.md
         * example-used.md
         * only-files.md
         * prologue.md
         * readme-splitted.md
-
-    * README.md
+    + ...
 ~~~
 
-The special file `about.yaml` allows to indicate the order to use to merge the different `MD` files. Its content was the following one.
+
+The special `about.yaml` file is used to specify a specific order in which the different `MD` files are put together (without this file, a "natural" order is used). Its content is as follows: we give the list of the files without their extension.
 
 ~~~yaml
 toc:
   - prologue
+  - about
   - example-used
   - build
   - only-files
   - readme-splitted
   - cli
 ~~~
 
-Here how `README.md` was built. We will suppose the use of the `cd` command to go inside the parent folder of `scr2prod` before launching the following script where we use instances of `Path` from `pathlib`.
+
+> ***WARNING!*** *You can use relative paths but you must use the Unix path separator `/`.*
+
+
+Building the final `README.md` file is done quickly on the command line using `multimd` after using the `cd` command to go into the `src2prod` folder. We use the option `-e` to allow to erase an existing `README.md` file.
+
+~~~bash
+> multimd -e readme README.md
+Successfully built file.
+  + Path given:
+    README.md
+  + Full path used:
+    /full/path/to/README.md
+~~~
+
+
+There is also an easy-to-use `Python` API.
 
 ~~~python
-from multimd import Builder
+from multimd import MMDBuilder, Path
 
-mybuilder = Builder(
-    output  = Path('README.md'),
-    content = Path('readme'),
+mybuilder = MMDBuilder(
+    src   = Path("/full/path/to/readme"),
+    dest  = Path("/full/path/to/README.md"),
+    erase = True
 )
-
 mybuilder.build()
 ~~~
 
 
+> ***NOTE.*** *It is possible to work with subfolders containing `MD` files. In this case, `multimd` will work recursively. In the `about.yaml` file, the path to a subfolder simply ends with the Unix path separator `/` like in `one/sub/folder/`.*
+
+
 Without the special `about.yaml` file
 -------------------------------------
 
-If you don't use the `about.yaml` file, the class `Builder` looks for all the `MD` files and then merges. The ordred used is the one given by `natsorted` from the package `natsort`.
+Without an `about.yaml` file, all the `MD` files will be merged into one after sorting them in a "natural" order.
+
 
+> ***WARNING!*** *Without an `about.yaml` file, it is impossible to work with subfolders containing `MD` files.*
```

