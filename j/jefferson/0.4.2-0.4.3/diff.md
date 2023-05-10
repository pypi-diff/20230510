# Comparing `tmp/jefferson-0.4.2.tar.gz` & `tmp/jefferson-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jefferson-0.4.2.tar", max compression
+gzip compressed data, was "jefferson-0.4.3.tar", max compression
```

## Comparing `jefferson-0.4.2.tar` & `jefferson-0.4.3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1083 2023-02-08 13:56:04.936639 jefferson-0.4.2/LICENSE
--rwxr-xr-x   0        0        0      870 2023-02-08 13:56:04.936639 jefferson-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-02-08 13:56:04.936639 jefferson-0.4.2/jefferson/__init__.py
--rw-r--r--   0        0        0     1792 2023-02-08 13:56:04.936639 jefferson-0.4.2/jefferson/cli.py
--rw-r--r--   0        0        0        0 2023-02-08 13:56:04.936639 jefferson-0.4.2/jefferson/compression/__init__.py
--rw-r--r--   0        0        0      395 2023-02-08 13:56:04.936639 jefferson-0.4.2/jefferson/compression/jffs2_lzma.py
--rw-r--r--   0        0        0      829 2023-02-08 13:56:04.936639 jefferson-0.4.2/jefferson/compression/rtime.py
--rw-r--r--   0        0        0        0 2023-02-08 13:56:04.936639 jefferson-0.4.2/jefferson/core/__init__.py
--rw-r--r--   0        0        0    16751 2023-02-08 13:56:04.936639 jefferson-0.4.2/jefferson/jffs2.py
--rw-r--r--   0        0        0      824 2023-02-08 13:56:04.936639 jefferson-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 jefferson-0.4.2/setup.py
--rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 jefferson-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-10 06:39:36.328341 jefferson-0.4.3/LICENSE
+-rwxr-xr-x   0        0        0      965 2023-05-10 06:39:36.328341 jefferson-0.4.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/__init__.py
+-rw-r--r--   0        0        0     1792 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/cli.py
+-rw-r--r--   0        0        0        0 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/compression/__init__.py
+-rw-r--r--   0        0        0      395 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/compression/jffs2_lzma.py
+-rw-r--r--   0        0        0      829 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/compression/rtime.py
+-rw-r--r--   0        0        0        0 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/core/__init__.py
+-rw-r--r--   0        0        0    16776 2023-05-10 06:39:36.328341 jefferson-0.4.3/jefferson/jffs2.py
+-rw-r--r--   0        0        0      825 2023-05-10 06:39:36.328341 jefferson-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 jefferson-0.4.3/PKG-INFO
```

### Comparing `jefferson-0.4.2/LICENSE` & `jefferson-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.2/jefferson/cli.py` & `jefferson-0.4.3/jefferson/cli.py`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.2/jefferson/compression/rtime.py` & `jefferson-0.4.3/jefferson/compression/rtime.py`

 * *Files identical despite different names*

### Comparing `jefferson-0.4.2/jefferson/jffs2.py` & `jefferson-0.4.3/jefferson/jffs2.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import stat
 import struct
 import sys
 import zlib
 from pathlib import Path
 
 import cstruct
-import lzo
+from lzallright.lzallright import LZOCompressor as lzo
 
 import jefferson.compression.jffs2_lzma as jffs2_lzma
 import jefferson.compression.rtime as rtime
 
 
 def PAD(x):
     return ((x) + 3) & ~3
@@ -176,15 +176,15 @@
             elif self.compr == JFFS2_COMPR_ZLIB:
                 self.data = zlib.decompress(node_data)
             elif self.compr == JFFS2_COMPR_RTIME:
                 self.data = rtime.decompress(node_data, self.dsize)
             elif self.compr == JFFS2_COMPR_LZMA:
                 self.data = jffs2_lzma.decompress(node_data, self.dsize)
             elif self.compr == JFFS2_COMPR_LZO:
-                self.data = lzo.decompress(node_data, False, self.dsize)
+                self.data = lzo.decompress(node_data)
             else:
                 print("compression not implemented", self)
                 print(node_data.hex()[:20])
                 self.data = node_data
         except Exception as e:
             print(
                 "Decompression error on inode {}: {}".format(self.ino, e),
```

### Comparing `jefferson-0.4.2/pyproject.toml` & `jefferson-0.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "jefferson"
-version = "0.4.2"
+version = "0.4.3"
 description = "JFFS2 filesystem extraction tool."
 authors = ["ONEKEY <support@onekey.com>", "Stefan Viehböck <support@onekey.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "jefferson" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 cstruct = "^5.2"
-python-lzo = "^1.14"
 click = "^8.1.3"
+lzallright = "^0.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `jefferson-0.4.2/PKG-INFO` & `jefferson-0.4.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,58 @@
 Metadata-Version: 2.1
 Name: jefferson
-Version: 0.4.2
+Version: 0.4.3
 Summary: JFFS2 filesystem extraction tool.
 License: MIT
 Author: ONEKEY
 Author-email: support@onekey.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cstruct (>=5.2,<6.0)
-Requires-Dist: python-lzo (>=1.14,<2.0)
+Requires-Dist: lzallright (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 ## Jefferson
 
-JFFS2 filesystem extraction tool
+JFFS2 filesystem extraction tool.
 
 ### Installation
 
-Follow these steps on Debian based systems (Debian, Ubuntu, Kali, ...) to perform a system-wide installation of jefferon:
+You can install Jefferson from PyPi with the following command:
 
-```bash
-git clone https://github.com/sviehb/jefferson.git
-cd jefferson
-sudo apt update
-sudo apt install python3-pip liblzo2-dev
-sudo python3 -m pip install -r requirements.txt
-sudo python3 setup.py install
+```
+pip install --user jefferson
 ```
 
+### Usage
+
+```sh
+jefferson filesystem.img -d outdir
+```
 
 ### Features
 
 - big-endian and little-endian support with auto-detection
 - zlib, rtime, LZMA, and LZO compression support
 - CRC checks - for now only enforced on `hdr_crc`
 - extraction of symlinks, directories, files, and device nodes
 - detection/handling of duplicate inode numbers. Occurs if multiple JFFS2 filesystems are found in one file and causes `jefferson` to treat segments as separate filesystems
 
-### Usage
+### Development
+
+The package is maintained with Poetry. If you want to contribute, we recommend you follow these steps:
 
-```bash
-$ jefferson filesystem.img -d outdir
+```sh
+git clone https://github.com/onekey-sec/jefferson.git
+cd jefferson
+poetry install
+poetry run jefferson
 ```
 
+You can install Poetry by following this [guide](https://python-poetry.org/dos/#installation)
+
```

