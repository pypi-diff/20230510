# Comparing `tmp/cbgen-1.0.2.tar.gz` & `tmp/cbgen-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbgen-1.0.2.tar", max compression
+gzip compressed data, was "cbgen-1.0.4.tar", max compression
```

## Comparing `cbgen-1.0.2.tar` & `cbgen-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1069 2022-07-13 12:07:31.723423 cbgen-1.0.2/LICENSE
--rw-r--r--   0        0        0     1475 2022-07-13 12:07:31.723423 cbgen-1.0.2/README.md
--rw-r--r--   0        0        0     3592 2022-07-13 12:07:31.723423 cbgen-1.0.2/build_ext.py
--rw-r--r--   0        0        0      778 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/__init__.py
--rw-r--r--   0        0        0     7645 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/_bgen_file.py
--rw-r--r--   0        0        0     5286 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/_bgen_metafile.py
--rw-r--r--   0        0        0      282 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/_env.py
--rw-r--r--   0        0        0      442 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/_testit.py
--rw-r--r--   0        0        0      690 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/conftest.py
--rw-r--r--   0        0        0     1750 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/example.py
--rw-r--r--   0        0        0      535 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/genotype.c
--rw-r--r--   0        0        0      197 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/genotype.h
--rw-r--r--   0        0        0     3536 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/interface.h
--rw-r--r--   0        0        0     2682 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/partition.c
--rw-r--r--   0        0        0      676 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/partition.h
--rw-r--r--   0        0        0      923 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/samples.c
--rw-r--r--   0        0        0      308 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/samples.h
--rw-r--r--   0        0        0        0 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/test/__init__.py
--rw-r--r--   0        0        0     8100 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/test/test_bgen.py
--rw-r--r--   0        0        0     3287 2022-07-13 12:07:31.723423 cbgen-1.0.2/cbgen/typing.py
--rw-r--r--   0        0        0     1273 2022-07-13 12:07:31.727423 cbgen-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2241 2022-07-13 12:07:43.727051 cbgen-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-10 14:52:37.732816 cbgen-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1475 2023-05-10 14:52:37.732816 cbgen-1.0.4/README.md
+-rw-r--r--   0        0        0     4358 2023-05-10 14:52:37.736816 cbgen-1.0.4/build_ext.py
+-rw-r--r--   0        0        0      778 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/__init__.py
+-rw-r--r--   0        0        0     7645 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/_bgen_file.py
+-rw-r--r--   0        0        0     5286 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/_bgen_metafile.py
+-rw-r--r--   0        0        0      282 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/_env.py
+-rw-r--r--   0        0        0      442 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/_testit.py
+-rw-r--r--   0        0        0      690 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/conftest.py
+-rw-r--r--   0        0        0     1750 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/example.py
+-rw-r--r--   0        0        0      535 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/genotype.c
+-rw-r--r--   0        0        0      197 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/genotype.h
+-rw-r--r--   0        0        0     3536 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/interface.h
+-rw-r--r--   0        0        0     2682 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/partition.c
+-rw-r--r--   0        0        0      676 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/partition.h
+-rw-r--r--   0        0        0      923 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/samples.c
+-rw-r--r--   0        0        0      308 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/samples.h
+-rw-r--r--   0        0        0        0 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/test/__init__.py
+-rw-r--r--   0        0        0     8100 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/test/test_bgen.py
+-rw-r--r--   0        0        0     3287 2023-05-10 14:52:37.736816 cbgen-1.0.4/cbgen/typing.py
+-rw-r--r--   0        0        0     1250 2023-05-10 14:52:37.736816 cbgen-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 cbgen-1.0.4/PKG-INFO
```

### Comparing `cbgen-1.0.2/LICENSE` & `cbgen-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/README.md` & `cbgen-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/build_ext.py` & `cbgen-1.0.4/build_ext.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 import os
 import platform
 import shutil
 import subprocess
+import sys
 import tarfile
 import urllib.request
 from pathlib import Path
 from typing import List
 
-from cffi import FFI
-from cmake import CMAKE_BIN_DIR
 
-ffibuilder = FFI()
+def rm(folder: Path, pattern: str):
+    for filename in folder.glob(pattern):
+        filename.unlink()
 
-libs = ["bgen", "athr", "elapsed"]
 
-if platform.system() == "Windows":
-    libs += ["zstd_static", "zlibstatic"]
-else:
-    libs += ["zstd", "z"]
+def get_cmake_bin():
+    from cmake import CMAKE_BIN_DIR
 
-pwd = Path(os.path.dirname(os.path.abspath(__file__)))
+    bins = [str(v) for v in Path(CMAKE_BIN_DIR).glob("cmake*")]
+    return str(sorted(bins, key=lambda v: len(v))[0])
 
 
-def rm(folder: Path, pattern: str):
-    for filename in folder.glob(pattern):
-        filename.unlink()
+def darwin_setup():
+    os.environ.setdefault("MACOSX_DEPLOYMENT_TARGET", "11.0")
+
+    machine = platform.machine()
+    # Set by setuptools/cibuildwheels
+    archflags = os.environ.get("ARCHFLAGS")
+    if archflags is not None:
+        machine = ";".join(set(archflags.split()) & {"x86_64", "arm64"})
+
+    os.environ.setdefault("CMAKE_OSX_ARCHITECTURES", machine)
 
 
 def build_deps(pwd: Path, user: str, project: str, version: str):
     ext_dir = pwd / ".ext_deps"
     shutil.rmtree(ext_dir, ignore_errors=True)
 
     prj_dir = ext_dir / f"{project}-{version}"
@@ -44,15 +50,18 @@
 
     with open(ext_dir / tar_filename, "wb") as lf:
         lf.write(data)
 
     with tarfile.open(ext_dir / tar_filename) as tf:
         tf.extractall(ext_dir)
 
-    cmake_bin = str(next(Path(CMAKE_BIN_DIR).glob("cmake*")))
+    if sys.platform == "darwin":
+        darwin_setup()
+
+    cmake_bin = get_cmake_bin()
     subprocess.check_call(
         [
             cmake_bin,
             "-S",
             str(prj_dir),
             "-B",
             str(build_dir),
@@ -82,52 +91,70 @@
 
     if len(extra_libs) > 1:
         extra_libs.remove("curses")
 
     return list(extra_libs)
 
 
-if not os.getenv("BGEN_SKIP_BUILD_DEPS", False):
-    libs += build_deps(pwd, "limix", "bgen", "4.1.9")
+def compile_extension():
 
-with open(pwd / "cbgen" / "interface.h", "r") as f:
-    ffibuilder.cdef(f.read())
+    from cffi import FFI
 
-with open(pwd / "cbgen" / "genotype.h", "r") as f:
-    ffibuilder.cdef(f.read())
+    ffibuilder = FFI()
 
-with open(pwd / "cbgen" / "genotype.c", "r") as f:
-    genotype_c = f.read()
-
-with open(pwd / "cbgen" / "partition.h", "r") as f:
-    ffibuilder.cdef(f.read())
-
-with open(pwd / "cbgen" / "partition.c", "r") as f:
-    partition_c = f.read()
-
-with open(pwd / "cbgen" / "samples.h", "r") as f:
-    ffibuilder.cdef(f.read())
-
-with open(pwd / "cbgen" / "samples.c", "r") as f:
-    samples_c = f.read()
-
-extra_link_args: List[str] = []
-if "BGEN_EXTRA_LINK_ARGS" in os.environ:
-    extra_link_args += os.environ["BGEN_EXTRA_LINK_ARGS"].split(os.pathsep)
-
-ffibuilder.set_source(
-    "cbgen._ffi",
-    rf"""
-    #include "bgen/bgen.h"
-    {genotype_c}
-    {partition_c}
-    {samples_c}
-    """,
-    libraries=libs,
-    extra_link_args=extra_link_args,
-    language="c",
-    library_dirs=[str(pwd / ".ext_deps" / "lib"), str(pwd / ".ext_deps" / "lib64")],
-    include_dirs=[str(pwd / ".ext_deps" / "include")],
-)
+    libs = ["bgen", "athr", "elapsed"]
+
+    if platform.system() == "Windows":
+        libs += ["zstd_static", "zlibstatic"]
+    else:
+        libs += ["zstd", "z"]
+
+    pwd = Path(os.path.dirname(os.path.abspath(__file__)))
+
+    if not os.getenv("BGEN_SKIP_BUILD_DEPS", False):
+        libs += build_deps(pwd, "limix", "bgen", "4.1.9")
+
+    with open(pwd / "cbgen" / "interface.h", "r") as f:
+        ffibuilder.cdef(f.read())
+
+    with open(pwd / "cbgen" / "genotype.h", "r") as f:
+        ffibuilder.cdef(f.read())
+
+    with open(pwd / "cbgen" / "genotype.c", "r") as f:
+        genotype_c = f.read()
+
+    with open(pwd / "cbgen" / "partition.h", "r") as f:
+        ffibuilder.cdef(f.read())
+
+    with open(pwd / "cbgen" / "partition.c", "r") as f:
+        partition_c = f.read()
+
+    with open(pwd / "cbgen" / "samples.h", "r") as f:
+        ffibuilder.cdef(f.read())
+
+    with open(pwd / "cbgen" / "samples.c", "r") as f:
+        samples_c = f.read()
+
+    extra_link_args: List[str] = []
+    if "BGEN_EXTRA_LINK_ARGS" in os.environ:
+        extra_link_args += os.environ["BGEN_EXTRA_LINK_ARGS"].split(os.pathsep)
+
+    ffibuilder.set_source(
+        "cbgen._ffi",
+        rf"""
+        #include "bgen/bgen.h"
+        {genotype_c}
+        {partition_c}
+        {samples_c}
+        """,
+        libraries=libs,
+        extra_link_args=extra_link_args,
+        language="c",
+        library_dirs=[str(pwd / ".ext_deps" / "lib"), str(pwd / ".ext_deps" / "lib64")],
+        include_dirs=[str(pwd / ".ext_deps" / "include")],
+    )
 
-if __name__ == "__main__":
     ffibuilder.compile(verbose=True)
+
+
+if __name__ == "__main__":
+    compile_extension()
```

### Comparing `cbgen-1.0.2/cbgen/__init__.py` & `cbgen-1.0.4/cbgen/__init__.py`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/_bgen_file.py` & `cbgen-1.0.4/cbgen/_bgen_file.py`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/_bgen_metafile.py` & `cbgen-1.0.4/cbgen/_bgen_metafile.py`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/conftest.py` & `cbgen-1.0.4/cbgen/conftest.py`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/example.py` & `cbgen-1.0.4/cbgen/example.py`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/genotype.c` & `cbgen-1.0.4/cbgen/genotype.c`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/interface.h` & `cbgen-1.0.4/cbgen/interface.h`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/partition.c` & `cbgen-1.0.4/cbgen/partition.c`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/partition.h` & `cbgen-1.0.4/cbgen/partition.h`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/samples.c` & `cbgen-1.0.4/cbgen/samples.c`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/test/test_bgen.py` & `cbgen-1.0.4/cbgen/test/test_bgen.py`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/cbgen/typing.py` & `cbgen-1.0.4/cbgen/typing.py`

 * *Files identical despite different names*

### Comparing `cbgen-1.0.2/pyproject.toml` & `cbgen-1.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 [build-system]
-requires = ["poetry_core>=1.0.8", "cffi>=1.15.1", "cmake>=3.22.5"]
+requires = ["poetry-core>=1.0.8", "cffi>=1.15.1", "cmake>=3.22.5"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cbgen"
-version = "1.0.2"
+version = "1.0.4"
 description = "Python wrapper around a BGEN library"
 license = "MIT"
 authors = ["Carl Kadie <carlk@msn.com>", "Danilo Horta <danilo.horta@pm.me>"]
 readme = "README.md"
 repository = "https://github.com/limix/cbgen"
 homepage = "https://github.com/limix/cbgen"
 keywords = ["bgen", "reader", "genetics"]
 classifiers = ["License :: OSI Approved :: MIT License"]
 include = [
-  { path = "build_ext_deps", format = "sdist" },
   { path = "cbgen/*.c", format = "sdist" },
   { path = "cbgen/*.h", format = "sdist" },
   { path = "cbgen/*.pyd", format = "wheel" },
   { path = "cbgen/*.so", format = "wheel" },
 ]
 
 [tool.poetry.dependencies]
 appdirs = "*"
-build = "*"
 cffi = "*"
 numpy = "*"
 pooch = "*"
 pytest = "*"
-python = "^3.8"
-toml = "^0.9"
+python = ">=3.8"
+urllib3 = ">=1.26"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 isort = "*"
 pyright = "*"
 pytest = "*"
 
 [tool.poetry.build]
-script = "build_ext.py"
 generate-setup-file = false
+script = "build_ext.py"
 
 [tool.cibuildwheel]
 skip = "pp* *-win32 *_i686 *musllinux*"
 manylinux-x86_64-image = "manylinux2014"
 manylinux-aarch64-image = "manylinux2014"
 
 [tool.cibuildwheel.linux]
 before-all = "yum install -y libffi-devel"
+
+[tool.isort]
+profile = "black"
```

### Comparing `cbgen-1.0.2/PKG-INFO` & `cbgen-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: cbgen
-Version: 1.0.2
+Version: 1.0.4
 Summary: Python wrapper around a BGEN library
 Home-page: https://github.com/limix/cbgen
 License: MIT
 Keywords: bgen,reader,genetics
 Author: Carl Kadie
 Author-email: carlk@msn.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs
-Requires-Dist: build
 Requires-Dist: cffi
 Requires-Dist: numpy
 Requires-Dist: pooch
 Requires-Dist: pytest
-Requires-Dist: toml (>=0.9,<0.10)
+Requires-Dist: urllib3 (>=1.26)
 Project-URL: Repository, https://github.com/limix/cbgen
 Description-Content-Type: text/markdown
 
 # cbgen
 
 Python wrapper around a BGEN library.
 ([cbgen documentation](https://cbgen.readthedocs.io)).
```

